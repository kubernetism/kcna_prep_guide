Control Plane and Worker Nodes
Control Plane Node (Formally known as Master Node)

Manages processes like scheduling, restarting nodes, maintaining the overall state of the cluster

API Server – the backbone of communication
Scheduler – determines where to start a pod on worker node
Controller Manager – detect state changes (if pod crashes, restart it)
etcd – A Key/Value Store that stores the state of the cluster
Kubelet – Allows user to interact with the node via KubeCTL
Cloud Control Manager (optional) – Integrates with the cloud provider
Worker Node

Does the work of running your app in pods and containers

Components:

Kubelet
Kube Proxy
Container Runtime
Pods and Containers