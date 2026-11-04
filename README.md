# DevOps Configuration Project

This repository contains Docker, Jenkins,
and Kubernetes configuration files.

## Technologies

- Docker
- Jenkins
- Kubernetes
- Git
- GitHub

## Project Structure

- Dockerfile - Builds Docker image
- Jenkinsfile - Defines CI/CD pipeline
- k8s/deployment.yaml - Kubernetes deployment
- k8s/service.yaml - Kubernetes service
- app/index.html - Sample web application

## Docker Build

docker build -t devops-project:v1 .

## Run Docker Container

docker run -d -p 8080:80 devops-project:v1

## Kubernetes Deployment

kubectl apply -f k8s/

## Check Pods

kubectl get pods

## Check Services

kubectl get services