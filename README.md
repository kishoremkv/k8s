# Learn Kubernetes along with me!
Resources - https://projects.100xdevs.com/

## Sample commands
* kind create cluster --name local
* kind delete cluster -n local

--> kubectl is a tool to interact with kubernates clusters
* kubectl get pods
* kubectl get nodes
* docker run -p 3005:80 nginx
* kubectl run nginx --image=nginx --port=80
* kubectl describe pod nginx
* kubectl delete pod nginx
* kubectl apply -f rs.yml
* kubectl rollout history deployment/nginx-deployment
* kubectl get pods -owide
* kubectl logs -f nginx
* kubectl create namespace backend-team
* kubectl get namespaces
* kubectl get pods -n my-namespace
* kubectl config set-context --current --namespace=default
* kubectl describe configmap ecom-backend-config

### Serivce Types: 
> Service is a policy by which we access pods
> Services let you expose your pods to other pods/over the internet
* Cluster IP - Default Service Type -> Exposes IP internally
* Node Port - Exposes Node IP on a static port outside the cluster
* LoadBalancer - Exposes service externally using cloud provider's load balancer

> **NOTE**: Services use labels to select pods they target

### Downsides of Services:
* No centralized traffic management
* Multiple certificates for every route
* No centralized logic to handle rate limitting to all services


### Ingress and Ingress Controller
* An API object that manages external access to the services in a cluster, typically HTTP. 
* Ingress exposes HTTP and HTTPS routes from outside the cluster to services within the clus9ter. 

### Namespaces
* Divides cluster resources between multiple users/teams

### Secrets and config maps
* To store the configuration of your application outside image/pod
* 
