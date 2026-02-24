# DevOps CI/CD Pipeline with Docker

This project demonstrates an **end-to-end CI/CD pipeline** for a Node.js application using **Docker** and **GitHub Actions**. The pipeline automatically builds and pushes Docker images to Docker Hub whenever code changes are pushed. Kubernetes manifests are included for deployment, but the deployment step is currently skipped for local Minikube.

## Features

- Node.js application
- Dockerized container
- CI/CD pipeline with GitHub Actions
- Automated Docker image build & push
- Kubernetes manifests ready for deployment

## Setup

1. Clone the repo:

```bash
git clone https://github.com/sochy01/devops-cicd-k8s.git
cd devops-cicd-k8s

2. Install dependencies:

cd app
npm install

3. Run locally:
npm start

Build Docker image manually (optional):

docker build -t sochy01/devops-app:latest .
docker run -p 3000:3000 sochy01/devops-app:latest

CI/CD Pipeline

Triggered on push to main branch
Builds Docker image and pushes to Docker Hub
Kubernetes deployment ready but skipped for local Minikube

Here is what i accomplished so far:

Node.js app created and Dockerized ✅
Git repo initialized and pushed to GitHub ✅
Docker image automatically builds and pushes to Docker Hub via GitHub Actions ✅
Kubernetes deployment step skipped (so pipeline passes on GitHub) ✅
