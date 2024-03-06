### Deployment
* A Kubernetes object used to define and manage the desired state of an application.
* Describes the application's deployment, including the number of replicas, the container image to use, and other settings.
* Manages the creation, updating, and scaling of application instances (pods).
* Provides features like rolling updates and rollbacks, making it easier to manage changes to the application.
* Ensures that the specified number of replicas are always running, helping maintain the desired state of the application.

#### Create
~~~sh
kubectl create -f deployment.yaml
~~~
* This will create new deployment using .yaml file

#### Apply
~~~sh
kubectl apply -f deployment.yaml
~~~
* This will apply changes into already created deployment and also it can be use into create deployment
* User "apply" for best practices

#### Delete
~~~sh
kubectl delete -f deployment.yaml
~~~
* This will delete deployment using .yaml file

#### Delete Deployed Pod
~~~sh
kubectl delete pod <pod_name> -n <namespace_name>
~~~
* This will delete single pod using pod name

#### Get Info
~~~sh
kubectl get deployments -n <namespace_name>
~~~
~~~sh
kubectl get pods -n <namespace_name>

kubectl get pods -n <namespace_name> -o wide
~~~
* In her deploy for this pod, we used the development namespace


