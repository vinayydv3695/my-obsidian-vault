# Kubernetes: The Comprehensive Guide for Deep Learning

## 1. Architecture Deep Dive

Kubernetes (K8s) is an open-source system for automating deployment, scaling, and management of containerized applications. It groups containers that make up an application into logical units for easy management and discovery.

### 1.1 The Control Plane (The Brain)
The control plane makes global decisions about the cluster (for example, scheduling), as well as detecting and responding to cluster events (for example, starting up a new pod when a deployment's replicas field is unsatisfied).

#### 1.1.1 kube-apiserver Internals
The API server is the front end for the Kubernetes control plane. It exposes the Kubernetes API and handles RESTful requests.
- **Request Flow**: Authentication -> Authorization -> Admission Control -> Schema Validation -> etcd persistence.
- **Communication**: It's the only component that communicates with etcd. All other components (kubelet, scheduler, etc.) must go through the API server to query or change the cluster state.
- **Watch Mechanism**: Allows clients (like controllers) to subscribe to changes on specific resources.

#### 1.1.2 etcd Architecture
A consistent and highly-available key value store used as Kubernetes' backing store for all cluster data.
- **Consensus**: Uses the Raft algorithm to ensure data consistency across multiple nodes.
- **Quorum**: Requires (n/2)+1 nodes to be operational to maintain a quorum.
- **Compaction**: Regularly removes old versions of keys to prevent the database from growing indefinitely.
- **Best Practice**: In production, run etcd in a cluster of 3 or 5 nodes on dedicated high-speed SSDs.

#### 1.1.3 kube-scheduler Algorithm
Watches for newly created Pods with no assigned node and selects a node for them.
1. **Filtering (Predicates)**: Finding nodes where the pod can run (e.g., sufficient CPU/memory, matching node selectors).
2. **Scoring (Priorities)**: Ranking the remaining nodes to find the best fit (e.g., nodes with the requested image already present, balanced resource usage).
3. **Binding**: The scheduler notifies the API server of its decision.

#### 1.1.4 kube-controller-manager Patterns
Runs controller processes. Each controller is a control loop that watches the shared state of the cluster through the apiserver and makes changes attempting to move the current state towards the desired state.
- **Node Controller**: Responds when nodes go down.
- **Job Controller**: Watches for Job objects and creates Pods to run tasks.
- **EndpointSlice Controller**: Populates EndpointSlice objects (link between Services and Pods).

### 1.2 Node Components (The Muscle)

#### 1.2.1 kubelet Internals
An agent that runs on each node. It ensures that containers described in PodSpecs are running and healthy.
- **Pleg (Pod Lifecycle Event Generator)**: Relies on a "sync loop" to compare the desired pod state with the actual running state.
- **CRI (Container Runtime Interface)**: A plugin interface which enables kubelet to use a wide variety of container runtimes (containerd, CRI-O).
- **Probes**: Executes Liveness, Readiness, and Startup probes.

#### 1.2.2 kube-proxy Modes
A network proxy that implements part of the Kubernetes Service concept.
- **iptables mode**: Default. Uses Netfilter rules to redirect traffic. Fast but becomes slow with thousands of services.
- **IPVS mode**: Based on Linux Virtual Server. Uses hash tables for faster lookups. Better for large-scale clusters.

### 1.3 Architecture Diagram
```text
+----------------------------------------------------------+
|                      CONTROL PLANE                       |
|                                                          |
|  +--------------+      +------------------------------+  |
|  |   API Server |<---->|            etcd              |  |
|  +--------------+      +------------------------------+  |
|         ^                                                |
|         |          +------------------------------+      |
|         +--------->|       Scheduler              |      |
|         |          +------------------------------+      |
|         |                                                |
|         |          +------------------------------+      |
|         +--------->|      Controller Manager      |      |
|                    +------------------------------+      |
+----------------------------------------------------------+
          ^                        ^
          |                        |
+---------v----------+    +--------v-----------+
|       NODE 1       |    |       NODE 2       |
|  +--------------+  |    |  +--------------+  |
|  |   Kubelet    |  |    |  |   Kubelet    |  |
|  +--------------+  |    |  +--------------+  |
|  +--------------+  |    |  +--------------+  |
|  |  Kube-Proxy  |  |    |  |  Kube-Proxy  |  |
|  +--------------+  |    |  +--------------+  |
|  +--------------+  |    |  +--------------+  |
|  |   Runtime    |  |    |  |   Runtime    |  |
|  +--------------+  |    |  +--------------+  |
+--------------------+    +--------------------+
```

---

## 2. Workloads & Controllers

### 2.1 Pods: The Atomic Unit
A Pod is the smallest deployable unit. Containers within a Pod share storage, network IP, and port space.

- **Lifecycle Phases**: `Pending` (scheduling), `Running` (at least one container up), `Succeeded` (all exited with 0), `Failed` (at least one exited non-zero), `Unknown`.
- **Init Containers**: Run to completion before app containers start. Useful for setup tasks (e.g., waiting for a DB to be ready).
- **Sidecar Patterns**: 
    - **Proxy**: e.g., Envoy for service mesh.
    - **Adapter**: e.g., transforming monitoring data.
    - **Ambassador**: e.g., local proxy for remote services.

#### Pod YAML Example
```yaml
apiVersion: v1
kind: Pod
metadata:
  name: advanced-pod
spec:
  initContainers:
  - name: wait-service
    image: busybox:1.28
    command: ['sh', '-c', 'until nslookup mydb; do echo waiting; sleep 2; done']
  containers:
  - name: app
    image: my-app:v1
    ports:
    - containerPort: 8080
  - name: log-exporter
    image: fluentd:latest
```

### 2.2 Deployments: Stateless Scaling
Manage ReplicaSets and Pods. Support rolling updates and rollbacks.

- **Rolling Update Strategy**:
    - `maxUnavailable`: Max pods that can be down during update.
    - `maxSurge`: Max pods that can be created over the desired number.
- **Rollback**: `kubectl rollout undo deployment/my-deploy`

### 2.3 StatefulSets: Ordered Identity
For apps needing stable names (`web-0`, `web-1`), stable storage (PV sticks to the same pod index), and ordered startup/shutdown.

### 2.4 DaemonSets: Node-Level Agents
Ensures a pod runs on every node (or a subset via node selectors).
- **Common use**: `kube-proxy`, `fluentd`, `node-exporter`.

### 2.5 Jobs & CronJobs
- **Jobs**: Run to completion (parallelism and completions can be tuned).
- **CronJobs**: Scheduled jobs using crontab syntax.

---

## 3. Networking & Service Discovery

### 3.1 Service Types Comparison

| Type | Internal IP | External IP | Use Case |
|------|-------------|-------------|----------|
| **ClusterIP** | Yes | No | Internal pod-to-pod communication. |
| **NodePort** | Yes | Yes (NodeIP:Port) | Basic external access (ports 30000-32767). |
| **LoadBalancer** | Yes | Yes (Cloud LB) | Standard production external exposure. |
| **ExternalName** | No | No (CNAME) | Mapping internal DNS to external domain. |

### 3.2 Service Discovery
- **DNS**: CoreDNS maps service names to ClusterIPs (e.g., `myservice.namespace.svc.cluster.local`).
- **Environment Variables**: Kubelet injects variables for every active Service when a Pod starts.

### 3.3 Ingress
A layer 7 (HTTP/HTTPS) load balancer.
- **Host-based routing**: `api.example.com` -> `api-service`, `app.example.com` -> `app-service`.
- **Path-based routing**: `/v1` -> `service-v1`, `/v2` -> `service-v2`.

#### Ingress Example
```yaml
apiVersion: networking.k8s.io/v1
kind: Ingress
metadata:
  name: main-ingress
  annotations:
    nginx.ingress.kubernetes.io/rewrite-target: /
spec:
  rules:
  - host: myapp.com
    http:
      paths:
      - path: /shop
        pathType: Prefix
        backend:
          service:
            name: shop-service
            port:
              number: 80
```

### 3.4 Network Policies (Egress & Ingress)
Default behavior is "allow all". Use NetworkPolicies to isolate namespaces or specific pods.
- **Best Practice**: Start with a "deny-all" policy and explicitly allow necessary traffic.

---

## 4. Storage & Configuration

### 4.1 Persistent Storage Lifecycle
1. **StorageClass**: Defines storage types (SSD, HDD) and provisioner (AWS EBS, GCE PD).
2. **PersistentVolume (PV)**: Cluster-wide storage resource.
3. **PersistentVolumeClaim (PVC)**: A request for storage. K8s binds PVC to PV.
4. **Volume Mount**: Pod references PVC to mount the storage into a container path.

### 4.2 ConfigMaps & Secrets
- **ConfigMaps**: Injected as environment variables, command-line arguments, or files in a volume.
- **Secrets**: Encoded as Base64.
    - **Best Practice**: Use external secrets managers (HashiCorp Vault, AWS Secrets Manager) or Bitnami Sealed Secrets for production.
    - **Encryption at rest**: Must be enabled in the API server config.

---

## 5. Security & RBAC

### 5.1 RBAC Components
- **Subject**: User, Group, or ServiceAccount.
- **Role / ClusterRole**: A set of rules (verbs like `get`, `list`, `watch` on resources like `pods`).
- **RoleBinding / ClusterRoleBinding**: Connects a Subject to a Role.

#### RBAC Example
```yaml
apiVersion: rbac.authorization.k8s.io/v1
kind: Role
metadata:
  namespace: dev
  name: pod-reader
rules:
- apiGroups: [""]
  resources: ["pods"]
  verbs: ["get", "watch", "list"]
---
apiVersion: rbac.authorization.k8s.io/v1
kind: RoleBinding
metadata:
  name: read-pods
  namespace: dev
subjects:
- kind: ServiceAccount
  name: default
  namespace: dev
roleRef:
  kind: Role
  name: pod-reader
  apiGroup: rbac.authorization.k8s.io
```

### 5.2 Pod Security Standards
- **Privileged**: Open, unrestricted policy.
- **Baseline**: Minimally restrictive, prevents known privilege escalations.
- **Restricted**: Heavily restricted, follows hardening best practices.

---

## 6. Scheduling & Optimization

### 6.1 Taints & Tolerations
- **Taint**: Applied to a Node. "I only accept pods with this specific toleration."
- **Toleration**: Applied to a Pod. "I can be scheduled on nodes with this taint."
- **Effect**: `NoSchedule`, `PreferNoSchedule`, `NoExecute`.

### 6.2 Affinity & Anti-Affinity
- **Node Affinity**: Stronger version of `nodeSelector`.
- **Pod Anti-Affinity**: Ensures that pods of the same type are not scheduled on the same node (High Availability).

### 6.3 Resource Management
- **Requests**: Guaranteed resource (scheduler uses this).
- **Limits**: Hard ceiling (K8s kills processes if memory limit exceeded; throttles if CPU limit exceeded).

---

## 7. Autoscaling

- **HPA (Horizontal Pod Autoscaler)**: Scales pod count based on CPU/Memory or custom metrics.
- **VPA (Vertical Pod Autoscaler)**: Recommends or automatically updates pod resource requests/limits.
- **Cluster Autoscaler**: Adds or removes physical nodes from the cluster.

---

## 8. Observability

- **Liveness Probes**: "Is the app alive?" (K8s restarts if it fails).
- **Readiness Probes**: "Is the app ready to handle traffic?" (K8s removes from Service endpoints if it fails).
- **Startup Probes**: "Has the app finished starting up?" (Pauses other probes until this passes).

---

## 9. Helm

Helm is the "apt-get" of Kubernetes.
- **Charts**: Templates for K8s manifests.
- **Values.yaml**: Configuration file to customize charts.
- **Release**: A running instance of a chart in the cluster.

---

## 10. Troubleshooting & Commands

### 10.1 Diagnostic Workflow
1. `kubectl get pods -A` (Find the problem).
2. `kubectl describe pod <name>` (Check Events).
3. `kubectl logs <name> --previous` (Check why it crashed).
4. `kubectl exec -it <name> -- sh` (Inspect internal state).

### 10.2 Common Issues
- **CrashLoopBackOff**: App is crashing on start. Check logs and env vars.
- **ImagePullBackOff**: Registry auth error or wrong image name.
- **Pending**: No nodes have enough resources. Check `describe` for scheduling errors.

---

## 11. Advanced Topics

- **Custom Resource Definitions (CRDs)**: Extend the K8s API with your own objects.
- **Operators**: A method of packaging, deploying, and managing a Kubernetes application using CRDs and custom controllers.
- **Admission Controllers**: Plugins that intercept requests to the API server prior to persistence (e.g., MutatingAdmissionWebhook, ValidatingAdmissionWebhook).

---

## 12. Best Practices

1. **Namespace Isolation**: Use different namespaces for dev, staging, and prod.
2. **Resource Quotas**: Set limits on namespaces to prevent one team from consuming all cluster resources.
3. **Immutable Tags**: Never use `latest`. Use SHA or version tags.
4. **Security Context**: Run containers as non-root users.
5. **Node Maintenance**: Always use `kubectl drain` before performing node maintenance.
