Kubernetes Components Overview
Cluster
A logical grouping of all Kubernetes components.
Encompasses control plane and worker nodes.
Namespace
Logical grouping of components within a cluster.
Used to isolate workloads and manage resources efficiently.
Node
A virtual or physical machine hosting workloads.
Control Plane Node: Manages cluster state.
Worker Node: Runs applications and workloads.
Pod
The smallest deployable unit in Kubernetes.
An abstraction over a container.
Each pod runs one or more containers that share resources and networking.
Service
Provides a stable IP and DNS name for a set of pods.
Ensures connectivity even if pods restart.
Can act as a load balancer.
Ingress
Manages HTTP/S routing to services from outside the cluster.
Can include TLS termination.
API Server
Entry point for all K8s commands via kubectl or HTTP API.
Handles communication between components.
Kubelet
Agent running on each node.
Ensures containers are running as defined in Pod specs.
Communicates with API Server.
Kubectl
Command Line Interface (CLI) for managing the cluster.
Sends commands to the API Server.
Cloud Controller Manager
Connects Kubernetes to cloud provider APIs (e.g., AWS, Azure, GCP).
Controller Manager
Watches cluster state and reconciles desired vs. current state.
Manages controllers like Node, Replication, and Endpoint controllers.
Scheduler
Assigns pods to nodes based on available resources and constraints.
Kube Proxy
Maintains network rules on nodes for routing and load balancing of pods.
Network Policy
Acts as a virtual firewall at pod or namespace level.
ConfigMap
Stores non-confidential configuration data in key-value pairs.
Decouples configuration from container images.
Secret
Stores sensitive data (e.g., passwords, tokens, keys).
Base64-encoded but should be encrypted in production.
Volumes
Provides persistent storage for pods.
Can be local or remote (e.g., cloud storage).
StatefulSet
Manages stateful applications requiring stable IDs and storage.
Used for databases or apps needing ordered deployment.
ReplicaSet
Ensures a specified number of pod replicas are running.
Provides high availability and fault tolerance.
Deployment
Defines blueprints for pods.
Automates rolling updates and rollbacks.