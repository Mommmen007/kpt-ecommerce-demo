# E-commerce Kubernetes Deployment (kpt demo)

## Overview
This project demonstrates how to deploy and scale a microservices-based e-commerce application using Kubernetes.

## Features
- Kubernetes Deployment
- Service Exposure (NodePort)
- Horizontal Scaling
- Easy Configuration

## Architecture
- Deployment manages application pods
- Service exposes the application externally
- Docker container running Nginx
- Kubernetes Deployment manages replicas
- Service exposes the application
- GitHub Actions handles CI pipeline
- Health checks ensure reliability
- Resource limits control performance

## Containerization

   This project includes a Dockerfile to containerize the application using Nginx.

   Build the image:
   docker build -t ecommerce-app .

Run the container:
docker run -p 8080:80 ecommerce-app

## CI/CD

This project uses GitHub Actions to automatically build the Docker image on every push.

## How to Run
1. Apply deployment:
   kubectl apply -f k8s/deployment.yaml

2. Apply service:
   kubectl apply -f k8s/service.yaml

3. Access app:
   http://localhost:30007

## Future Work
- Convert into kpt package
- Add environment-based configurations
- Implement CI/CD pipeline
