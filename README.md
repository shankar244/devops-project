# DevOps ToDo Application

This project demonstrates a complete DevOps pipeline.

Tools used:
- Python Flask
- Docker
- Jenkins
- Kubernetes
- GitHub

Features:
- Dynamic ToDo application
- CI/CD pipeline
- Containerized deployment

# DevOps CI/CD Pipeline Project 🚀

This project demonstrates a complete **end-to-end DevOps workflow** using modern DevOps tools.

A simple **Flask ToDo application** is containerized with Docker, automatically built and deployed using **Jenkins CI/CD pipeline**, and orchestrated using **Kubernetes (Minikube).**

---

# Project Architecture

```
Developer
   │
   ▼
GitHub Repository
   │
   ▼
GitHub Webhook
   │
   ▼
Jenkins CI/CD Pipeline
   │
   ├── Build Docker Image
   ├── Push Image → DockerHub
   └── Deploy → Kubernetes
            │
            ▼
       Kubernetes Cluster
            │
            ├── Todo App Pod
            ├── PostgreSQL Pod
            └── Persistent Volume
```

---

# Tech Stack

| Tool | Purpose |
|-----|------|
| Flask | Web application |
| Docker | Containerization |
| Jenkins | CI/CD automation |
| Kubernetes | Container orchestration |
| DockerHub | Container registry |
| GitHub | Source control |
| Minikube | Local Kubernetes cluster |

---

# Features

✔ Task creation  
✔ Task deletion  
✔ PostgreSQL persistent storage  
✔ Docker containerized application  
✔ Jenkins automated pipeline  
✔ GitHub webhook auto trigger  
✔ Kubernetes deployment

---

# CI/CD Pipeline

Every code push triggers the pipeline automatically.

```
git push
   ↓
Webhook Trigger
   ↓
Jenkins Pipeline
   ↓
Build Docker Image
   ↓
Push to DockerHub
   ↓
Deploy to Kubernetes
```

---

# Application UI

![App Screenshot](screenshots/app.png)

---

# Jenkins Pipeline

![Pipeline Screenshot](screenshots/jenkins.png)

---

# Kubernetes Deployment

```
kubectl get pods
```

Example output:

```
todo-app-xxxxx   Running
postgres-xxxxx   Running
```

---

# How to Run Locally

### Clone the repository

```
git clone https://github.com/SANKET-tech22/todo-devops-project.git
```

### Build Docker image

```
docker build -t todo-app .
```

### Run container

```
docker run -p 5000:5000 todo-app
```

---

# Kubernetes Deployment

Apply Kubernetes manifests:

```
kubectl apply -f k8s/
```

Check pods:

```
kubectl get pods
```

---

# Future Improvements

- Add Kubernetes Ingress
- Implement Helm charts
- Add Prometheus & Grafana monitoring
- Deploy to cloud Kubernetes (EKS / GKE)

---

# Author

Sanket  
DevOps Enthusiast
