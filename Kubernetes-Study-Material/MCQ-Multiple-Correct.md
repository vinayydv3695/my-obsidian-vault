1. Which of the following are core components of the Kubernetes Control Plane?
   A) kube-scheduler
   B) kubelet
   C) etcd
   D) kube-proxy
   E) kube-controller-manager
   
   **Correct Answers: A, C, E**
   **Explanation:** The Control Plane includes the API server, etcd, scheduler, and controller manager. Kubelet and kube-proxy run on every worker node.

2. What can you use the `kubectl` command-line tool for?
   A) Creating new Kubernetes objects
   B) Viewing cluster logs
   C) Inspecting cluster resources
   D) Deleting namespaces
   E) Updating hardware BIOS
   
   **Correct Answers: A, B, C, D**
   **Explanation:** Kubectl is the primary tool for interacting with the Kubernetes API to manage resources, logs, and namespaces. It cannot manage hardware BIOS.

3. Which statements about a Kubernetes Pod are true?
   A) It is the smallest deployable unit in Kubernetes.
   B) It can contain only one container.
   C) Containers in a pod share the same network IP.
   D) It is always tied to a specific physical server forever.
   E) Containers in a pod share storage volumes.
   
   **Correct Answers: A, C, E**
   **Explanation:** A Pod can hold one or multiple containers that share network and storage. Pods are ephemeral and can be rescheduled to different nodes.

4. Which of these are common Kubernetes Service types?
   A) ClusterIP
   B) NodePort
   C) ExternalName
   D) LoadBalancer
   E) InternalPort
   
   **Correct Answers: A, B, C, D**
   **Explanation:** ClusterIP, NodePort, LoadBalancer, and ExternalName are the standard service types. InternalPort is not a Kubernetes service type.

5. What information is typically found in a Kubernetes YAML manifest?
   A) apiVersion
   B) kind
   C) metadata
   D) spec
   E) root password
   
   **Correct Answers: A, B, C, D**
   **Explanation:** Standard manifests require apiVersion, kind, metadata, and spec. Root passwords should never be stored in plain text manifests.

6. Which of the following are node-level components?
   A) kubelet
   B) kube-proxy
   C) container runtime
   D) cloud-controller-manager
   
   **Correct Answers: A, B, C**
   **Explanation:** Kubelet, kube-proxy, and the container runtime (like containerd) run on nodes. The cloud-controller-manager is a control plane component.

7. What are the benefits of using a Deployment instead of a bare Pod?
   A) Self-healing (restarts failed pods)
   B) Rolling updates
   C) Automatic scaling (with HPA)
   D) Ability to roll back to previous versions
   E) Physical hardware repair
   
   **Correct Answers: A, B, C, D**
   **Explanation:** Deployments provide declarative updates, scaling, and self-healing for pods. They do not handle hardware maintenance.

8. Which commands can you use to get information about pods?
   A) kubectl get pods
   B) kubectl describe pod <name>
   C) kubectl list pods
   D) kubectl view pods
   
   **Correct Answers: A, B**
   **Explanation:** 'get' and 'describe' are valid kubectl commands. 'list' and 'view' are not standard kubectl subcommands for this purpose.

9. What are common ways to provide configuration to a container in Kubernetes?
   A) Environment variables
   B) Command-line arguments
   C) ConfigMaps
   D) Secrets
   E) Hardcoding in the container image
   
   **Correct Answers: A, B, C, D**
   **Explanation:** Environment variables, arguments, ConfigMaps, and Secrets are the standard ways to inject configuration. Hardcoding is possible but not a Kubernetes feature or best practice.

10. Which of these are valid Kubernetes resource types?
    A) Namespace
    B) ReplicaSet
    C) Secret
    D) Folder
    E) ConfigMap
    
    **Correct Answers: A, B, C, E**
    **Explanation:** Namespaces, ReplicaSets, Secrets, and ConfigMaps are standard objects. 'Folder' is not a Kubernetes resource.

11. What happens when a Node in a Kubernetes cluster fails?
    A) The Control Plane stops working immediately.
    B) Pods on that node are marked for deletion after a timeout.
    C) The cluster automatically buys new hardware.
    D) The Control Plane attempts to reschedule pods to healthy nodes.
    
    **Correct Answers: B, D**
    **Explanation:** Kubernetes detects node failure and moves pods to other nodes. It does not stop the control plane or purchase hardware.

12. Which of the following can be used as a container runtime in Kubernetes?
    A) containerd
    B) CRI-O
    C) Docker Engine (via cri-dockerd)
    D) VirtualBox
    
    **Correct Answers: A, B, C**
    **Explanation:** containerd and CRI-O are common runtimes. Docker is supported through a shim. VirtualBox is a hypervisor, not a container runtime.

13. What does a Kubernetes Namespace provide?
    A) A way to divide cluster resources between multiple users.
    B) Logical isolation for resources.
    C) Faster CPU speeds for pods.
    D) Scope for names (unique names within a namespace).
    
    **Correct Answers: A, B, D**
    **Explanation:** Namespaces provide isolation and naming scopes. They do not increase hardware performance.

14. Which of these can be stored in a Kubernetes Secret?
    A) API keys
    B) Database passwords
    C) SSH keys
    D) Public website images
    E) OAuth tokens
    
    **Correct Answers: A, B, C, E**
    **Explanation:** Secrets are for sensitive data like keys and passwords. Public images are stored in registries, not secrets.

15. What are the characteristics of a Kubernetes ReplicaSet?
    A) It ensures a specific number of pod replicas are running.
    B) It can acquire pods that match its selector.
    C) It creates new pods if some fail or are deleted.
    D) It manages the physical power supply of the node.
    
    **Correct Answers: A, B, C**
    **Explanation:** ReplicaSets maintain the desired count of pods. They have no control over hardware power.

16. Which fields are found in the 'metadata' section of a resource?
    A) name
    B) labels
    C) annotations
    D) container image
    E) namespace
    
    **Correct Answers: A, B, C, E**
    **Explanation:** Name, labels, annotations, and namespace are metadata. The container image is part of the 'spec' section.

17. What is the purpose of 'Labels' in Kubernetes?
    A) To organize and select subsets of objects.
    B) To store non-identifying information for tools.
    C) To attach identifying metadata to objects.
    D) To encrypt container traffic.
    
    **Correct Answers: A, C**
    **Explanation:** Labels are identifying key-value pairs used for selection. Annotations are for non-identifying data. Labels do not provide encryption.

18. Which of these are valid ways to delete a pod?
    A) kubectl delete pod <name>
    B) kubectl remove pod <name>
    C) kubectl delete -f <file.yaml>
    D) kubectl kill pod <name>
    
    **Correct Answers: A, C**
    **Explanation:** 'delete' is the correct command, used either by name or by reference to the manifest file. 'remove' and 'kill' are not valid.

19. What is 'etcd' used for in a Kubernetes cluster?
    A) Storing the entire cluster state.
    B) Storing configuration data.
    C) Serving as the primary web UI.
    D) Acting as the cluster's "source of truth".
    
    **Correct Answers: A, B, D**
    **Explanation:** etcd is a distributed key-value store for all cluster data. The Dashboard or Lens are web UIs.

20. Which statements about 'kube-proxy' are correct?
    A) It runs on every node.
    B) It manages network rules on nodes.
    C) It schedules pods onto nodes.
    D) It allows network communication to pods from inside or outside the cluster.
    
    **Correct Answers: A, B, D**
    **Explanation:** kube-proxy handles host-level networking for services. The scheduler handles pod placement.

21. What are valid states (Phases) for a Kubernetes Pod?
    A) Pending
    B) Running
    C) Succeeded
    D) Failed
    E) Sleeping
    
    **Correct Answers: A, B, C, D**
    **Explanation:** The official pod phases are Pending, Running, Succeeded, Failed, and Unknown. 'Sleeping' is not a pod phase.

