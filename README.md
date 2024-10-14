# K8s-cluster-setup
# Kubernetes Cluster Setup

A basic setup of a Kubernetes cluster using Minikube. This project demonstrates deploying an NGINX application.

## Features

- Local Kubernetes cluster using Minikube.
- Deployment of NGINX with 2 replicas.
- Exposed service for web access.

## Setup Instructions
A.)
1. Install [Docker](https://docs.docker.com/get-docker/).
2. Install [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/).
3. Install [Minikube](https://minikube.sigs.k8s.io/docs/start/).
4. Start Minikube:
   ```bash
   minikube start
B.)
Deploy the application:kubectl apply -f nginx-deployment.yaml
C.)
Expose the deployment:kubectl expose deployment nginx-deployment --type=NodePort --port=80
D.)
Get the service URL:minikube service nginx-deployment --url
