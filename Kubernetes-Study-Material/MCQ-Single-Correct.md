# Kubernetes Easy-Level Multiple Choice Questions

1. What is the primary role of Kubernetes in a containerized environment?
   A) Building container images
   B) Managing and orchestrating containers
   C) Storing source code
   D) Running virtual machines

   **Correct Answer: B**
   **Explanation:** Kubernetes is a container orchestration platform that automates the deployment, scaling, and management of containerized applications.

2. Which component is known as the "brain" of a Kubernetes cluster?
   A) Kubelet
   B) Kube-proxy
   C) Control Plane
   D) Container Runtime

   **Correct Answer: C**
   **Explanation:** The Control Plane manages the state of the cluster, makes decisions about scheduling, and responds to cluster events.

3. What is the smallest deployable unit in Kubernetes?
   A) Container
   B) Pod
   C) Service
   D) Node

   **Correct Answer: B**
   **Explanation:** A Pod is the smallest and simplest unit in the Kubernetes object model that you create or deploy.

4. Which command is used to list all pods in the current namespace?
   A) kubectl get pods
   B) kubectl show pods
   C) kubectl list pods
   ) kubectl describe pods

   **Correct Answer: A**
   **Explanation:** The 'get' command is the standard way to retrieve a list of resources in Kubernetes.

5. What does the 'Kubelet' do on a worker node?
   A) It schedules pods to nodes
   B) It ensures containers are running in a pod
   C) It provides a web UI for the cluster
   D) It manages the cluster's network rules

   **Correct Answer: B**
   **Explanation:** The Kubelet is an agent that runs on each node in the cluster and makes sure that containers are running in a Pod as expected.

6. Which Kubernetes component stores all cluster data?
   A) Kube-apiserver
   B) Kube-scheduler
   C) etcd
   D) Cloud-controller-manager

   **Correct Answer: C**
   **Explanation:** etcd is a consistent and highly-available key-value store used as Kubernetes' backing store for all cluster data.

7. How do you apply a configuration change defined in a YAML file?
   A) kubectl run -f file.yaml
   B) kubectl create -f file.yaml
   C) kubectl apply -f file.yaml
   D) kubectl set -f file.yaml

   **Correct Answer: C**
   **Explanation:** The 'apply' command manages applications through files and is the recommended way to create or update resources.

8. What is a Kubernetes Node?
   A) A physical or virtual machine in a cluster
   B) A group of containers
   C) A networking rule
   D) A storage volume

   **Correct Answer: A**
   **Explanation:** A node is a worker machine in Kubernetes and may be either a virtual or a physical machine, depending on the cluster.

9. Which object is used to expose a Pod or set of Pods to the network?
   A) Deployment
   B) ReplicaSet
   C) Service
   D) ConfigMap

   **Correct Answer: C**
   **Explanation:** A Service is an abstract way to expose an application running on a set of Pods as a network service.

10. What is the purpose of a ReplicaSet?
    A) To store sensitive data
    B) To ensure a specified number of pod replicas are running
    C) To provide persistent storage
    D) To balance network traffic

    **Correct Answer: B**
    **Explanation:** A ReplicaSet's purpose is to maintain a stable set of replica Pods running at any given time.

11. Which kubectl command shows detailed information about a specific resource?
    A) kubectl get
    B) kubectl logs
    C) kubectl describe
    D) kubectl explain

    **Correct Answer: C**
    **Explanation:** The 'describe' command provides a detailed summary of a resource, including events and status.

12. In which file format are Kubernetes resource definitions usually written?
    A) JSON only
    B) XML
    C) YAML
    D) HTML

    **Correct Answer: C**
    **Explanation:** While Kubernetes supports JSON, YAML is the most common format used for defining resources due to its readability.

13. What is a Namespace in Kubernetes used for?
    A) Storing passwords
    B) Isolating groups of resources within a single cluster
    C) Connecting different clusters together
    D) Scaling the number of nodes

    **Correct Answer: B**
    **Explanation:** Namespaces provide a mechanism for isolating groups of resources within a single cluster.

14. Which command shows the logs of a specific pod?
    A) kubectl view logs [pod-name]
    B) kubectl get logs [pod-name]
    C) kubectl logs [pod-name]
    D) kubectl describe logs [pod-name]

    **Correct Answer: C**
    **Explanation:** 'kubectl logs' is the direct command used to retrieve logs from a container in a pod.

15. What does 'Desired State' mean in Kubernetes?
    A) The current status of the hardware
    B) The configuration you want the cluster to maintain
    C) The history of all previous deployments
    D) The speed of the network connection

    **Correct Answer: B**
    **Explanation:** Desired state is the configuration (number of replicas, image version, etc.) that you tell Kubernetes you want to run.

16. Which component is responsible for distributing work to nodes?
    A) Kube-proxy
    B) Kube-scheduler
    C) Kube-apiserver
    D) Container Runtime

    **Correct Answer: B**
    **Explanation:** The scheduler watches for newly created Pods that have no Node assigned and selects a Node for them to run on.

17. What is the default namespace if one is not specified?
    A) kube-system
    B) kube-public
    C) default
    D) main

    **Correct Answer: C**
    **Explanation:** If you do not specify a namespace when creating or looking for a resource, Kubernetes uses the 'default' namespace.

18. Which object provides declarative updates for Pods and ReplicaSets?
    A) Service
    B) Job
    C) Deployment
    D) Secret

    **Correct Answer: C**
    **Explanation:** A Deployment provides declarative updates for Pods and ReplicaSets, allowing you to describe a desired state.

19. How do you delete a pod named 'my-pod'?
    A) kubectl remove pod my-pod
    B) kubectl delete pod my-pod
    C) kubectl stop pod my-pod
    D) kubectl kill pod my-pod

    **Correct Answer: B**
    **Explanation:** The 'delete' command is used to remove resources from the cluster.

