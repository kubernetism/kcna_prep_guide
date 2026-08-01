Deployment
A Deployment provides declarative updates for Pods and ReplicaSets.

A Deployment Controller changes the actual state to the desired state at a controlled rate.

The default Deployment Controller can be swapped out for other deployments tools eg:
Argo CD, Flux, Jenkin X…..
A Deployment define the desired state of ReplicaSets and Pods.

A deployment will create and manage a ReplicaSet.

A ReplicaSet will manage replicas of pod.

Reference
Deployments

Kubernetes: Deployment Strategies types, and Argo Rollouts