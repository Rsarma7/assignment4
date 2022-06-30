# assignment4
some basic comands i have used
User command 
Docker login –username r647
It will for password 

tag your local image with username /reponame
docker push usename/reponame

minikube start 
or 
minikube start <cluster name>

kubectl config get-cluster  = to see if cluster is running or not

kubectl deployment <DeploymentName> --image= <image name>

kubectl get pods  ===== if pod is runing 

kubectl expose deployment <spring-web> --type=LoadBalancer --port 80 --target-port 8080 ==== to expose to port 

Minikube ip ==== to get the ip of the pod 
kubectl get service === to get the port
  
Be prepared to show pod logs during demonstration, and how to debug errors if Pod crashes

imagepullbackoff error debuging
create secreate.

add 
imagePullSecrets:
- name: regcred

kubectl create secret docker-registry regcred --docker-username=r647 --docker-password=******** --docker-email=rahulthesharma01@gmail.com -n my-app

command for autoscaling -- kubectl autoscale deployment myapp --cpu-percent=60 --min=1 --max=10