22. Which of these can be used to limit resource usage of a container?
    A) spec.containers[].resources.limits.cpu
    B) spec.containers[].resources.requests.memory
    C) spec.node.hardware.limit
    D) spec.containers[].resources.limits.memory
    
    **Correct Answers: A, B, D**
    **Explanation:** Resource limits and requests are defined in the container spec. There is no 'node.hardware.limit' in a standard pod spec.

23. What does the 'Succeeded' pod phase mean?
    A) The pod has been deleted.
    B) All containers in the pod have terminated in success.
    C) The pod will not be restarted.
    D) The pod is currently downloading its image.
    
    **Correct Answers: B, C**
    **Explanation:** Succeeded means the containers exited with code 0 and won't restart. Image pulling happens in the Pending phase.

24. Which components belong to the worker node?
    A) kubelet
    B) kube-proxy
    C) etcd
    D) container runtime
    E) kube-apiserver
    
    **Correct Answers: A, B, D**
    **Explanation:** Kubelet, proxy, and runtime are on worker nodes. API server and etcd are part of the Control Plane.

25. What is the role of the 'kube-scheduler'?
    A) It watches for newly created pods with no assigned node.
    B) It selects a node for the pod to run on.
    C) It pulls images from the registry.
    D) It restarts failed containers.
    
    **Correct Answers: A, B**
    **Explanation:** The scheduler assigns pods to nodes. Kubelet handles image pulling and container restarts.

26. Which of these are valid `kubectl get` options?
    A) -o yaml (output as YAML)
    B) -n <namespace> (specify namespace)
    C) -A (all namespaces)
    D) -w (watch for changes)
    E) -f (force delete)
    
    **Correct Answers: A, B, C, D**
    **Explanation:** YAML output, namespace filtering, and watching are all valid 'get' flags. '-f' is used for filenames in 'get', but 'force' is for the 'delete' command.

27. What are the main parts of a Service's spec?
    A) selector
    B) ports
    C) type
    D) replicationFactor
    
    **Correct Answers: A, B, C**
    **Explanation:** Services use selectors to find pods, define ports, and specify a type. replicationFactor is part of a ReplicaSet or Deployment.

28. Which of the following describe 'ConfigMaps'?
    A) Used to store non-confidential data.
    B) Can be consumed as environment variables.
    C) Can be mounted as files in a volume.
    D) They automatically encrypt all data.
    
    **Correct Answers: A, B, C**
    **Explanation:** ConfigMaps are for plain-text config and can be used as env vars or files. They do not provide encryption (Secrets do).

29. What is a 'Liveness Probe' used for?
    A) To check if a container is running.
    B) To decide when to restart a container.
    C) To check if a container is ready to accept traffic.
    D) To measure the CPU temperature.
    
    **Correct Answers: A, B**
    **Explanation:** Liveness probes detect when to restart a container. Readiness probes determine when a container can receive traffic.

30. Which commands help in troubleshooting a failing pod?
    A) kubectl logs <pod-name>
    B) kubectl describe pod <pod-name>
    C) kubectl get events
    D) kubectl edit bios
    
    **Correct Answers: A, B, C**
    **Explanation:** Logs, describe, and events are essential for debugging. There is no kubectl command for BIOS.
1. Which of the following describe the behavior of a Kubernetes Deployment when updating the container image?
   A) It creates a new ReplicaSet to manage the new pods.
   B) It immediately deletes all old pods before starting new ones.
   C) It allows configuring the maxUnavailable parameter to control how many pods can be down during the rollout.
   D) It automatically rolls back if the new pods fail their readiness probes.
   E) It maintains the history of previous ReplicaSets to allow for rollbacks.

   **Correct Answers: A, C, E**
   **Explanation:** A Deployment creates a new ReplicaSet for the new version while scaling down the old ReplicaSet. The maxUnavailable parameter controls the update pace. Deployments keep old ReplicaSets (up to the revisionHistoryLimit) to facilitate rollbacks. It does not delete all old pods at once unless specifically configured with a Recreate strategy, and it doesn't automatically rollback on failure unless external tools or specific operators are used.

2. A Service of type NodePort is created. Which statements are true regarding its accessibility?
   A) It is accessible on the cluster IP from within the cluster.
   B) It is accessible on every node's IP at the specified static port.
   C) It requires an external load balancer to function.
   D) It automatically allocates a port in the range 30000-32767 by default.
   E) It can only be reached by pods on the same node.

   **Correct Answers: A, B, D**
   **Explanation:** NodePort services are extensions of ClusterIP, so they have a cluster-internal IP. They open a port on every node in the cluster. The default port range is 30000-32767. They do not require an external load balancer, though one can be used to route traffic to the nodes.

3. Which of the following are valid ways to inject configuration data into a pod using a ConfigMap?
   A) Mapping the ConfigMap as a volume in the pod specification.
   B) Using the configMapKeyRef in the container's env section.
   C) Using the envFrom field to define all ConfigMap data as environment variables.
   D) Directly hardcoding the ConfigMap YAML into the pod's metadata.
   E) Passing the ConfigMap name as a command-line argument to the entrypoint.

   **Correct Answers: A, B, C**
   **Explanation:** ConfigMaps can be mounted as volumes where each key becomes a file. They can also be used to set specific environment variables using configMapKeyRef or all keys at once using envFrom. Hardcoding the YAML into metadata is not a valid injection method.

4. When defining resource requests and limits for a container, which statements are correct?
   A) Requests are used by the scheduler to decide which node to place the pod on.
   B) If a container exceeds its CPU limit, it is immediately terminated (OOMKilled).
   C) If a container exceeds its memory limit, it is a candidate for termination.
   D) Limits can be smaller than requests.
   E) CPU is a compressible resource, meaning the container will be throttled rather than killed if it hits the limit.

   **Correct Answers: A, C, E**
   **Explanation:** The scheduler uses requests to ensure a node has enough capacity. Memory is non-compressible; exceeding the limit leads to the container being killed. CPU is compressible; exceeding the limit leads to throttling. Limits must always be greater than or equal to requests.

5. Which components are part of the Kubernetes Control Plane?
   A) kube-proxy
   B) kube-apiserver
   ) etcd
   D) kubelet
   E) kube-scheduler

   **Correct Answers: B, C, E**
   **Explanation:** The control plane includes the API server, etcd (the data store), the scheduler, and the controller manager. kube-proxy and kubelet are node-level components that run on every node in the cluster.

6. What happens when a PersistentVolumeClaim (PVC) is deleted in a cluster using the 'Retain' reclaim policy?
   A) The corresponding PersistentVolume (PV) is automatically deleted.
   B) The PV remains in the cluster but is marked as 'Released'.
   C) The data on the underlying storage is immediately wiped.
   D) The PV cannot be claimed by another PVC until it is manually handled.
   E) The PV is reformatted and returned to the 'Available' pool.

   **Correct Answers: B, D**
   **Explanation:** With the 'Retain' policy, the PV is not deleted or wiped. It moves to the 'Released' state. It is not available for another claim until the administrator manually deletes the PV or cleans up the data and recreates the PV object.

7. Which of the following are true about Kubernetes Secrets?
   A) They are encrypted at rest by default in all Kubernetes installations.
   B) They are stored in etcd.
   C) They are base64 encoded, which is not the same as encryption.
   D) They can be mounted as volumes or injected as environment variables.
   E) A pod can only use Secrets that are in the same namespace.

   **Correct Answers: B, C, D, E**
   **Explanation:** Secrets are stored in etcd. By default, they are only base64 encoded, not encrypted (unless encryption at rest is specifically configured). Like ConfigMaps, they can be mounted or used as env vars. They are namespace-scoped objects.