20. What is a 'sidecar' container?
    A) The main container in a pod
    B) A container that runs in a separate pod to help another
    C) A second container in the same pod that assists the primary container
    D) A container used only for testing

    **Correct Answer: C**
    **Explanation:** A sidecar is a design pattern where a second container is added to a pod to provide supporting features like logging or proxying.

21. Which component handles network communication between services?
    A) Kube-scheduler
    B) Kube-proxy
    C) etcd
    D) Kube-controller-manager

    **Correct Answer: B**
    **Explanation:** Kube-proxy is a network proxy that runs on each node and maintains network rules to allow communication to your Pods.

22. What command allows you to see the version of kubectl and the server?
    A) kubectl status
    B) kubectl info
    C) kubectl version
    D) kubectl check

    **Correct Answer: C**
    **Explanation:** 'kubectl version' displays the client and server versions of Kubernetes.

23. Which resource is best for storing sensitive information like passwords?
    A) ConfigMap
    B) Pod
    C) Secret
    D) Service

    **Correct Answer: C**
    **Explanation:** Kubernetes Secrets are specifically designed to hold sensitive information such as passwords, OAuth tokens, and ssh keys.

24. What is a 'Cluster'?
    A) A single container
    B) A set of node machines for running containerized applications
    C) A single YAML file
    D) A database of pod names

    **Correct Answer: B**
    **Explanation:** A Kubernetes cluster consists of a set of worker machines, called nodes, that run containerized applications.

25. How can you change the number of replicas in a deployment?
    A) Use the kubectl scale command
    B) Delete and recreate the pod
    C) Restart the Kubelet
    D) Change the node's memory

    **Correct Answer: A**
    **Explanation:** The 'kubectl scale' command allows you to immediately scale the number of replicas for a deployment, replicaset, or statefulset.

26. What does the API Server do?
    A) It stores the cluster's data
    B) It serves as the front end for the Kubernetes control plane
    C) It runs the containers
    D) It manages the physical hardware

    **Correct Answer: B**
    **Explanation:** The API server is the primary management interface for Kubernetes; all internal and external communication goes through it.

27. What is a 'Label' in Kubernetes?
    A) A unique ID for every pod
    B) A key-value pair used to identify and organize resources
    C) A command to start a container
    D) A type of service

    **Correct Answer: B**
    **Explanation:** Labels are key-value pairs that are attached to objects, such as pods, and are used to specify identifying attributes of objects.

28. Which command is used to enter a running container's shell?
    A) kubectl enter [pod-name]
    B) kubectl exec -it [pod-name] -- /bin/bash
    C) kubectl connect [pod-name]
    D) kubectl run [pod-name] -shell

    **Correct Answer: B**
    **Explanation:** The 'exec' command allows you to execute a command in a container, and '-it' provides an interactive terminal session.

29. What is a 'ConfigMap' used for?
    A) Storing non-confidential configuration data
    B) Encrypting passwords
    C) Managing network traffic
    D) Scheduling pods

    **Correct Answer: A**
    **Explanation:** A ConfigMap is an API object used to store non-confidential data in key-value pairs, which pods can consume as environment variables or configuration files.

30. Which Kubernetes component runs the controllers?
    A) Kube-apiserver
    B) Kube-controller-manager
    C) Kube-scheduler
    D) etcd

    **Correct Answer: B**
    **Explanation:** The Kube-controller-manager is a control plane component that runs controller processes, such as the node controller or job controller.
1. What happens when a Deployment's replica count is increased from 3 to 5?
   A) Two new Pods are created immediately with the same specification as the existing ones.
   B) The existing Pods are deleted and 5 new Pods are created.
   C) A new ReplicaSet is created to manage the additional 2 Pods.
   D) The Deployment waits for the current Pods to restart before adding new ones.

   **Correct Answer: A**
   **Explanation:** Increasing the replicas in a Deployment updates the underlying ReplicaSet, which then creates the necessary number of new Pods to reach the desired state.

2. Which service type is most appropriate for exposing a set of Pods to external traffic via a cloud provider's load balancer?
   A) ClusterIP
   B) NodePort
   C) LoadBalancer
   D) ExternalName

   **Correct Answer: C**
   **Explanation:** The LoadBalancer service type integrates with cloud providers to provision an external load balancer that routes traffic to the Service.

3. How does a ConfigMap differ from a Secret in Kubernetes?
   A) ConfigMaps are stored in etcd, while Secrets are stored in a separate database.
   B) Secrets are base64 encoded by default, while ConfigMaps are stored as plain text.
   C) ConfigMaps can be mounted as volumes, but Secrets cannot.
   D) There is no functional difference; they are interchangeable.

   **Correct Answer: B**
   **Explanation:** While both store configuration data, Secrets are intended for sensitive information and are base64 encoded, whereas ConfigMaps are for non-sensitive data.

4. What is the primary purpose of a Liveness Probe?
   A) To check if a container is ready to start accepting traffic.
   B) To determine if a container needs to be restarted because it is in a broken state.
   C) To verify if the Node has enough resources to run the Pod.
   D) To measure the latency of requests handled by the application.

   **Correct Answer: B**
   **Explanation:** Liveness probes help the kubelet know when to restart a container. If a liveness probe fails, the kubelet kills the container and subjects it to its restart policy.

5. In a RollingUpdate strategy for a Deployment, what does 'maxUnavailable' define?
   A) The maximum number of Pods that can be created above the desired replica count.
   B) The total number of Pods that are allowed to fail during the update.
   C) The maximum number of Pods that can be unavailable during the update process.
   D) The time limit for how long a Pod can be in a pending state.

   **Correct Answer: C**
   **Explanation:** 'maxUnavailable' is an optional field that specifies the maximum number of Pods that can be unavailable during the update process, ensuring a minimum level of availability.

