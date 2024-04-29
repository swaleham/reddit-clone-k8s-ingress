# Reddit Clone App on Kubernetes with Ingress
This project demonstrates how to deploy a Reddit clone app on Kubernetes with Ingress and expose it to the world using Minikube as the cluster.
## Prerequisites
Before you begin, you should have the following tools installed on your local machine: 

- Docker
- Minikube cluster ( Running )
- kubectl
- Git

<img src="https://github.com/swaleham/reddit-clone-k8s-ingress/blob/main/IngressK8s.svg">

## Installation

1. **Clone the repository to your local machine: git clonehttps://github.com/swaleham/reddit-clone-k8s-ingress.git.**
2. **Navigate to the project directory: cd reddit-clone-k8s-ingress.**
3. **Build the Docker image : docker build -t reddit-clone-app .**
4. **Deploy the app to Kubernetes: kubectl apply -f deployment.yaml**
5. **Deploy the Service for deployment to Kubernetes: kubectl apply -f service.yaml**
6. **Enable Ingress by using Command: minikube addons enable ingress**
7. **Expose the app as a Kubernetes service: kubectl expose deployment reddit-deployment --type=NodePort --port=5000**
8. **Create an Ingress resource: kubectl apply -f ingress.yaml**