8. Identify the correct statements regarding Kubernetes Namespaces.
   A) They provide a way to divide cluster resources between multiple users.
   B) All Kubernetes resources must belong to a namespace.
   C) ResourceQuotas can be applied at the namespace level.
   D) Pods in different namespaces cannot communicate with each other by default.
   E) Namespaces provide a scope for names, allowing duplicate names in different namespaces.

   **Correct Answers: A, C, E**
   **Explanation:** Namespaces help with multi-tenancy and resource isolation via ResourceQuotas. Names must be unique within a namespace but can be duplicated across different ones. Some resources (like Nodes and PersistentVolumes) are cluster-wide and do not belong to a namespace. Pods can communicate across namespaces unless NetworkPolicies are implemented.

9. Which fields are required in every Kubernetes object configuration?
   A) apiVersion
   B) kind
   C) status
   D) metadata
   E) spec

   **Correct Answers: A, B, D**
   **Explanation:** Every object needs apiVersion, kind, and metadata. Most objects also need a spec to define the desired state, but it is not strictly required for all object types (though common). The status field is managed by the cluster, not the user.

10. A ReplicaSet's primary responsibility is to:
    A) Ensure a specified number of pod replicas are running at any given time.
    B) Handle the rolling update of container images.
    C) Scale pods based on CPU utilization.
    D) Replace pods that fail or are deleted.
    E) Balance traffic between pods.

    **Correct Answers: A, D**
    **Explanation:** ReplicaSets ensure the desired count of pods is maintained. If a pod fails or is manually deleted, the ReplicaSet creates a new one. Rolling updates are handled by Deployments (which use ReplicaSets), and auto-scaling is handled by the Horizontal Pod Autoscaler. Traffic balancing is the job of Services.

11. Which of the following are valid Service types in Kubernetes?
    A) ClusterIP
    B) NodePort
    C) LoadBalancer
    D) ExternalName
    E) Ingress

    **Correct Answers: A, B, C, D**
    **Explanation:** ClusterIP, NodePort, LoadBalancer, and ExternalName are all valid Service types. Ingress is a separate resource type used to manage external access to services, typically via HTTP/HTTPS.

12. Regarding Liveness and Readiness probes, which statements are true?
    A) A failed Liveness probe causes the container to be restarted.
    B) A failed Readiness probe causes the container to be restarted.
    C) A failed Readiness probe removes the pod from the Service's endpoints.
    D) Both probes can use HTTP GET, TCP Socket, or Exec commands.
    E) Probes are executed by the API server.

    **Correct Answers: A, C, D**
    **Explanation:** Liveness probes restart unhealthy containers. Readiness probes stop traffic from being sent to the pod by removing it from service endpoints but do not restart the container. Both support the same check mechanisms. Probes are executed by the kubelet on the node, not the API server.

13. Which of the following describe a 'Sidecar' container pattern?
    A) A container that runs before the main application container starts.
    B) A container that runs in the same pod as the main application container.
    C) A container used to ship logs or provide a proxy for the main application.
    D) A container that shares the same network namespace as the main container.
    E) A container that must have a different lifecycle than the main container.

    **Correct Answers: B, C, D**
    **Explanation:** Sidecars are helper containers in the same pod that share the network and storage. They are used for auxiliary tasks like logging or proxying. Containers that run before the main one are called Init Containers.

14. What are the characteristics of a Kubernetes Job?
    A) It ensures that a specified number of pods terminate with success.
    B) It is used for long-running processes like web servers.
    C) It can run multiple pods in parallel.
    D) It restarts the pod indefinitely if it fails.
    E) It can be configured to clean up completed pods automatically using a TTL controller.

    **Correct Answers: A, C, E**
    **Explanation:** Jobs are for batch tasks that run to completion. They can run parallel replicas. They have a retry limit (backoffLimit) rather than restarting indefinitely. The ttlSecondsAfterFinished attribute allows for automatic cleanup.

15. Which of the following are true about DaemonSets?
    A) They ensure a copy of a pod runs on all (or some) nodes.
    B) They are typically used for cluster storage, log collection, or node monitoring.
    C) Deleting a DaemonSet will leave the pods running on the nodes.
    D) They automatically add pods to new nodes as they are added to the cluster.
    E) They can only run on worker nodes, never on master nodes.

    **Correct Answers: A, B, D**
    **Explanation:** DaemonSets manage node-level tasks and ensure the pod exists on all matching nodes. When a DaemonSet is deleted, its pods are also deleted by default. They can run on any node that doesn't have a taints preventing it (including control plane nodes if taints are tolerated).

16. What is the role of the kube-proxy component?
    A) It manages the pod network interface on each node.
    B) It maintains network rules on nodes to allow network communication to pods from sessions inside or outside the cluster.
    C) It implements the Kubernetes Service abstraction.
    D) It acts as an API gateway for the cluster.
    E) It can use IPVS or iptables to handle traffic redirection.

    **Correct Answers: B, C, E**
    **Explanation:** kube-proxy manages the networking for Services on each node, using iptables or IPVS to route traffic to the correct backend pods. It does not manage the pod network interfaces (that's the CNI plugin) or act as an API gateway.

17. Which statements correctly describe Kubernetes Taints and Tolerations?
    A) Taints are applied to pods to restrict which nodes they can join.
    B) Taints are applied to nodes to repel a set of pods.
    C) Tolerations are applied to pods to allow them to schedule on tainted nodes.
    D) A pod with a matching toleration is guaranteed to be scheduled on the tainted node.
    E) Taints can have effects like NoSchedule, PreferNoSchedule, and NoExecute.

    **Correct Answers: B, C, E**
    **Explanation:** Taints are node properties, while tolerations are pod properties. Tolerations allow pods to be scheduled on tainted nodes but do not guarantee it (the scheduler still considers other factors). Common effects include NoSchedule and NoExecute.

18. What are the benefits of using a Headless Service (clusterIP: None)?
    A) It allows for direct pod-to-pod communication without a proxy.
    B) It provides a single stable IP for a group of pods.
    C) DNS queries for the service return the A records (IPs) of all ready pods.
    D) It is required for creating a LoadBalancer service.
    E) It is commonly used with StatefulSets to discover individual pod identities.

    **Correct Answers: A, C, E**
    **Explanation:** Headless services don't have a cluster IP. Instead, they allow DNS to return the individual pod IPs, which is useful for stateful applications where pods need to know about each other's identity.

19. Which of the following are valid volume types in Kubernetes?
    A) emptyDir
    B) hostPath
    C) nfs
    D) configMap
    E) persistentVolumeClaim
    F) local

    **Correct Answers: A, B, C, D, E, F**
    **Explanation:** All listed are valid volume types. emptyDir is for temporary storage, hostPath and local are for node-specific storage, nfs is for networked storage, and configMap/PVC are ways to mount data into containers.

20. When using RBAC, which of the following are valid subjects for a RoleBinding?
    A) User
    B) Group
    C) ServiceAccount
    D) Pod
    E) Namespace

    **Correct Answers: A, B, C**
    **Explanation:** RoleBindings link roles to users, groups, or service accounts. Pods and namespaces are not subjects themselves; pods use service accounts to interact with the API, and namespaces are scopes for resources.

21. What does the 'imagePullPolicy: IfNotPresent' setting do?
    A) Always pulls the image from the registry to ensure it's up to date.
    B) Only pulls the image if it is not already cached on the node.
    C) Fails if the image is already present on the node.
    D) Is the default policy if the image tag is ':latest'.
    E) Is the default policy if the image tag is anything other than ':latest'.

    **Correct Answers: B, E**
    **Explanation:** IfNotPresent skips pulling if the image exists locally. It is the default for tagged images (except :latest, where 'Always' is the default).

22. Which of the following describe the behavior of a StatefulSet?
    A) Pods are created with a stable, unique network identifier.
    B) Pods are created in a random order to speed up deployment.
    C) Persistent storage is linked to the specific pod index.
    D) When a StatefulSet is scaled down, pods are deleted in reverse ordinal order.
    E) It is primarily used for stateless web applications.

    **Correct Answers: A, C, D**
    **Explanation:** StatefulSets provide stable identities (pod-0, pod-1) and ensure storage persists across restarts for each specific index. Pods are created and deleted in a strict order (0 to N-1). They are for stateful apps like databases.

