API Server
The core of the Kubernetes control plane is the API server.

The API server exposes an HTTP API that lets end-users, different parts of your cluster, and external components communicate with one another.

The Kubernetes API lets you query and manipulates the state of API objects in Kubernetes (for example: Pods, Namespaces, ConfigMaps, and Events).

The API server is a component of the Kubernetes control plane that exposes the Kubernetes API. The API server is the front end for the Kubernetes control plane.

The main implementation of a Kubernetes API server is kube-apiserver.

kube-apiserver is designed to scale horizontally—that is, it scales by deploying more instances.

You can run several instances of kube-apiserver and balance traffic between those instances.

Everything has to go through the API Server.

You can interact with the API Server in three ways:

UI
API
CLI KubeCTL



Reference
kube-apiserver - Synopsis
https://kubernetes.io/docs/reference/command-line-tools-reference/kube-apiserver/
The Kubernetes API
https://kubernetes.io/docs/concepts/overview/kubernetes-api/
kube-apiserver
https://kubernetes.io/docs/concepts/overview/components/#kube-apiserver