6. Which field in a Pod specification is used to ensure that a Pod only runs on nodes with specific hardware like GPUs?
   A) nodeSelector
   B) nodeRestriction
   C) affinity.podAffinity
   D) tolerations

   **Correct Answer: A**
   **Explanation:** 'nodeSelector' is the simplest way to constrain Pods to nodes with particular labels, such as those indicating specific hardware.

7. What is the role of a Headless Service in Kubernetes?
   A) To provide a single stable IP for a set of Pods without a proxy.
   B) To allow direct access to Pod IPs via DNS without load balancing.
   C) To hide the Service name from the internal DNS.
   D) To manage Pods that do not have any containers.

   **Correct Answer: B**
   **Explanation:** A Headless Service (spec.clusterIP: None) does not have a cluster IP. Instead, DNS returns the IP addresses of the individual Pods backing the service.

8. Which volume type is suitable for sharing data between containers within the same Pod that persists only for the lifetime of that Pod?
   A) hostPath
   B) persistentVolumeClaim
   C) emptyDir
   D) nfs

   **Correct Answer: C**
   **Explanation:** 'emptyDir' is created when a Pod is assigned to a Node and exists as long as that Pod is running on that node. It is shared among all containers in the Pod.

9. What does the 'imagePullPolicy: Always' setting guarantee?
   A) The container will always restart if it fails.
   B) The kubelet will always pull the image from the registry before starting the container, even if it exists locally.
   C) The image will be pulled only if the tag is 'latest'.
   D) Kubernetes will automatically update the image when a new version is pushed to the registry.

   **Correct Answer: B**
   **Explanation:** With 'Always', the kubelet queries the container image registry to resolve the name to an image digest. If the digest is different from the local one, it pulls the image.

10. How can you limit the amount of CPU a specific Namespace can consume in total?
    A) ResourceQuota
    B) LimitRange
    |C) PodDisruptionBudget
    D) NetworkPolicy

    **Correct Answer: A**
    **Explanation:** A ResourceQuota provides constraints that limit aggregate resource consumption per Namespace, such as total CPU, memory, or number of objects.

11. What is the effect of setting 'hostNetwork: true' in a Pod spec?
    A) The Pod can access all other Pods in the cluster using their hostnames.
    B) The Pod uses the network namespace of the host node instead of its own isolated network namespace.
    C) The Pod is automatically exposed to the internet via the host's public IP.
    D) The Pod shares the same storage as the host node.

    **Correct Answer: B**
    **Explanation:** When 'hostNetwork' is true, the Pod can see and use the network interfaces of the node it is running on, which is often used for system-level components.

12. Which Kubernetes object is used to manage stateful applications, ensuring stable network identifiers and persistent storage?
    A) Deployment
    B) ReplicaSet
    C) StatefulSet
    D) DaemonSet

    **Correct Answer: C**
    **Explanation:** StatefulSets are designed for applications that require stable identifiers (like web-0, web-1) and stable, persistent storage across restarts.

13. What is the purpose of an Ingress resource?
    A) To manage internal traffic between Pods in different namespaces.
    B) To provide HTTP and HTTPS routes from outside the cluster to services within the cluster.
    C) To act as a firewall for all incoming traffic to the Node.
    D) To encrypt all traffic between Nodes in the cluster.

    **Correct Answer: B**
    **Explanation:** Ingress exposes HTTP and HTTPS routes from outside the cluster to services within the cluster. Traffic routing is controlled by rules defined on the Ingress resource.

14. How does a Readiness Probe affect a Pod's lifecycle?
    A) It determines if the Pod should be terminated.
    B) It decides whether the Pod's IP should be added to the Endpoints of its associated Service.
    C) It triggers a restart of the container if it fails multiple times.
    D) It controls the priority of the Pod during scheduling.

    **Correct Answer: B**
    **Explanation:** If a Readiness Probe fails, the Pod is removed from the Endpoints of all Services that match its labels, stopping traffic from being sent to it.

15. What is the difference between a ClusterRole and a Role in RBAC?
    A) Roles are cluster-wide, while ClusterRoles are namespace-specific.
    B) Roles apply to users, while ClusterRoles apply to service accounts.
    C) Roles are namespace-specific, while ClusterRoles are cluster-wide.
    D) There is no difference; they are used for the same purpose.

    **Correct Answer: C**
    **Explanation:** A Role can only be used to grant access to resources within a single namespace. A ClusterRole is a non-namespaced resource and can grant access to cluster-scoped resources or resources across all namespaces.

16. Which of the following is true about a PersistentVolume (PV)?
    A) It is a request for storage by a user.
    B) It is a storage resource in the cluster that exists independently of any individual Pod.
    C) It is automatically deleted when the Pod using it is deleted.
    D) It can only be used by one Pod at a time regardless of access modes.

    **Correct Answer: B**
    **Explanation:** A PersistentVolume is a piece of storage in the cluster that has been provisioned by an administrator or dynamically provisioned using Storage Classes. It has a lifecycle independent of any Pod that uses it.

17. What happens if a Pod exceeds its memory 'limit'?
    A) The Pod is throttled and its performance decreases.
    B) The Pod is evicted from the node immediately.
    C) The container is terminated with an Out of Memory (OOM) error.
    D) Kubernetes automatically increases the memory limit for that Pod.

    **Correct Answer: C**
    **Explanation:** When a container reaches its memory limit, the Linux kernel's OOM killer usually terminates the process, leading to a container restart if the restart policy allows.