23. Which of the following are components of a Persistent Volume workflow?
    A) StorageClass
    B) PersistentVolume
    C) PersistentVolumeClaim
    D) VolumeAttachment
    E) StorageProvider

    **Correct Answers: A, B, C**
    **Explanation:** The core user-facing workflow involves the StorageClass (template), the PersistentVolume (actual storage resource), and the PersistentVolumeClaim (user request for storage). VolumeAttachment is an internal API object.

24. How can you restrict network traffic between pods in Kubernetes?
    A) Using SecurityContext in the pod spec.
    B) Implementing NetworkPolicies.
    C) Changing the Service type to ClusterIP.
    D) Using a CNI plugin that supports NetworkPolicies (like Calico or Cilium).
    E) Configuring firewall rules on the underlying nodes.

    **Correct Answers: B, D**
    **Explanation:** NetworkPolicies define how pods communicate. However, they require a CNI plugin that supports and enforces these policies to function. SecurityContext is for OS-level permissions, not networking.

25. What information is typically found in the 'status' section of a Kubernetes object?
    A) The desired number of replicas.
    B) The current number of running replicas.
    C) Conditions like 'Ready' or 'Available'.
    D) The container image being used.
    E) Observed generation of the resource.

    **Correct Answers: B, C, E**
    **Explanation:** Status reflects the actual state of the system. Desired replicas and container images are part of the 'spec'. Conditions and observed generation help controllers determine if the current state matches the desired state.

26. Which of the following are true about Init Containers?
    A) They always run to completion before the main containers start.
    B) If an Init Container fails, the pod is always restarted.
    C) They share the same network namespace and volumes as the main containers.
    D) They can have different resource limits than the main containers.
    E) They run in parallel with the main containers to speed up startup.

    **Correct Answers: A, C, D**
    **Explanation:** Init containers run sequentially and must finish successfully. They share the same pod environment. If an init container fails, the pod is restarted unless the restartPolicy is Never. They do not run in parallel with main containers.

27. A Horizontal Pod Autoscaler (HPA) can scale which of the following?
    A) Deployments
    B) ReplicaSets
    C) StatefulSets
    D) DaemonSets
    E) Static Pods

    **Correct Answers: A, B, C**
    **Explanation:** HPA can scale objects that support the /scale subresource, which includes Deployments, ReplicaSets, and StatefulSets. DaemonSets cannot be scaled this way as they are tied to nodes, and static pods are managed by kubelet directly.

28. What are 'Annotations' used for in Kubernetes?
    A) To select a group of pods for a Service.
    B) To store non-identifying metadata for external tools and libraries.
    C) To provide information for the scheduler to place pods.
    D) To store build or release information like timestamps or git hashes.
    E) To configure behavior for Ingress controllers.

    **Correct Answers: B, D, E**
    **Explanation:** Unlike labels, annotations are not used for selection (filtering). They store larger, non-queryable metadata that tools or controllers (like Ingress) use for configuration.

29. Which of the following are valid strategies for a Deployment rollout?
    A) RollingUpdate
    B) Recreate
    C) BlueGreen
    D) Canary
    E) Shadow

    **Correct Answers: A, B**
    **Explanation:** Native Kubernetes Deployment objects only support RollingUpdate and Recreate. Strategies like BlueGreen and Canary are achieved by managing multiple Deployments or using external tools like Argo Rollouts or Istio.

30. What happens if a pod is evicted from a node?
    A) The kubelet on that node deletes the pod.
    B) The pod is automatically rescheduled by the API server.
    C) If managed by a Deployment, a new pod is created on a different node.
    D) The pod's data in an 'emptyDir' volume is lost.
    E) The pod stays in 'Failed' state on the original node until manually deleted.

    **Correct Answers: A, C, D**
    **Explanation:** Eviction leads to the termination of the pod on that node, resulting in the loss of local temporary data (emptyDir). If the pod is part of a controller (like a Deployment), the controller will notice the missing replica and create a new one elsewhere. The API server does not reschedule pods; controllers do.
1. When a CustomResourceDefinition (CRD) is created in a cluster, which of the following events occur within the Kubernetes control plane?
   A) The kube-apiserver registers a new RESTful resource path.
   B) The kube-controller-manager automatically spawns a generic controller for the new resource.
   C) The custom resource storage is initialized in etcd under a new prefix.
   D) The kube-scheduler is updated with internal logic to handle the new resource type.
   E) The discovery API is updated so clients like kubectl can find the new resource.
   F) OpenAPI v3 schemas are validated and served for the new resource.
   
   **Correct Answers: A, C, E, F**
   **Explanation:** When a CRD is established, the kube-apiserver creates a new REST endpoint. It handles storage in etcd, usually under /registry/group/resource. It also updates the discovery information so clients know the resource exists and provides OpenAPI schemas for validation and client-side tool generation. The controller-manager and scheduler do not automatically gain logic for custom resources; that requires an external operator or custom controller.

2. Which mechanisms does the Kubernetes API server use to ensure data consistency and prevent "lost updates" during concurrent modifications?
   A) Distributed locking via the lease API on every object.
   B) Optimistic concurrency control using the resourceVersion field.
   C) Strict two-phase commit protocols across all etcd replicas.
   D) Rejection of PUT requests if the provided resourceVersion does not match the server state.
   E) Server-side Apply (SSA) which tracks field ownership to resolve conflicts.
   F) Mandatory admission webhooks that sequence all writes.
   
   **Correct Answers: B, D, E**
   **Explanation:** Kubernetes primarily uses optimistic concurrency control. Every object has a resourceVersion. If a client tries to update a resource (PUT) with an outdated version, the server returns a 409 Conflict. Server-side Apply (SSA) is a newer mechanism that allows multiple actors to manage different fields of the same object without overwriting each other, using field managers to track ownership. Kubernetes does not use distributed locks for every object update, nor does it rely on admission webhooks for basic sequencing or consistency.

3. Regarding the Admission Controller chain, which statements accurately describe its execution flow and characteristics?
   A) Mutating admission controllers run before Validating admission controllers.
   B) If a Mutating admission controller modifies an object, the chain restarts from the beginning of the Mutating phase.
   C) Validating admission controllers can modify the object to ensure it meets organizational standards.
   D) Admission controllers only run on requests that modify state (Create, Update, Delete, Connect), not on Get or List.
   E) All admission controllers must be compiled into the kube-apiserver binary.
   F) Webhook admission controllers can be used to implement custom logic outside the apiserver.
   
   **Correct Answers: A, B, D, F**
   **Explanation:** The admission chain follows a strict order: Mutating controllers first, then Validating. If a mutation occurs, the Mutating phase can re-trigger to ensure all controllers see the final state. Validating controllers are strictly read-only regarding the object. Admission logic is skipped for read-only operations like Get/List. While some are "In-Tree" (compiled in), "Out-of-Tree" webhooks allow external logic.

4. In a complex operator pattern using the Controller Runtime (Kube-builder), what are the primary functions of the Cache/Informer?
   A) To reduce load on the API server by serving Read requests from local memory.
   B) To provide a synchronous interface for creating and deleting resources.
   C) To trigger the Reconcile loop via Watches when resources change.
   D) To manage the leader election process for high-availability deployments.
   E) To transform raw etcd data into typed Go structs.
   F) To implement the "Level Triggered" logic by maintaining a local state of the world.
   
   **Correct Answers: A, C, E, F**
   **Explanation:** Informers/Caches are the heart of the "List-Watch" pattern. They maintain a local, indexed copy of resources to avoid constant API server polling. They trigger Reconcile loops when events occur. They also handle the serialization from JSON/Protobuf into Go objects. Leader election is usually handled by a separate manager component, not the cache itself.

