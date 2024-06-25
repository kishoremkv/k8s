# Learn Kubernates along with me!
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

### Serivce Types: 
> Service is a policy by which we access pods
* Cluster IP - Default Service Type -> Exposes IP internally 
* Node Port - Exposes Node IP on a static port outside the cluster
* LoadBalancer - Exposes service externally using cloud provider's load balancer

> **NOTE**: Services use labels to select pods they target