18. What is the primary function of the kube-proxy component?
    A) To schedule Pods onto available Nodes.
    |B) To maintain network rules on nodes and allow network communication to Pods from inside or outside the cluster.
    C) To manage the lifecycle of containers on a Node.
    D) To provide a consistent API for users to interact with the cluster.

    **Correct Answer: B**
    **Explanation:** kube-proxy is a network proxy that runs on each node in the cluster and implements part of the Kubernetes Service concept, handling request forwarding.

19. Which label-based mechanism allows you to group Pods together for Service discovery or ReplicaSet management?
    A) Annotations
    B) Selectors
    C) Namespaces
    D) Taints

    **Correct Answer: B**
    **Explanation:** Selectors are used by Services and ReplicaSets to identify a set of Pods based on their labels.

20. When using a 'Recreate' strategy for a Deployment, what sequence of events occurs during an update?
    A) New Pods are created, and then old Pods are deleted.
    B) All existing Pods are killed before new ones are created.
    C) One old Pod is deleted, followed by the creation of one new Pod, until the update is complete.
    D) The Deployment pauses and waits for manual intervention to delete old Pods.

    **Correct Answer: B**
    **Explanation:** The Recreate strategy kills all existing Pods before starting the new version, resulting in downtime but ensuring no two versions run simultaneously.

21. What is the purpose of Taints and Tolerations?
    A) To ensure Pods are scheduled on nodes with specific labels.
    B) To allow a node to repel a set of Pods unless those Pods have a matching toleration.
    C) To encrypt communication between Pods and the API server.
    D) To define the resource limits for a specific Node.

    **Correct Answer: B**
    **Explanation:** Taints are applied to nodes to mark them as "restricted," and only Pods with matching tolerations are allowed to be scheduled on those nodes.

22. Which command is used to view the detailed status and events of a specific Pod?
    A) kubectl get pods
    B) kubectl log pod
    C) kubectl describe pod
    D) kubectl status pod

    **Correct Answer: C**
    **Explanation:** 'kubectl describe' provides detailed information about a resource, including its configuration, current status, and a list of recent events associated with it.

23. What does the 'Pending' status of a Pod typically indicate?
    A) The containers in the Pod have finished successfully.
    B) The Pod has been accepted by the cluster, but one or more containers are not yet running.
    C) The Pod has failed to start due to a configuration error.
    D) The Pod is being deleted from the cluster.

    **Correct Answer: B**
    **Explanation:** A Pod is in the 'Pending' state when it has been created but hasn't been scheduled yet, or it is in the process of pulling images.

24. How do you inject a specific key-value pair from a ConfigMap as an environment variable in a container?
    A) Use the 'envFrom' field with the ConfigMap name.
    B) Use the 'valueFrom' field with a 'configMapKeyRef'.
    C) Use the 'configData' field in the container spec.
    D) Environment variables cannot be injected from ConfigMaps.

    **Correct Answer: B**
    **Explanation:** The 'valueFrom' field combined with 'configMapKeyRef' allows you to select a specific key from a ConfigMap to be used as the value for an environment variable.

25. What is the significance of the 'terminationGracePeriodSeconds' field in a Pod spec?
    A) It defines the time Kubernetes waits for a Pod to become ready.
    B) It specifies the duration the kubelet waits before forcibly killing a container after sending a termination signal.
    C) It sets the timeout for a liveness probe.
    D) It determines how long a Pod remains in the 'Terminating' state after it has already died.

    **Correct Answer: B**
    **Explanation:** When a Pod is deleted, Kubernetes sends a SIGTERM signal to the processes. 'terminationGracePeriodSeconds' is the time it waits for the process to exit gracefully before sending a SIGKILL.

26. Which component is responsible for maintaining the desired state of the cluster by watching the current state and making changes?
    A) kube-apiserver
    B) etcd
    C) kube-controller-manager
    D) kube-scheduler

    **Correct Answer: C**
    **Explanation:** The controller manager runs various controller processes (like replication controller, endpoint controller) that continuously work to bring the current state closer to the desired state.

27. What is a 'Sidecar' container pattern?
    A) A main container that runs multiple processes.
    B) A helper container that runs in the same Pod as the main application container to extend its functionality.
    C) A container that runs on every node in the cluster.
    D) A container that only runs during the initialization phase of a Pod.

    **Correct Answer: B**
    **Explanation:** A Sidecar is a container that runs alongside the main application container in the same Pod, sharing the same network and storage to provide auxiliary features like logging or proxying.

28. In a NetworkPolicy, what does an 'egress' rule control?
    A) Incoming traffic to the Pods.
    B) Outgoing traffic from the Pods.
    C) Traffic between containers in the same Pod.
    D) Traffic between the API server and the Nodes.

    **Correct Answer: B**
    **Explanation:** 'egress' rules in a NetworkPolicy define what outgoing traffic is allowed from the Pods that match the policy's selector.

29. What is the purpose of 'imagePullSecrets' in a Pod specification?
    A) To store passwords for the application running inside the container.
    B) To provide credentials for the kubelet to authenticate with a private container registry.
    C) To encrypt the container image while it is at rest.
    D) To define which users are allowed to pull images from the cluster.

    **Correct Answer: B**
    **Explanation:** 'imagePullSecrets' is a list of local Secret names in the same namespace that contain the credentials needed to pull images from a private registry.

30. Which Kubernetes object can be used to run a task to completion exactly once or on a recurring schedule?
    A) Deployment
    B) DaemonSet
    C) Job or CronJob
    D) StatefulSet

    **Correct Answer: C**
    **Explanation:** A Job creates one or more Pods and ensures that a specified number of them successfully terminate. A CronJob manages Jobs that run on a periodic schedule.
# Advanced Kubernetes Multiple-Choice Questions (Hard Level)

