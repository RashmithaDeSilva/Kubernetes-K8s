### Using "YAML" Files

#### Create
~~~sh
kubectl create -f namespace.yaml
~~~
* This will create new namespace using .yaml file

#### Apply
~~~sh
kubectl apply -f namespace.yaml
~~~
* This will apply changes into already created namespace also it can be use into create namespace

#### Delete
~~~sh
kubectl delete -f namespace.yaml
~~~
* This will delete namespaces using .yaml file
___

### Using Commands

#### Create
~~~sh
kubectl create namespace <namespace_name>
~~~

####  Delete
~~~sh
kubectl delete namespace <namespace_name>
~~~
