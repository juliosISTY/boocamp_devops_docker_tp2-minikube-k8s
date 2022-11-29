# boocamp_devops_docker_tp2-minikube-k8s

## Commandes impératives

### For creating and running a pod
> kubectl run --image=mmumshad/simple-webapp-color --env "APP_COLOR=red" --restart=Never simple-webapp-color

### For creating and running deployment ressource
> kubectl create deployment nginx-deploy --image=nginx:1.18.0

* To update number of replicasets
> kubectl scale deployment nginx-deploy --replicas=2

* To edit a tag of pod image in the deployment
>  kubectl set image deployment nginx-deploy nginx=latest