1. When using the Kubernetes API, what is the primary purpose of the 'resourceVersion' field during a WATCH operation?
   A) To specify the version of the API schema being used.
   B) To enable optimistic concurrency control for concurrent writes.
   C) To allow the client to resume a stream from a specific point in time.
   D) To determine the expiration time of the cached object in etcd.

   **Correct Answer: C**
   **Explanation:** The resourceVersion is used by the API server to identify the state of a resource at a specific point in time. In a WATCH operation, providing a resourceVersion allows the client to receive all events that occurred after that specific version, ensuring no events are missed during reconnection or restarts.

2. In a cluster with multiple CNI plugins chained together, which component is responsible for invoking the 'ADD' command for each plugin in the correct order?
   A) The kubelet
   B) The container runtime (e.g., containerd)
   C) The CNI bridge plugin
   D) The kube-proxy

   **Correct Answer: B**
   **Explanation:** While the kubelet triggers the pod creation process, it is the container runtime (via CNI library calls) that executes the CNI plugins defined in the configuration. The runtime reads the CNI configuration list and calls each plugin's ADD method sequentially to set up the network interface.

3. Which of the following best describes the 'PreFilter' phase in the Kubernetes Scheduler Framework?
   A) It removes nodes that do not meet the pod's hard constraints.
   B) It pre-calculates information required for the Filter phase to improve efficiency.
   C) It ranks nodes based on resource availability before final selection.
   D) It ensures that the pod's volume claims can be satisfied by the node.

   **Correct Answer: B**
   **Explanation:** The PreFilter phase is used to pre-process or calculate information about the pod or the cluster that multiple Filter plugins might need. This avoids redundant calculations during the Filter phase, where every node is evaluated against the pod.

4. When a Custom Resource Definition (CRD) is deleted, what happens to the existing Custom Resources (CRs) of that type?
   A) They remain in the cluster but become unmanaged.
   B) They are automatically deleted by the garbage collector.
   C) They are converted into ConfigMaps to preserve their data.
   D) The deletion of the CRD is blocked until all CRs are manually removed.

   **Correct Answer: B**
   **Explanation:** Deleting a CRD triggers the asynchronous deletion of all Custom Resources associated with that definition. The Kubernetes API server handles this cleanup automatically to ensure no orphaned resources remain without a schema.

5. What is the technical function of the 'BoundServiceAccountTokenVolume' feature gate in Kubernetes security?
   A) It encrypts ServiceAccount tokens at rest in etcd.
   B) It ensures ServiceAccount tokens are unique per pod and have a limited lifetime.
   C) It prevents pods from accessing the API server without a valid certificate.
   D) It maps ServiceAccounts to specific OIDC providers outside the cluster.

   **Correct Answer: B**
   **Explanation:** This feature (now GA) improves security by using the TokenRequest API to provide pods with tokens that are time-bound, audience-bound, and tied to the specific pod's identity. If the pod is deleted, the token becomes invalid, unlike the older permanent secret-based tokens.

6. Which etcd mechanism does Kubernetes rely on to implement the 'Lease' object for node heartbeats?
   A) Multi-version Concurrency Control (MVCC)
   B) Distributed locking via the v3 API
   C) TTL-based keys that automatically expire
   D) Watchable key-value pairs for event notification

   **Correct Answer: C**
   **Explanation:** Kubernetes Node heartbeats use the Lease API, which is built on etcd's ability to attach Time-To-Live (TTL) values to keys. If the kubelet fails to renew the lease within the specified timeframe, the lease expires, signalling to the controller manager that the node may be unhealthy.

7. In the context of the Out-Of-Memory (OOM) Killer, how does the kubelet influence which process is killed first when a node runs out of memory?
   A) By adjusting the oom_score_adj of the container process based on QoS class.
   B) By sending a SIGTERM signal to pods with high memory usage.
   C) By reducing the memory limit of the container dynamically.
   D) By priority-sorting pods in the etcd database.

   **Correct Answer: A**
   **Explanation:** The kubelet assigns an oom_score_adj value to each container's process based on its Quality of Service (QoS) class (Guaranteed, Burstable, BestEffort). Lower values make a process less likely to be killed, while higher values (like those for BestEffort pods) make them the primary targets for the kernel OOM killer.

8. What occurs when the 'ValidatingAdmissionWebhook' returns a 'dryRun' field in its response?
   A) The API server ignores the webhook's decision.
   B) The webhook indicates it only checked the request without side effects.
   C) The API server simulates the admission process without persisting the object.
   D) The webhook requests a re-evaluation after a delay.

   **Correct Answer: B**
   **Explanation:** While 'dryRun' as a query parameter in an API request tells the server not to persist changes, the webhook response can also include information about whether the webhook itself performed any side effects. This is critical for auditing and ensuring that validation-only calls don't trigger external actions.

9. How does the 'topologyKeys' field (deprecated in favor of Topology Aware Hints) affect Service traffic routing?
   A) It forces the load balancer to use round-robin across all zones.
   B) It defines a preference order for directing traffic to endpoints based on node labels.
   C) It encrypts traffic between pods in different regions.
   D) It identifies which pods should be co-located on the same node.

   **Correct Answer: B**
   **Explanation:** TopologyKeys allowed developers to define a list of labels (like hostname or zone) that the proxy should use to filter and prioritize endpoints. This ensures traffic stays local to a node or zone before attempting to cross network boundaries, reducing latency and costs.

10. Which component is responsible for the 'Synchronize' loop that ensures the actual state of a StatefulSet matches the desired state?
    A) Kube-scheduler
    B) Kube-controller-manager
    C) Kube-apiserver
    D) Cloud-controller-manager

    **Correct Answer: B**
    **Explanation:** The Kube-controller-manager runs various controller loops, including the StatefulSet controller. This controller is responsible for managing the deployment and scaling of a set of pods with persistent identities, ensuring that the correct number of pods are running and ordered according to the spec.

