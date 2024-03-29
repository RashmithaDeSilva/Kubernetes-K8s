# Kubernetes - K8s

### Basic informations

#### Claster
~~~sh
kubectl cluster-info
~~~
* A collection of nodes (machines) that work together to run containerized applications.
* Managed by Kubernetes to provide a unified environment for deploying and managing applications.
* Consists of a control plane (manages the cluster) and multiple nodes (execute the workloads).
* Provides high availability, scalability, and fault tolerance for applications.
* Enables efficient resource utilization and workload distribution across the nodes in the cluster.

#### Node
~~~sh
kubectl get nodes
kubectl get nodes -A
~~~
* A single machine within a Kubernetes cluster.
* Can be a physical server or a virtual machine.
* Responsible for running pods, which are the smallest deployable units in Kubernetes.
* Provides the necessary runtime environment for containers, such as networking and storage.
* Nodes work together to form a distributed and scalable Kubernetes cluster.

#### Namespace
~~~sh
kubectl get namespaces
kubectl get namespaces -A
kubectl get ns
kubectl get ns -A
~~~
*  Provide a way to partition and isolate resources within a Kubernetes cluster.
* Prevent naming conflicts between different applications or teams.
* Enable multiple users or teams to share the same cluster without interfering with each other's resources.

#### Pod
~~~sh
# Show default namespase pods
kubectl get pods

# Show all namespases pods
kubectl get pods -A
kubectl get pods --all-namespaces

# Show specific namespace pods
kubectl get pods --namespace=<namespace-name>
kubectl get pods -n <namespace-name>

# Show additional information
kubectl get pods -o wide
kubectl get pods -n <namespace-name> -o wide

# Get logs and more infomations
kubectl describe pod <pod_name> -n <namespace>
kubectl logs <pod_name> -n <namespace>

# Log in to pod
kubectl exec -it <pod_name> <sell_name>
~~~
* Smallest deployable unit in Kubernetes.
* Can contain one or more tightly coupled containers that share the same network namespace.
* Represents a single instance of a running process or application.
* Acts as the basic building block for deploying and managing applications in Kubernetes.

#### Service
~~~sh
kubectl get services
kubectl get services -A
kubectl get services -n <namespace>
kubectl get services -n <namespace> -o wide
~~~
* An abstraction that defines a logical set of Pods.
* Acts as a stable endpoint for accessing the functionality provided by those Pods.
* Enables communication and discovery between different parts of an application or between different applications.
* Supports load balancing and abstracts the underlying network details.
* Allows applications to scale and evolve independently while maintaining a consistent way to access their components.

#### Remove Files
~~~sh
kubctl delete -f <file_name.yaml>
~~~
* This can be delete created resistors using this file

#### Minikube
~~~sh
minikube start
minikube delete
~~~
* A tool for running Kubernetes clusters locally on a developer's machine.
* Provides a single-node Kubernetes cluster in a virtual machine.
* Enables developers to experiment with Kubernetes features and test applications in a local environment.
* Useful for learning, development, and testing purposes without the need for a full-scale production-like cluster.
* Supports various hypervisors, such as VirtualBox, Hyper-V, and KVM, to create the virtual machine.

#### Kubernetes API Server
~~~sh
kubectl api-resources
~~~