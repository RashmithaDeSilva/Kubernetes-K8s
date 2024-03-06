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

#### Namespace
~~~k8s
kubectl get namespaces
kubectl get namespaces -A
kubectl get ns
kubectl get ns -A
~~~
*  Provide a way to partition and isolate resources within a Kubernetes cluster.
* Prevent naming conflicts between different applications or teams.
* Enable multiple users or teams to share the same cluster without interfering with each other's resources.

#### Pod
~~~k8s
# Show default namespase pods
kubectl get pods

# Show all namespases pods
kubectl get pods -A
kubectl get pods --all-namespaces

# Show specific namespace pods
kubectl get pods --namespace=<namespace-name>

# Show with additional information
kubectl get pods -o wide
kubectl get pods --namespace=<namespace-name> -o wide

~~~
* Smallest deployable unit in Kubernetes.
* Can contain one or more tightly coupled containers that share the same network namespace.
* Represents a single instance of a running process or application.
* Acts as the basic building block for deploying and managing applications in Kubernetes.