11. What is the primary bottleneck when scaling a Kubernetes cluster to 5,000+ nodes regarding etcd?
    A) The disk I/O throughput of the etcd nodes.
    B) The linearizability of read requests across the cluster.
    C) The size of the etcd database reaching the default 2GB quota.
    D) The number of concurrent gRPC connections from kube-proxies.

    **Correct Answer: C**
    **Explanation:** etcd has a default database size quota (usually 2GB). In very large clusters, the volume of metadata for tens of thousands of pods, secrets, and configmaps can exceed this limit, causing etcd to enter a maintenance mode that blocks all writes until the database is compacted and defragmented.

12. In a 'PriorityClass' definition, what does the 'preemptionPolicy: Never' setting achieve?
    A) The pod will never be evicted by other higher-priority pods.
    B) The pod will be scheduled immediately regardless of resource availability.
    C) The pod will not trigger the eviction of lower-priority pods to make room for itself.
    D) The pod will ignore taints on nodes during scheduling.

    **Correct Answer: C**
    **Explanation:** By default, a high-priority pod that cannot be scheduled will preempt (evict) lower-priority pods. Setting 'preemptionPolicy: Never' allows a pod to have a high priority for scheduling order (it goes to the front of the queue) without causing the disruptive eviction of other running pods.

13. Which of the following is a characteristic of a 'MutatingAdmissionWebhook' that differentiates it from a 'ValidatingAdmissionWebhook'?
    A) It can only be used for standard Kubernetes objects, not CRDs.
    B) It is executed before the ValidatingAdmissionWebhook in the admission chain.
    C) It cannot reject a request, only modify it.
    D) It must return a patch in JSONPatch format.

    **Correct Answer: B**
    **Explanation:** Mutating webhooks are called first because their modifications might change the object in a way that requires re-validation. Validating webhooks are called last to ensure that the final version of the object (after all mutations) complies with all policies.

14. How does the 'Secret' encryption-at-rest feature work in a standard Kubernetes control plane?
    A) The kubelet encrypts secrets before sending them to the API server.
    B) The API server uses a configured provider (like KMS or AES-GCM) to encrypt the data before writing to etcd.
    C) etcd natively encrypts all data stored on its local disk using LUKS.
    D) The cloud provider's storage layer handles encryption automatically for the etcd volume.

    **Correct Answer: B**
    **Explanation:** Encryption at rest is a feature of the kube-apiserver. When enabled, the API server passes the raw data through an encryption provider (such as a KMS plugin or a local key) before the value is sent to etcd. When reading, it decrypts the value before returning it to the client.

15. What is the purpose of the 'Finalizers' field in a Kubernetes object's metadata?
    A) To prevent the object from being deleted until specific cleanup logic is performed.
    B) To mark the object as ready for production use.
    C) To indicate that the object is the last version in a series of updates.
    D) To define the order in which containers within a pod should terminate.

    **Correct Answer: A**
    **Explanation:** Finalizers are keys in the metadata that signal to controllers that certain conditions must be met before the object can be fully removed from the API. When a delete request is made, the API server sets a deletionTimestamp but won't remove the record until all strings in the finalizers list are gone.

16. In the Operator pattern, what is the 'Reconciliation Loop'?
    A) A process that synchronizes etcd data across master nodes.
    B) A continuous loop that compares the observed state of a system with the desired state defined in a CR.
    C) A method for upgrading the Kubernetes control plane without downtime.
    D) A security check that verifies the checksum of container images.

    **Correct Answer: B**
    **Explanation:** The heart of any operator or controller is the reconciliation loop. It constantly watches for changes to its target resources and takes actions (like creating pods or updating config) to ensure the actual state in the cluster matches the desired state specified by the user in the Custom Resource.

17. Which Linux kernel feature does the 'User Namespaces' support in Kubernetes (alpha/beta) primarily leverage?
    A) cgroups v2
    B) seccomp profiles
    C) Mapping container UIDs/GIDs to different host UIDs/GIDs.
    D) AppArmor mandatory access control.

    **Correct Answer: C**
    **Explanation:** User namespaces allow a process inside a container to run as 'root' (UID 0) while being mapped to a non-privileged user on the host. This provides a significant layer of security, as a container breakout would not result in root access to the underlying node.

18. What is the 'Aggregated API Server' used for in Kubernetes?
    A) To combine multiple clusters into a single management pane.
    B) To extend the Kubernetes API with custom resources that require high-performance logic not possible with CRDs.
    C) To cache API requests and reduce the load on the primary etcd instance.
    D) To provide a unified interface for logging and monitoring data.

    **Correct Answer: B**
    **Explanation:** While CRDs are the standard way to extend the API, Aggregated API Servers allow developers to write their own API server (often using the library-go) to handle specific resource types. This is useful for complex logic, custom storage backends, or sub-resources that CRDs don't support well (e.g., the metrics-server).

19. In a network policy, what happens if a pod matches multiple policies that overlap?
    A) Only the policy with the highest priority is applied.
    B) The policies are combined using a logical AND (all must allow).
    C) The policies are combined using a logical OR (any one can allow).
    D) The pod is isolated until the conflict is resolved manually.

    **Correct Answer: C**
    **Explanation:** Network policies in Kubernetes are additive. If multiple policies apply to a pod, the resulting allow-list is the union of all rules. If any single policy allows the traffic, the traffic is permitted. If no policies allow the traffic, it is denied by default (if ingress/egress is selected).

20. What does the 'PodDisruptionBudget' (PDB) protect against?
    A) Hardware failures of the underlying physical nodes.
    B) Intentional disruptions caused by cluster administrators (e.g., node drains).
    C) Malicious attacks targeting the availability of a specific service.
    D) Network partitions between the control plane and the worker nodes.

    **Correct Answer: B**
    **Explanation:** PDBs are designed to handle voluntary disruptions, such as when an admin drains a node for maintenance or a deployment is updated. They do not protect against involuntary disruptions like kernel panics, hardware failures, or network outages.

