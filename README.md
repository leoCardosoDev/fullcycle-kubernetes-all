minikube start 
minikube status
minikube stop



kubectl apply -f pod.yaml    
   
kubectl logs pod-exemplo 
kubectl get pods 
kubectl delete pods pod-exemplo  

kubectl create deployment hello-nginx --image=nginx:1.17-alpine 
kubectl get deployments

kubectl expose deployment hello-nginx --type=LoadBalancer --port=80
kubectl get services
minikube service hello-nginx


kubectl delete deployments --all
kubectl apply -f deployment.yaml
kubectl api-resources | grep deployment 
kubectl api-versions
kubectl get deployments
kubectl delete deployment hello-world-nginx
kubectl delete deployment --all  

kubectl apply -f service.yaml
kubectl get svc
minikube service nginx-service 

kubectl apply -f configmap.yaml 
kubectl get configmaps

kubectl apply -f persistent-volume.yaml
kubectl get persistentvolumeclaim

kubectl create secret generic mysql-pass --from-literal=password='a1s2d3f4'
kubctl get secret