5. What are the consequences of setting the `finalizers` field on a Kubernetes object?
   A) It prevents the object from being physically deleted from etcd until the list is empty.
   B) It immediately puts the object in a "Terminating" state upon a delete request.
   C) It automatically triggers a cascading deletion of all child resources.
   D) It sets the `deletionTimestamp` field to a non-nil value when a deletion is requested.
   E) It forces the kube-scheduler to evict pods associated with the resource.
   F) It allows controllers to perform cleanup logic before the resource is purged.
   
   **Correct Answers: A, B, D, F**
   **Explanation:** Finalizers are used for asynchronous cleanup. When a delete request is made, if finalizers exist, Kubernetes sets a `deletionTimestamp` and puts the object in "Terminating" state but does not remove it from etcd. Controllers see this and perform cleanup, then remove their specific string from the finalizers list. Once empty, the API server deletes the object. It does not automatically handle cascading deletion; that is managed by OwnerReferences.

6. Which components or features are involved in the "Aggregated API Server" pattern in Kubernetes?
   A) An APIService object that registers the API group and version.
   B) The Extension API server which runs as a separate pod.
   C) The kube-aggregator module within the main kube-apiserver.
   D) Shared etcd storage between the main server and the aggregated server.
   E) Front-proxy certificates for authentication between the main apiserver and the extension server.
   F) CNI plugins for routing traffic to the extension server.
   
   **Correct Answers: A, B, C, E**
   **Explanation:** Aggregated APIs allow developers to write their own API server (extension server) and register it with the main cluster using an APIService object. The kube-aggregator acts as a proxy. Usually, extension servers have their own storage (their own etcd or database) to keep the main etcd clean. Front-proxy certificates are essential for the main apiserver to securely identify itself to the extension server.

7. When troubleshooting a "Timed out waiting for cache to sync" error in a custom controller, what are the most likely root causes?
   A) The controller's ServiceAccount lacks "list" and "watch" permissions for the target resource.
   B) The API server is under heavy load and cannot fulfill the initial LIST request.
   C) The controller is trying to watch a resource that has not been defined (missing CRD).
   D) The etcd cluster has lost quorum.
   E) The controller is running on a node with no network connectivity to the API server.
   F) The resource being watched has too many objects, exceeding the controller's memory limits.
   
   **Correct Answers: A, B, C, E**
   **Explanation:** Cache sync failure means the Informer cannot perform the initial List and start the Watch. Permission issues (RBAC) are a very common cause. API server saturation or network issues between the controller and apiserver also prevent the sync. If the CRD is missing, the API server returns a 404, causing the sync to fail. High object count might cause a crash or slowness, but usually, the "sync" itself is about the connection and initial handshake.

8. Which fields in the `CustomResourceDefinition` spec are used to manage versioning and schema evolution?
   A) `spec.versions[].served`: Determines if the version is accessible via the API.
   B) `spec.versions[].storage`: Identifies which version is used to persist data in etcd.
   C) `spec.conversion`: Defines how to translate objects between different versions.
   D) `spec.preserveUnknownFields`: Controls whether fields not in the schema are dropped.
   E) `spec.versions[].schema`: Provides the validation rules for each specific version.
   F) `spec.group`: Changes the base URL for the API to avoid conflicts.
   
   **Correct Answers: A, B, C, E**
   **Explanation:** CRD versioning is handled within the `versions` array. `served` toggles visibility. Only one version can be the `storage` version. `conversion` (often via a webhook) handles multi-version logic. `schema` defines the per-version structure. `preserveUnknownFields` is a legacy field (mostly replaced by structural schemas) but it doesn't manage versioning evolution directly. `group` defines the API identity, changing it creates a completely different resource.

9. What is the role of the `Discovery` and `OpenAPI` endpoints in the Kubernetes API?
   A) They provide the metadata needed for `kubectl` to perform client-side validation.
   B) They allow the `kube-scheduler` to understand resource requirements for custom types.
   C) They enable dynamic client generation (e.g., in Python or Go).
   D) They are used by `kube-proxy` to generate iptables rules for Services.
   E) They provide a list of all available GVRs (Group, Version, Resource) in the cluster.
   F) They allow the API server to perform server-side field pruning.
   
   **Correct Answers: A, C, E**
   **Explanation:** Discovery endpoints (/api, /apis) list available resources. OpenAPI endpoints (/openapi/v2 or /v3) provide full schemas. This information is crucial for CLI tools to know what commands are valid and for dynamic clients to work without pre-compiled types. The scheduler and proxy use internal logic or specific resource fields, not the general discovery API for their core operations.

10. In the context of "OwnerReferences", what happens when a "Foreground" deletion policy is used?
    A) The owner is deleted first, then the children are deleted.
    B) The owner enters a "deletion in progress" state and remains until all children are gone.
    C) Children are deleted immediately, regardless of their own finalizers.
    D) The API server sets the `blockOwnerDeletion` field to true on the children.
    E) The garbage collector handles the deletion of dependents before removing the owner.
    F) The user must manually delete every child before the owner can be removed.
    
    **Correct Answers: B, D, E**
    **Explanation:** With Foreground deletion, the owner's `deletionTimestamp` is set, and it stays in "Terminating" state. The garbage collector then deletes all dependents that have `blockOwnerDeletion: true`. Once dependents are gone, the owner is deleted. This is the opposite of Background deletion, where the owner is deleted first and children are cleaned up later.

11. Which components or headers are used by the Container Network Interface (CNI) to configure pod networking?
    A) The `CNI_COMMAND` environment variable to specify the action (ADD, DEL, CHECK).
    B) Standard input (stdin) to pass JSON configuration to the plugin.
    C) The `kube-proxy` configuration file to determine the CIDR range.
    D) The `CNI_PATH` environment variable to locate plugin binaries.
    E) The `CNI_IFNAME` environment variable to set the interface name inside the container.
    F) The `CNI_NETNS` environment variable to specify the network namespace path.
    
    **Correct Answers: A, B, D, E, F**
    **Explanation:** CNI is an executable-based protocol. The runtime calls binaries with specific environment variables (CNI_COMMAND, CNI_PATH, CNI_IFNAME, CNI_NETNS) and passes the network configuration via stdin as JSON. kube-proxy is not part of the pod-to-node CNI setup; it handles Service-level load balancing.

12. How does the "IP-per-Pod" model in Kubernetes differ from traditional Docker networking?
    A) Every pod has a unique IP address that is reachable from all other pods in the cluster without NAT.
    B) Pods use the host's IP address and distinct ports for communication.
    C) Containers within the same pod share the same network namespace and IP.
    D) Nodes must act as routers or use an overlay to ensure pod IPs are routable across node boundaries.
    E) Kubernetes requires an external LoadBalancer to route traffic between pods on different nodes.
    F) Pod IPs are ephemeral and can change if a pod is rescheduled.
    
    **Correct Answers: A, C, D, F**
    **Explanation:** In Kubernetes, every pod gets its own IP, shared by all containers in that pod. This IP must be routable across the cluster without NAT (the "flat network" requirement). This is achieved via overlays (VXLAN, Geneve) or direct routing (BGP, VPC routing). Pod IPs are indeed ephemeral. Traditional Docker often relies on host-port mapping or bridge-local NAT, which Kubernetes avoids for internal pod-to-pod traffic.

13. What are the characteristics of the "IPVS" mode in `kube-proxy` compared to the "iptables" mode?
    A) IPVS uses hash tables for rule lookup, providing O(1) performance regardless of Service count.
    B) IPVS supports more load-balancing algorithms (e.g., least connection, shortest expected delay).
    C) iptables mode is inherently more secure because it integrates better with NetworkPolicies.
    D) IPVS is implemented in kernel space, reducing the overhead of context switching.
    E) iptables rules grow linearly (O(n)) with the number of Services, leading to latency at scale.
    F) IPVS requires the installation of specific kernel modules on the host.
    
    **Correct Answers: A, B, D, E, F**
    **Explanation:** IPVS is designed for high-performance load balancing. Unlike iptables, which performs a sequential scan of rules (O(n)), IPVS uses hash tables (O(1)), making it much faster for clusters with thousands of Services. It also offers advanced balancing algorithms. Both operate in kernel space, but IPVS is specialized. iptables is the default and does not require extra modules, whereas IPVS does. Security (NetworkPolicy) is usually handled by the CNI, not the kube-proxy mode itself.

