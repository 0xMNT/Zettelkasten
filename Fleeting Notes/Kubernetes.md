20241003153212

tags: #it #devops
links: 
- [[Orchestration]] 
- [[Container]] 
- [[Cloud]]
- [[Kubernetes Networking]]
- [[Kubernetes Best Practices]]
- [[Kubernetes Deployment Strategies]]

# Kubernetes

---

# Control Plane

The Control Plane manages the Kubernetes cluster and runs on one or more Master Nodes. The main components include:

[[kube-apiserver]]: The front-end for the Kubernetes API, handling all REST requests.
[[kube-scheduler]]: Assigns pods to appropriate worker nodes based on resource availability.
[[kube-controller-manager]]: Ensures the desired state of the cluster is maintained through various controllers.
[[etcd]]: A distributed key-value store that holds the cluster's state and configuration data.

# Worker Nodes

[[Pod|Pods]] are the smallest deployable units in Kubernetes. Each pod can contain one or more containers that share the same network namespace and storage.

---
# Resources
