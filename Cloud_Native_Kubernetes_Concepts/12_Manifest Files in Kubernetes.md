Manifest Files in Kubernetes
Manifest (not technical description)

A Manifest file is a document that is commonly used for customs to list the contents of cargo, or passengers. Its an itemized list of things.

Manifest File (in the context of Kubernetes)

A Manifest file is a generalized name for any Kubernetes Configuration File that define the configuration of various K8s components.

These are all Manifest files with specific purposes:

Deployment File
PodSpec File
Network Policy File
Manifest Files can be written in either:

YAML
JSON
A manifest can contain multiple K8s component definitions/configurations.

In YAML you can see the three hyphens --- is used to defined multiple components.

kubectl apply command is generally used to deploy manifest files

Resource Configuration file is sometimes used to describe multiple resources in a manifest.

Reference
Kubectl