14. In a Service Mesh like Istio or Linkerd, how is "mTLS" (Mutual TLS) typically enforced and managed?
    A) The control plane issues X.509 certificates to each workload identity.
    B) Sidecar proxies (e.g., Envoy) intercept all incoming and outgoing TCP traffic.
    C) Applications must be modified to use specific TLS libraries.
    D) The sidecar proxy handles the TLS handshake and encryption/decryption transparently.
    E) Certificates are rotated automatically by the mesh control plane.
    F) mTLS can be configured in "Permissive" mode to allow both encrypted and plaintext traffic during migration.
    
    **Correct Answers: A, B, D, E, F**
    **Explanation:** Service meshes provide "transparent" mTLS. Sidecars intercept traffic, use certificates provided by the control plane (like Istiod), and handle the encryption. This requires no application code changes. Automatic rotation is a core feature. Permissive mode is a standard transition state.

15. What are the primary functions of the "Pause" container (also known as the infra container) in a Kubernetes pod?
    A) It serves as the parent process for all other containers in the pod to reap zombie processes.
    B) It holds the network namespace for the pod, allowing other containers to join it.
    C) It provides a small filesystem for storing shared secrets and configmaps.
    D) It acts as a health check agent for the other containers.
    E) It manages the IPC and UTS namespaces for the pod.
    F) It stays alive for the duration of the pod's life, even if other containers restart.
    
    **Correct Answers: B, E, F**
    **Explanation:** The pause container's main job is to "hold" the namespaces (Network, IPC, UTS). When a pod is created, the runtime starts the pause container first, creates the namespaces, and then joins all other containers to those namespaces. This allows containers in a pod to communicate via localhost and share a lifecycle. It does not act as a general init/reaper for application processes (each container has its own PID 1 unless PID sharing is enabled).

16. Which of the following are valid reasons for a pod to be stuck in `ImagePullBackOff`?
    A) The container image does not exist in the specified registry.
    B) The node's disk is full, preventing the download of new image layers.
    C) The `imagePullSecrets` provided are incorrect or missing for a private registry.
    D) The container's `command` or `args` are invalid.
    E) The registry is experiencing a rate limit (e.g., Docker Hub limits).
    F) The pod's CNI plugin is not functioning, preventing network access to the registry.
    
    **Correct Answers: A, B, C, E, F**
    **Explanation:** `ImagePullBackOff` is strictly related to the inability to successfully pull the image. This can be due to non-existent images, auth failures, disk space issues on the node, registry throttling, or network issues (CNI failure). If `command` or `args` are invalid, the pod will pull the image but then fail with `CrashLoopBackOff` or `RunContainerError`.

17. When implementing "NetworkPolicies", which of the following statements are true regarding their behavior?
    A) By default, all traffic is allowed to and from pods if no policy exists.
    B) Policies are additive; if multiple policies apply to a pod, the union of allowed traffic is used.
    C) NetworkPolicies are enforced by the `kube-apiserver`.
    D) An empty `ingress: {}` rule allows all incoming traffic.
    E) A policy with an empty `podSelector: {}` applies to all pods in the namespace.
    F) NetworkPolicies can filter traffic based on DNS names (FQDNs).
    
    **Correct Answers: A, B, E**
    **Explanation:** Kubernetes is "allow-all" by default. Policies are additive (OR logic). An empty `podSelector` targets every pod in that namespace. Policies are enforced by the CNI plugin (e.g., Calico, Cilium), not the API server. An empty `ingress` block (no rules) actually denies all traffic; to allow all, you need a rule with an empty selector. Standard NetworkPolicies do not support FQDNs; that is a feature of specific CNI implementations or Service Meshes.

18. What is the "Hairpin NAT" (or promiscuous bridge) mode in Kubernetes networking used for?
    A) To allow a pod to communicate with itself via its Service's ClusterIP.
    B) To allow pods to reach the external internet without a gateway.
    C) To enable communication between pods in different VPCs.
    D) To bypass the CNI plugin for performance reasons.
    E) To resolve issues where a pod's request to its own Service IP is dropped because the source and destination are the same.
    F) To enable load balancing for UDP traffic.
    
    **Correct Answers: A, E**
    **Explanation:** Without Hairpin NAT, if a pod sends traffic to a Service IP that happens to load balance back to the same pod, the packet might be dropped because the bridge sees the same source and destination MAC/IP. Hairpin NAT allows the packet to "turn around" and come back in.

19. Which headers or fields are manipulated by an Ingress Controller to preserve the client's original IP address?
    A) `X-Forwarded-For`
    B) `X-Real-IP`
    C) `Proxy-Protocol`
    D) `Host`
    E) `X-Original-Source`
    F) `Via`
    
    **Correct Answers: A, B, C**
    **Explanation:** Standard HTTP proxies use `X-Forwarded-For` and `X-Real-IP` to pass the client IP. For TCP/Layer 4 level preservation, `Proxy-Protocol` is used (often by cloud load balancers). `Host` and `Via` are standard headers but aren't used for source IP preservation.

20. In the context of Kubernetes Services, what is the effect of setting `externalTrafficPolicy: Local`?
    A) It forces the traffic to stay within the local cluster network.
    B) It preserves the client's source IP address by avoiding SNAT during node-to-node routing.
    C) It limits the Service to only load balance to pods on the node that received the traffic.
    D) It increases the risk of uneven load distribution if pods are not spread evenly across nodes.
    E) It automatically creates a local DNS record for the Service.
    F) It disables health checks for the Service.
    
    **Correct Answers: B, C, D**
    **Explanation:** `externalTrafficPolicy: Local` tells the node to only send traffic to local pods. This avoids the extra hop to another node, which in turn avoids the need for SNAT to ensure the return path. This preserves the client IP. However, if Node A has 1 pod and Node B has 10 pods, Node A will still receive ~50% of the traffic from an external LB, leading to an imbalance.

21. How does the Kubernetes `kube-scheduler` use "Node Affinity" and "Pod Affinity" differently?
    A) Node Affinity constrains which nodes a pod can be scheduled on based on node labels.
    B) Pod Affinity constrains which nodes a pod can be scheduled on based on labels of pods already running on the node.
    C) Node Affinity only supports "Hard" (required) requirements.
    D) Pod Anti-Affinity is used to ensure pods from the same service are spread across different failure domains.
    E) Both use the `topologyKey` to define the scope (node, rack, zone).
    F) Node Affinity uses the `matchExpressions` field while Pod Affinity uses `labelSelector`.
    
    **Correct Answers: A, B, D, F**
    **Explanation:** Node Affinity is pod-to-node (using node labels). Pod Affinity is pod-to-pod (using pod labels to find nodes). Both support "Hard" (RequiredDuringScheduling...) and "Soft" (PreferredDuringScheduling...) variants. `topologyKey` is specific to Pod Affinity/Anti-Affinity to define the domain (e.g., don't put two of these pods in the same `kubernetes.io/hostname` or `topology.kubernetes.io/zone`). Node Affinity does not use `topologyKey` because it maps directly to nodes.

22. What happens during the "Prioritizing" (Scoring) phase of the kube-scheduler?
    A) Nodes that do not meet the pod's resource requirements are filtered out.
    B) Remaining nodes are ranked based on a set of scoring functions (e.g., LeastRequestedPriority).
    C) The scheduler checks for Taints and Tolerations.
    D) The node with the highest cumulative score is selected for the pod.
    E) The scheduler calculates the "BalancedResourceAllocation" to ensure CPU and Memory usage are even.
    F) The scheduler binds the pod to the selected node in etcd.
    
    **Correct Answers: B, D, E**
    **Explanation:** The scheduler has two main steps: Filtering (Predicates) and Scoring (Priorities). Filtering removes unsuitable nodes (Taints, Resource limits). Scoring ranks the survivors. Functions like LeastRequested (favors empty nodes) and BalancedResource (favors nodes where CPU/Mem usage ratios match) are used. Binding is a separate step that happens after the best node is found.