21. When using 'ExternalName' type Services, how is traffic routed?
    A) Via an IPVS load balancer rule on each node.
    B) By the kube-proxy creating an iptables DNAT rule.
    C) By returning a CNAME record from the internal CoreDNS.
    D) Through a dedicated ingress controller acting as a reverse proxy.

    **Correct Answer: C**
    **Explanation:** An ExternalName Service has no selectors and no clusterIP. Instead, when a pod looks up the service's DNS name, CoreDNS returns a CNAME record pointing to the external domain specified in the service definition. No proxying or NAT occurs within the cluster.

22. What is the significance of the 'generation' field in the metadata of a Kubernetes object?
    A) It tracks how many times the status of the object has changed.
    B) It is incremented by the API server every time the spec of the object is modified.
    C) It identifies the version of the controller that created the resource.
    D) It represents the number of pods currently managed by a controller.

    **Correct Answer: B**
    **Explanation:** The metadata.generation field is a sequence number that the API server increments whenever the 'spec' (the desired state) of an object is changed. Controllers often compare the generation with a 'observedGeneration' in the status to see if the latest changes have been processed.

23. Which of the following is true about 'OwnerReferences' in Kubernetes?
    A) They are used to grant permissions to users via RBAC.
    B) They allow a child object to be automatically deleted when its parent is deleted.
    C) They prevent a resource from being moved between namespaces.
    D) They define the primary key for resources stored in etcd.

    **Correct Answer: B**
    **Explanation:** OwnerReferences are used by the garbage collector. By setting an ownerReference on a resource (like a Pod pointing to a ReplicaSet), Kubernetes knows that if the parent (ReplicaSet) is deleted, the children (Pods) should also be cleaned up.

24. How does 'EmptyDir' storage behave when a container within a pod crashes and restarts?
    A) The data is lost and a new empty directory is created.
    B) The data is preserved and is available to the restarted container.
    C) The data is moved to the host's /tmp directory for debugging.
    D) The data is synchronized to other nodes for high availability.

    **Correct Answer: B**
    **Explanation:** An emptyDir volume is tied to the lifecycle of the Pod, not the individual containers. If a container crashes, the Pod remains on the node, and the emptyDir volume persists. The data is only deleted when the Pod is removed from the node.

25. What is the primary purpose of 'RuntimeClass' in Kubernetes?
    A) To specify the version of the Go compiler used to build the kubelet.
    B) To allow users to select different container runtimes (e.g., runc, gVisor, Kata) for different pods.
    C) To define the resource limits for the container runtime process itself.
    D) To categorize pods based on their execution time (Short-lived vs Long-running).

    **Correct Answer: B**
    **Explanation:** RuntimeClass provides a way to support multiple container runtimes in a single cluster. For example, you might use 'runc' for standard trusted workloads and 'gVisor' or 'Kata' for untrusted workloads that require stronger isolation.

26. In a 'CustomResourceDefinition', what does 'spec.preserveUnknownFields: false' (in structural schemas) ensure?
    A) That the API server will reject any fields in the CR that are not defined in the schema.
    B) That the API server will automatically add missing fields to the CR.
    C) That the API server will encrypt any fields it does not recognize.
    D) That the CRD can be updated without losing data in existing CRs.

    **Correct Answer: A**
    **Explanation:** In a structural schema, setting preserveUnknownFields to false (the default in newer versions) implements strict validation. Any field sent in a request that isn't explicitly defined in the OpenAPI v3 schema will be pruned (removed) by the API server.

27. Which component is responsible for populating the '.status.hostIP' field of a Pod?
    A) The API Server
    B) The Scheduler
    C) The Kubelet
    D) The Cloud Provider

    **Correct Answer: C**
    **Explanation:** The kubelet on the node where the pod is running is responsible for monitoring the pod and reporting its status back to the API server, including the IP address of the host node and the pod's own IP address once the CNI has assigned it.

28. What is the 'SelfSubjectAccessReview' API used for?
    A) To allow an administrator to audit the permissions of all users.
    B) To allow a user or service account to check its own permissions within the cluster.
    C) To automatically rotate ServiceAccount tokens before they expire.
    D) To prevent a user from accessing their own resources if they are under investigation.

    **Correct Answer: B**
    **Explanation:** This API is part of the authorization.k8s.io group. It allows a client to ask the API server "What can I do?". This is useful for UIs (to hide buttons the user can't click) or for CLI tools to verify they have sufficient access before starting a complex operation.

29. How does 'SidecarContainers' (the native feature introduced in 1.29) change pod initialization?
    A) Sidecars start after the main containers are ready.
    B) Sidecars are started sequentially before init containers.
    C) Sidecars are started alongside init containers but remain running during the pod's life.
    D) Sidecars can only be used in Job resources to handle logging.

    **Correct Answer: C**
    **Explanation:** Native sidecars are implemented by adding a 'restartPolicy: Always' to an entry in the initContainers list. These containers start in order with other init containers but do not need to exit before the main containers start, and they are kept running throughout the pod's lifecycle.

30. In 'Dual-stack' networking, how does Kubernetes handle Service ClusterIPs?
    A) It assigns a single IP that works for both IPv4 and IPv6.
    B) It assigns one IPv4 and one IPv6 address to the Service.
    C) It requires a separate Service object for each IP family.
    D) It uses IPv6-to-IPv4 NAT at the cluster boundary.

    **Correct Answer: B**
    **Explanation:** When configured for dual-stack, a Service can have 'ipFamilyPolicy: PreferDualStack' or 'RequireDualStack'. This results in the Service being assigned two ClusterIPs (one from the IPv4 range and one from the IPv6 range), allowing it to handle traffic from both protocol versions.

