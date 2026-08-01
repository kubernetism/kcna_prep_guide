Pods
Pods are the smallest unit in Kubernetes.

Pods abstract away the container layer so you can directly interact with the Kubernetes Layer.

A Pod is intended to run one application in multiple containers

Database Pod, Job Pod, Frontend App Pod, Backend App Pod
You can run multiple apps in a pod but those containers will tightly dependent.
Each Pod gets its own private IP address

Containers will run on different ports
Containers can talk to each other via localhost
Each Pod can have a shared storage volume attached.

All containers will share the same volume
When the last remaining container dies (maybe crashes) in a pod so does the pod

When a replacement pod is created, the pod will have an IP address will be assigned.
IP addresses are Ephemeral, (temporary) for pods, they don’t by default persist.
Get pods and show their IP addresses

kubectl get pod -o wide