23. Regarding Kubernetes "Resource Quotas", which statements are correct?
    A) They can limit the total number of resources (Pods, Services, etc.) in a namespace.
    B) They can limit the total sum of compute resources (CPU, Memory) requested in a namespace.
    C) They are enforced at the node level by the kubelet.
    D) If a namespace has a quota, every pod must have explicit resource requests/limits defined (or a LimitRange must exist).
    E) Quotas are only checked during the creation of a resource, not during updates.
    F) Resource Quotas can be applied globally across all namespaces.
    
    **Correct Answers: A, B, D**
    **Explanation:** Quotas are namespace-scoped. They limit total counts or sum of requests/limits. If a CPU quota exists, the API server will reject any pod that doesn't specify how much CPU it needs (unless a LimitRange provides a default). They are enforced by the Admission Controller in the API server. They are checked on updates as well.

24. What are the implications of using "PriorityClass" and Pod Preemption in a crowded cluster?
    A) High-priority pods can evict lower-priority pods to make room for themselves.
    B) Preempted pods follow their standard termination grace period.
    C) The `preemptionPolicy: Never` setting allows a pod to be high priority without evicting others.
    D) Preemption is handled by the `kubelet` on the local node.
    E) High-priority pods are always scheduled first in the queue.
    F) Preemption can trigger a "thrashing" effect if priority levels are not designed carefully.
    
    **Correct Answers: A, B, C, E, F**
    **Explanation:** PriorityClasses define the importance and the preemption behavior. When a high-priority pod cannot be scheduled, the scheduler looks for pods to evict. Preemption is a scheduler-level decision (it clears the `nodeName` or deletes the victim). Victim pods get their grace period. `preemptionPolicy: Never` lets a pod jump the queue without kicking others out. Thrashing (pods constantly evicting each other) is a risk with cyclic dependencies or poorly tuned priorities.

25. How does the "Vertical Pod Autoscaler" (VPA) work in its "Auto" or "Recreate" mode?
    A) It dynamically changes the CPU and Memory limits of a running container without restarting it.
    B) It monitors actual resource usage and updates the pod's `resourceRequests`.
    C) It evicts the pod if the current requests are significantly different from the recommended values.
    D) It uses an Admission Webhook to inject the new resource values when the pod is recreated.
    E) It works seamlessly with the Horizontal Pod Autoscaler (HPA) when both target the same metrics.
    F) It requires the Metrics Server to be running in the cluster.
    
    **Correct Answers: B, C, D, F**
    **Explanation:** VPA (currently) cannot update resources in-place (in-place update is an alpha/beta feature in K8s, but VPA mostly relies on restarts). In Auto mode, VPA evicts the pod. When the Deployment recreates it, the VPA admission webhook patches the new request values. HPA and VPA usually conflict if they both use CPU/Memory metrics (HPA tries to add pods, VPA tries to make them bigger). VPA relies on Metrics Server for usage data.

26. Which of the following are "Built-in" Taints that Kubernetes might automatically apply to nodes?
    A) `node.kubernetes.io/not-ready`
    B) `node.kubernetes.io/unreachable`
    C) `node.kubernetes.io/out-of-disk`
    D) `node.kubernetes.io/memory-pressure`
    E) `node.kubernetes.io/network-unavailable`
    F) `node.kubernetes.io/unschedulable`
    
    **Correct Answers: A, B, D, E, F**
    **Explanation:** The control plane or kubelet applies taints to signal node problems. `not-ready` and `unreachable` are common for node failures. `memory-pressure` and `disk-pressure` (note: `out-of-disk` was deprecated/replaced by `disk-pressure`) signal resource exhaustion. `unschedulable` is used when a node is cordoned.

27. What is the purpose of the "Topology Aware Hints" feature in Kubernetes Services?
    A) To ensure traffic stays within the same zone as the originating pod to reduce latency and cost.
    B) To allow pods to discover the physical rack they are running on.
    C) To provide the `kube-proxy` with information about the cluster's network topology.
    D) To automatically scale pods based on zonal demand.
    E) It is enabled by setting the `service.kubernetes.io/topology-aware-hints` annotation to `Auto`.
    F) It requires the `EndpointSlice` controller to be active.
    
    **Correct Answers: A, C, E, F**
    **Explanation:** Topology Aware Hints (now often referred to as Topology Aware Routing) help keep traffic local to a zone. The EndpointSlice controller adds "hints" to endpoints, and kube-proxy uses these hints to filter which backends it sends traffic to. It's a key feature for multi-zone clusters to save on cross-zone data costs and latency.

28. In the "Cgroup v2" implementation for Kubernetes, what improvements are offered over v1?
    A) Better support for memory pressure handling and the "OOM Killer".
    B) Unified hierarchy for all resource types.
    C) Ability to set "Memory High" (throttling) instead of just "Memory Max" (killing).
    D) Direct support for GPU resource isolation.
    E) Improved CPU isolation for multi-tenant workloads.
    F) Native support for rootless containers.
    
    **Correct Answers: A, B, C, E, F**
    **Explanation:** Cgroup v2 is a significant rewrite. It provides a single tree for all controllers (CPU, Mem, I/O). It introduces "memory.high" which allows the kernel to throttle or reclaim memory from a process before it hits the hard limit (OOM). It's essential for rootless operation and provides much better insights into resource pressure (PSI).

29. Which factors influence the "Quality of Service" (QoS) class assigned to a pod?
    A) The `priorityClassName` assigned to the pod.
    B) Whether `requests` and `limits` are equal for all containers.
    C) The presence of a `PreemptionPolicy`.
    D) Whether any container in the pod has missing `requests` or `limits`.
    E) The total amount of CPU requested compared to the node capacity.
    F) The presence of Init Containers.
    
    **Correct Answers: B, D**
    **Explanation:** QoS classes (Guaranteed, Burstable, BestEffort) are determined solely by the relationship between `requests` and `limits`. Guaranteed: Requests == Limits for every container (including Init). BestEffort: No requests or limits set for any container. Burstable: Everything else. Priority classes and node capacity do not affect the QoS label.

30. What is the function of the "Kubelet Eviction" mechanism compared to the "API-initiated Eviction"?
    A) Kubelet eviction happens when the local node is under resource pressure (Memory, Disk).
    B) API-initiated eviction is triggered by a client (like `kubectl drain`) via the `/eviction` subresource.
    C) Kubelet eviction honors PodDisruptionBudgets (PDBs).
    D) Kubelet eviction is hard and immediate, potentially ignoring grace periods if pressure is extreme.
    E) API-initiated eviction respects PDBs and follows the pod's grace period.
    F) Only API-initiated eviction can trigger a reschedule of the pod.
    
    **Correct Answers: A, B, D, E**
    **Explanation:** Kubelet eviction is a self-preservation mechanism of the node; it does NOT respect PDBs because it needs to save the node from crashing. API-initiated eviction (used by drain) is a "polite" request that respects PDBs and grace periods. Both result in the pod being deleted, and if managed by a controller (Deployment), the controller will try to recreate it elsewhere.

31. Which of the following are components of the Kubernetes "Control Plane Hardening" best practices?
    A) Enabling TLS encryption for all API communication.
    B) Restricting access to the etcd cluster to only the kube-apiserver.
    C) Enabling RBAC with the "AlwaysAllow" authorization mode.
    D) Using "NodeRestriction" admission controller to limit kubelet permissions.
    E) Encrypting secrets at rest in etcd.
    F) Running all control plane components as root for maximum performance.
    
    **Correct Answers: A, B, D, E**
    **Explanation:** Hardening involves TLS everywhere, isolating etcd, and using fine-grained RBAC (AlwaysAllow is insecure). NodeRestriction prevents a compromised node from modifying objects outside its scope. Secret encryption at rest protects data if etcd is accessed directly. Running as root is a security risk, not a hardening measure.