31. What happens when a 'PriorityClass' has 'globalDefault: true'?
    A) All nodes in the cluster are assigned this priority by default.
    B) Any pod created without a specific priorityClassName will be assigned this priority.
    C) The priority class is synchronized across all clusters in a federation.
    D) Only one PriorityClass in the entire cluster can have this setting.

    **Correct Answer: B**
    **Explanation:** The globalDefault field allows administrators to set a "fallback" priority level. If a pod is submitted without a priority, Kubernetes automatically assigns it the value of the PriorityClass marked as the global default. Only one PriorityClass can be the global default.

32. What is the function of the 'kube-reserved' flag in kubelet configuration?
    A) It sets the amount of memory and CPU reserved for Kubernetes system daemons (like kubelet, container runtime).
    B) It defines the maximum number of pods that can be scheduled on a node.
    C) It reserves resources for 'Guaranteed' QoS pods only.
    D) It limits the burst capacity of pods on the node.

    **Correct Answer: A**
    **Explanation:** To ensure node stability, 'kube-reserved' allows you to set aside resources specifically for the Kubernetes system components. This prevents user pods from consuming all resources and causing the kubelet or container runtime to starve and fail.

33. Which field in a Pod Spec is used to influence the 'Spread' of pods across failure domains without using hard constraints?
    A) podAffinity
    B) podAntiAffinity
    C) topologySpreadConstraints
    D) nodeSelector

    **Correct Answer: C**
    **Explanation:** While podAntiAffinity can be used for spreading, topologySpreadConstraints provides more granular control. It allows you to define how pods should be distributed across topologies (like zones or hosts) and specify a 'maxSkew' to balance the distribution without being as binary as affinity rules.

34. How does the 'HorizontalPodAutoscaler' (HPA) determine when to scale if multiple metrics are provided?
    A) It calculates a recommendation for each metric and chooses the highest one.
    B) It averages the recommendations from all metrics.
    C) It only considers the first metric in the list.
    D) It requires all metrics to exceed their threshold before scaling.

    **Correct Answer: A**
    **Explanation:** When multiple metrics are used in an HPA, the controller calculates the desired replica count for each metric individually. To ensure the application can handle the load from any perspective (CPU, Memory, or custom), it selects the maximum replica count among all calculated recommendations.

35. What is the role of the 'Cloud Controller Manager' (CCM)?
    A) To manage the hardware lifecycle of bare-metal servers.
    B) To decouple Kubernetes core logic from cloud-provider-specific logic (like LoadBalancers and Routes).
    C) To provide a web-based dashboard for managing multiple cloud accounts.
    D) To encrypt all traffic leaving the cluster for the public internet.

    **Correct Answer: B**
    **Explanation:** The CCM allows the Kubernetes project to evolve independently of cloud providers. It contains the logic for creating cloud load balancers, managing node addresses, and setting up routes in the cloud's VPC, which used to be part of the main controller manager.

36. In 'etcd', what is the purpose of 'Compaction'?
    A) To compress the data to save disk space.
    B) To remove old versions of keys and free up space in the multi-version database.
    C) To merge multiple etcd clusters into one.
    D) To encrypt the database using a more efficient algorithm.

    **Correct Answer: B**
    **Explanation:** etcd is a multi-versioned database, meaning it keeps every change to a key as a new version. Compaction is the process of discarding these historical versions. Without regular compaction, the database would grow indefinitely until it hit the size quota, even if the number of active keys is small.

37. Which of the following is a limitation of 'Shared Process Namespace' in a Pod?
    A) Containers can no longer see each other's files.
    B) The 'init' process (PID 1) is no longer unique to each container; instead, it is shared.
    C) Networking is disabled for all containers in the pod.
    D) It requires the containers to be running the same base image.

    **Correct Answer: B**
    **Explanation:** When 'shareProcessNamespace: true' is set, containers in a pod can see and signal each other's processes. However, this means that the container's own process is no longer PID 1 (an init-like process in the pod takes that role). This can break applications that expect to be PID 1 to handle signals correctly.

38. What is the 'Kubernetes Resource Model' (KRM)?
    A) A specific type of high-performance database used by etcd.
    B) A set of conventions for defining resources, including metadata, spec, and status.
    C) A tool for calculating the cost of running pods in the cloud.
    D) A networking protocol for high-speed pod communication.

    **Correct Answer: B**
    **Explanation:** KRM refers to the standardized way Kubernetes handles data. It involves using declarative YAML/JSON files that follow a specific structure (apiVersion, kind, metadata, spec, status) and can be manipulated using the same API patterns (GET, POST, PUT, PATCH, WATCH).

39. In a 'StatefulSet', what does the 'serviceName' field do?
    A) It identifies the LoadBalancer used to access the pods.
    B) It links the StatefulSet to a Headless Service to provide stable DNS names for each pod.
    C) It defines the internal name of the controller managing the set.
    D) It is a label used for billing purposes.

    **Correct Answer: B**
    **Explanation:** The serviceName must match a Headless Service (a service with clusterIP: None). This allows the creation of DNS entries for each pod in the format `pod-name.service-name.namespace.svc.cluster.local`, which is essential for stateful applications like databases that need stable identities.

40. When troubleshooting a 'NodeNotReady' status, which log is most likely to contain information about CNI plugin failures on the node?
    A) The kube-apiserver logs.
    B) The kube-scheduler logs.
    C) The kubelet logs.
    D) The etcd logs.

    **Correct Answer: C**
    **Explanation:** The kubelet is the component on the node that interacts directly with the CNI plugins. If a CNI plugin fails to initialize or cannot assign an IP, the error will be reported in the kubelet's system logs (journalctl -u kubelet). The control plane components generally only see the resulting 'NotReady' status, not the specific networking error details.