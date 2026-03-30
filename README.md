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
