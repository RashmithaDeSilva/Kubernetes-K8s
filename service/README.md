### Service

#### Create
~~~sh
kubectl create -f service.yaml
~~~
* This will create new service using .yaml file

#### Apply
~~~sh
kubectl apply -f service.yaml
~~~
* This will apply changes into already created service and also it can be use into create service
* User "apply" for best practices

#### Delete
~~~sh
kubectl delete -f service.yaml
~~~
* This will delete service using .yaml file
___


#### If service didn't work
~~~sh
minikube tunnel
~~~
* Then it will ask password for your local system for expose service into your local system