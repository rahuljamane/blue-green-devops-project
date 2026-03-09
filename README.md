Blue-Green Deployment DevOps Project

This project demonstrates zero-downtime deployment using the Blue-Green deployment strategy with Kubernetes.

Tech Stack

- Python (Flask)
- Docker
- Kubernetes
- Jenkins
- GitHub

Architecture

Developer → GitHub → Jenkins Pipeline → Docker Image → Kubernetes Cluster → Blue/Green Deployment

Features

- Containerized Python application
- Kubernetes blue-green deployment strategy
- CI/CD pipeline using Jenkins
- Zero downtime updates

Run Application

Build Docker image:

docker build -t bluegreen-app -f docker/Dockerfile .

Deploy Blue:

kubectl apply -f kubernetes/blue-deployment.yaml

Deploy Service:

kubectl apply -f kubernetes/service.yaml
