# 🚀 Simple Kubernetes App Deployment

## 📌 Project Overview

This project demonstrates how to deploy a simple static web application on Kubernetes using Docker and Kubernetes core components like Deployment, Service, and Namespace.

The application is containerized using Docker and deployed on a Kubernetes cluster (Minikube).

---

## 🎯 Objectives

* Containerize a simple web application using Docker
* Deploy the application on Kubernetes
* Expose the application using a Service
* Manage resources using a Namespace
* Verify deployment using kubectl

---

## 🛠️ Technologies Used

* Docker
* Kubernetes
* Minikube
* kubectl
* Nginx
* HTML

---

## 📁 Project Structure

```
simple-k8s-app/
├── app/
│   └── index.html
├── Dockerfile
├── namespace.yaml
├── deployment.yaml
├── service.yaml
└── README.md
```

---

## ⚙️ Prerequisites

Make sure you have installed:

* Docker
* Kubernetes (Minikube)
* kubectl

---

## 🚀 Step-by-Step Deployment

### 1. Clone the Repository

```
git clone <your-repo-url>
cd simple-k8s-app
```

---

### 2. Build Docker Image

```
docker build -t <your-dockerhub-username>/simple-k8s-app:latest .
```

---

### 3. Push Image to Docker Hub

```
docker login
docker push <your-dockerhub-username>/simple-k8s-app:latest
```

---

### 4. Start Kubernetes Cluster

```
minikube start
```

---

### 5. Create Namespace

```
kubectl apply -f namespace.yaml
```

---

### 6. Deploy Application

```
kubectl apply -f deployment.yaml
```

---

### 7. Expose Application

```
kubectl apply -f service.yaml
```

---

### 8. Verify Resources

```
kubectl get all -n simple-app
```

---

### 9. Access the Application

```
minikube service simple-k8s-service -n simple-app
```

---

## 📊 Kubernetes Components Used

### 🔹 Namespace

Used to isolate project resources.

### 🔹 Deployment

Manages application pods and replicas.

### 🔹 Pod

Runs the containerized application.

### 🔹 Service (NodePort)

Exposes the application externally.

---

## 🔄 Scaling the Application

Increase replicas:

```
kubectl scale deployment simple-k8s-app --replicas=3 -n simple-app
```

---

## 🔁 Rolling Update

Restart deployment:

```
kubectl rollout restart deployment simple-k8s-app -n simple-app
```

---

## 🧹 Cleanup

Delete resources:

```
kubectl delete namespace simple-app
```

---

## 📸 Screenshots to Include

* Docker image build
* Docker push
* Kubernetes nodes
* Pods running
* Services
* Browser output

---

## 💡 Key Learnings

* Docker image creation and management
* Kubernetes resource creation using YAML
* Deployment and scaling of applications
* Service exposure using NodePort
* Namespace isolation

---

## 📄 Resume Description

Deployed a containerized web application on Kubernetes using Docker, Deployment, Namespace, and NodePort Service. Managed application lifecycle, scaling, and service exposure using kubectl.

---

## ⭐ Future Improvements

* Add Ingress for routing
* Use ConfigMap
* Add liveness and readiness probes
* Implement CI/CD pipeline
* Add monitoring (Prometheus & Grafana)

---
