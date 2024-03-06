# Kubernetes - K8s

### Basic informations

#### Claster
~~~k8s
kubectl cluster-info
~~~
* A collection of nodes (machines) that work together to run containerized applications.
* Managed by Kubernetes to provide a unified environment for deploying and managing applications.
* Consists of a control plane (manages the cluster) and multiple nodes (execute the workloads).
* Provides high availability, scalability, and fault tolerance for applications.
* Enables efficient resource utilization and workload distribution across the nodes in the cluster.

#### Node
~~~k8s
kubectl get nodes
kubectl get nodes -A
~~~
* A single machine within a Kubernetes cluster.
* Can be a physical server or a virtual machine.
* Responsible for running pods, which are the smallest deployable units in Kubernetes.
* Provides the necessary runtime environment for containers, such as networking and storage.
* Nodes work together to form a distributed and scalable Kubernetes cluster.