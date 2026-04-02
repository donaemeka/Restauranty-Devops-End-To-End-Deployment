# 🚀 Restauranty - End-to-End DevOps Deployment

A full-stack **restaurant management platform** built with a **microservices architecture**, where users can browse items, authenticate, and apply discounts in a distributed system running on Kubernetes.

The system demonstrates how modern applications are **deployed, monitored, secured, and automated** using real-world DevOps practices.

---

## 📌 Project Overview

**Restauranty** simulates a real-world production system where multiple backend services communicate reliably and scale independently.

This system replicates how modern cloud-native applications are built and operated in production environments.

It demonstrates:

* Microservices architecture using **Node.js and React**
* Containerization with **Docker**
* Deployment using **Kubernetes**
* Monitoring with **Prometheus & Grafana**
* Secure communication using **Network Policies & Secrets**
* Automated delivery using **GitHub Actions CI/CD**

---

## 🎯 Problem It Solves

Modern applications (such as restaurant platforms) require:

* Independent services (authentication, items, discounts)
* Reliable service-to-service communication
* Scalable infrastructure
* Monitoring and observability

This project shows how to design and operate such systems using DevOps best practices.

---

## 🏗️ Architecture Overview

![Architecture](screenshots/architecture.png)

### 🔄 System Flow

```text
User → NGINX Ingress → Frontend (React) → Backend Services → MongoDB
```

### 🧱 Core Components

* **Frontend:** React.js application
* **Backend:** Auth, Items, Discounts (Node.js microservices)
* **Database:** MongoDB
* **Orchestration:** Kubernetes
* **Monitoring:** Prometheus + Grafana
* **Security:** Network Policies & Secrets

---

## 🔧 Technology Stack

| Layer                | Technology                 | Implementation                      |
| -------------------- | -------------------------- | ----------------------------------- |
| **Application**      | React.js + Node.js         | Frontend UI & Backend Microservices |
| **Containerization** | Docker                     | Service isolation                   |
| **Orchestration**    | Kubernetes (Minikube)      | Deployment & scaling                |
| **Networking**       | NGINX Ingress              | Routing & service discovery         |
| **Database**         | MongoDB                    | Data persistence                    |
| **Monitoring**       | Prometheus + Grafana       | Metrics & dashboards                |
| **CI/CD**            | GitHub Actions             | Automated pipelines                 |
| **Security**         | Network Policies + Secrets | Secure communication                |
| **Infrastructure**   | YAML Manifests             | Infrastructure as Code              |

---

## 📊 Key Achievements

* ✅ Deployed a **multi-service application on Kubernetes**
* ✅ Implemented a **CI/CD pipeline for automated delivery**
* ✅ Integrated **monitoring stack (Prometheus + Grafana)**
* ✅ Applied **network policies for secure service communication**
* ✅ Built a fully containerized production-like environment

---

## 📊 Results

* Improved deployment consistency using containerized environments
* Enabled real-time monitoring and observability
* Reduced manual setup through Infrastructure as Code

---

## 📸 Screenshots

| Application                 | Kubernetes Dashboard                  | Monitoring (Grafana)                             | CI/CD Pipeline                          |
| --------------------------- | ------------------------------------- | ------------------------------------------------ | --------------------------------------- |
| ![App](screenshots/App.png) | ![K8s](screenshots/k8s-dashboard.png) | ![Monitoring](screenshots/grafana-dashboard.png) | ![CI/CD](screenshots/cicd-pipeline.png) |

---

## 🚀 Quick Start

### Prerequisites

* Docker
* Kubernetes (Minikube)
* kubectl

---

### Clone Repository

```bash
git clone https://github.com/donaemeka/restauranty-devops-deployment
cd restauranty-devops-deployment
```

---

### Local Development

```bash
cd infrastructure
docker-compose up -d
```

Access: http://localhost

---

### Kubernetes Deployment

```bash
kubectl apply -f k8s/
minikube tunnel
```

Access: http://localhost

---

### Verify

```bash
kubectl get all
kubectl get ingress
```

---

## 🛠️ DevOps Implementation

### 1️⃣ Containerization

* Multi-stage Docker builds
* Optimized production-ready images

---

### 2️⃣ Kubernetes Orchestration

* Resource limits and requests
* Liveness and readiness probes
* ConfigMaps and Secrets

---

### 3️⃣ Networking

* NGINX Ingress controller
* Service-based communication

---

### 4️⃣ Monitoring

* Prometheus for metrics collection
* Grafana dashboards for visualization

---

### 5️⃣ Security

* Network Policies for service isolation
* Secrets management (no hardcoded credentials)
* Non-root container execution

---

### 6️⃣ CI/CD

* GitHub Actions pipeline
* Automated builds and validation

---

## 📁 Project Structure

```text
restauranty-devops-deployment/
├── backend/
├── client/
├── k8s/
├── infrastructure/
├── .github/workflows/
├── screenshots/
└── README.md
```

---

## 🐞 Troubleshooting

### Application not accessible?

```bash
kubectl get ingress
kubectl get pods
minikube tunnel
```

---

### Services not communicating?

```bash
kubectl get networkpolicies
kubectl get endpoints
```

---

## 🎯 DevOps Skills Demonstrated

| Category               | Tools               | Evidence                         |
| ---------------------- | ------------------- | -------------------------------- |
| Containerization       | Docker              | Multi-service images             |
| Orchestration          | Kubernetes          | Production manifests             |
| Monitoring             | Prometheus, Grafana | Dashboards                       |
| Security               | Network Policies    | Secure communication             |
| CI/CD                  | GitHub Actions      | Automated pipeline               |
| Infrastructure as Code | YAML                | Version-controlled configuration |

---

## 📈 Business Value

* Faster deployments
* Improved reliability
* Built-in security
* Scalable architecture

---

## 👨‍💻 About Me

**Donatus Emeka Anyalebechi**
Junior DevOps Engineer

📍 Germany
📧 [donaemeka92@gmail.com](mailto:donaemeka92@gmail.com)
🔗 https://www.linkedin.com/in/donatus-devops
🐙 https://github.com/donaemeka

---

⭐ Built to demonstrate real-world DevOps capabilities