32. What is the purpose and function of "Pod Security Admissions" (PSA)?
    A) It replaces the deprecated PodSecurityPolicies (PSP).
    B) It defines three levels: Privileged, Baseline, and Restricted.
    C) It is configured via labels on namespaces.
    D) It can operate in three modes: Enforce, Audit, and Warn.
    E) It requires a custom operator to be installed.
    F) It allows fine-grained control over specific Linux capabilities for individual pods.
    
    **Correct Answers: A, B, C, D**
    **Explanation:** PSA is the built-in replacement for PSP. It uses predefined profiles (Privileged, Baseline, Restricted) applied at the namespace level via labels. It can block pods (Enforce), log them (Audit), or show a message to the user (Warn). It is not as granular as PSP; for fine-grained control, tools like Kyverno or OPA Gatekeeper are used.

33. How does "Role-Based Access Control" (RBAC) handle "Deny" rules?
    A) RBAC is purely additive; there are no explicit "Deny" rules.
    B) If multiple Roles are bound to a user, a single "Deny" in any of them overrides all "Allows".
    C) Lack of an "Allow" rule is an implicit "Deny".
    D) "Deny" rules can be added using a `ClusterRoleBinding`.
    E) Admission webhooks must be used if explicit "Deny" logic is required.
    F) RBAC checks the `Verb`, `APIGroup`, and `Resource` fields.
    
    **Correct Answers: A, C, E, F**
    **Explanation:** Kubernetes RBAC is "Whitelist only". You only grant permissions; you cannot explicitly take them away with a "Deny" rule. If you aren't granted a permission, you don't have it. To implement complex "Deny" logic (e.g., allow everything except deleting this one specific pod), you must use an Admission Controller/Webhook.

34. Which statements are true regarding "Secret" management in Kubernetes?
    A) By default, Secrets are stored as base64 encoded plaintext in etcd.
    B) Secrets are automatically encrypted by the kubelet before being written to the node's disk.
    C) Using `tmpfs` for Secret volumes ensures they are never written to the node's non-volatile storage.
    D) The size of a Secret is limited to 1MB.
    E) `Immutable` Secrets can improve performance by reducing the number of Watches the kubelet needs to maintain.
    F) Secrets are more secure than ConfigMaps because they use a different encryption algorithm in transit.
    
    **Correct Answers: A, C, D, E**
    **Explanation:** Secrets are base64 encoded, which is NOT encryption. They are limited to 1MB (etcd limit). `tmpfs` is used to keep them in memory on the node. `Immutable` secrets (introduced in 1.21) tell the kubelet it doesn't need to watch for changes, saving resources. Both Secrets and ConfigMaps use the same TLS protection in transit.

35. In a multi-cluster setup using "Cluster API" (CAPI), what is the role of the "Management Cluster"?
    A) It hosts the controllers that manage the lifecycle of "Workload Clusters".
    B) It provides a unified API for deploying applications across all clusters.
    C) It stores the "Machine" and "Cluster" custom resources.
    D) It acts as a global load balancer for all workload clusters.
    E) It handles the provisioning of infrastructure (VMs, LoadBalancers) in the cloud provider.
    F) It must be the same version as the workload clusters it manages.
    
    **Correct Answers: A, C, E**
    **Explanation:** CAPI uses a Management Cluster to treat clusters as Kubernetes resources. It runs controllers that talk to cloud APIs (AWS, Azure, etc.) to spin up infrastructure and bootstrap workload clusters. It doesn't necessarily provide a global application API (that's more of a Federation/Fleet management task). It can manage clusters of different versions.

36. What are the common symptoms of "Etcd Fragmentation" and how is it addressed?
    A) Increased disk usage even after many keys are deleted.
    B) Slower write latency due to internal search overhead.
    C) Increased memory usage by the etcd process.
    D) Frequent "leader election" events.
    E) It is addressed by running the `etcdctl defrag` command.
    F) It is addressed by increasing the `quota-backend-bytes` limit.
    
    **Correct Answers: A, B, E**
    **Explanation:** etcd uses an append-only B-tree. Deleting keys doesn't shrink the file; it leaves "holes" (fragmentation). This leads to wasted space and slower performance. `defrag` is the command to reclaim that space. Increasing the quota is a temporary fix for space issues but doesn't solve fragmentation.

37. Which metrics are most critical to monitor for the "Kube-apiserver" health?
    A) `apiserver_request_duration_seconds`: To identify slow API calls.
    B) `apiserver_request_total`: To see the volume of traffic and error codes (4xx/5xx).
    C) `apiserver_current_inflight_requests`: To monitor saturation and potential throttling.
    D) `process_cpu_seconds_total`: To check CPU usage.
    E) `workqueue_depth`: To see if the internal controllers are falling behind.
    F) `etcd_db_total_size_in_bytes`: To monitor the underlying storage health.
    
    **Correct Answers: A, B, C, F**
    **Explanation:** Latency (duration), Error rates (total/code), and Saturation (inflight) are the Golden Signals for the API server. Since it depends heavily on etcd, monitoring the etcd DB size is also critical. `workqueue_depth` is more relevant for the controller-manager or custom operators.

38. When troubleshooting a "Pending" pod that has a "FailedScheduling" event with "0/N nodes are available: N node(s) had taint {key: value}, that the pod didn't tolerate", what steps should be taken?
    A) Add a matching `toleration` to the pod's specification.
    B) Remove the `taint` from the node if it's no longer applicable.
    C) Check if the pod has a `nodeSelector` that conflicts with the node's labels.
    D) Verify if the pod's `affinity` rules are too restrictive.
    E) Increase the resource requests of the pod.
    F) Check if the `kube-scheduler` pod is running correctly.
    
    **Correct Answers: A, B**
    **Explanation:** The error message explicitly identifies a Taint/Toleration mismatch. The fix is either to make the pod tolerate the taint or remove the taint from the node. While other issues like nodeSelector or resources could cause a pod to be Pending, the specific event message in the question points only to taints.

39. What are "Graceful Node Shutdown" and "Non-Graceful Node Shutdown" in Kubernetes 1.20+?
    A) Graceful shutdown allows the kubelet to detect host shutdown and terminate pods cleanly.
    B) Non-graceful shutdown allows a cluster admin to manually trigger pod eviction when a node is lost.
    C) Graceful shutdown requires the `ShutdownGracePeriod` feature gate.
    D) Non-graceful shutdown automatically migrates stateful volumes to other nodes without risk of corruption.
    E) Graceful shutdown uses systemd inhibition locks to delay the host power-off.
    F) Both require the `NodeLease` feature to be enabled.
    
    **Correct Answers: A, B, C, E**
    **Explanation:** Graceful shutdown (Kubelet-led) lets pods clean up before the OS kills them. It uses systemd/logind integration. Non-graceful shutdown (Admin-led) is a way to tell the cluster "this node is gone, don't wait for it to come back" so that Volume attachments (like EBS/AzureDisk) can be moved to other nodes immediately. Without it, stateful pods might stay stuck in "Terminating" for a long time.

40. Which features are provided by "EndpointSlices" that the original "Endpoints" resource lacked?
    A) Scalability: Ability to handle thousands of endpoints without overloading the API server.
    B) Support for multiple network families (IPv4 and IPv6) in a single resource.
    C) Ability to store custom metadata for each individual endpoint.
    D) Integration with `kube-proxy` for more efficient rule updates.
    E) Support for "Headless" services.
    F) Automatic grouping of endpoints by zone for topology-aware routing.
    
    **Correct Answers: A, B, D, F**
    **Explanation:** The original Endpoints resource was a single object containing every IP for a Service. For large services, this object became massive, causing API performance issues. EndpointSlices break this into multiple smaller objects. They also natively support dual-stack (IPv4/v6) and provide the metadata (like zone) needed for topology-aware routing. Headless services were supported by the original Endpoints too.
