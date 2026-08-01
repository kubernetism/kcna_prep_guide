Replica Sets
ReplicaSet is a way to maintain a desired amount of redundant pods (replicas) to provide a guarantee of availability.

The pod field metadata.ownerReferences determines the link from a pod to a ReplicaSet.

It is not recommended to directly create ReplicaSets. Instead, a Deployment can create and manage a ReplicaSet for you.

Horizontal Pod Autoscaler (HPA) can be used to autoscale a ReplicaSet

Reference
ReplicaSet

What is the relationship between the HPA and ReplicaSet in Kubernetes?