#  Start Minikube
minikube start --driver=docker


# Deploy to Kubernetes
kubectl apply -f k8s/deployment.yaml  

kubectl apply -f k8s/service.yaml

# Access the Web App
http://localhost:3000/calculate?num1=10&num2=5&operation=add

