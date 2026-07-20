# 🚀 Three-Tier Web Application Deployment on AWS EKS

A production-style Three-Tier Web Application deployed on **Amazon Elastic Kubernetes Service (EKS)** using **Terraform**, **Kubernetes**, **Docker**, **Helm**, **MongoDB**, and the **AWS Load Balancer Controller**.

This project demonstrates how to provision cloud infrastructure using Infrastructure as Code (Terraform), deploy containerized applications to Kubernetes, expose them using an AWS Application Load Balancer (ALB), and connect frontend, backend, and database services within a scalable Kubernetes environment.

---

# 📌 Project Overview

This project deploys a complete Three-Tier Web Application on Amazon EKS.

The application consists of:

- React Frontend
- Node.js Backend REST API
- MongoDB Database
- Kubernetes Deployments
- Kubernetes Services
- Kubernetes Ingress
- AWS Application Load Balancer (ALB)
- Infrastructure provisioned using Terraform

The project follows modern DevOps practices including:

- Infrastructure as Code (IaC)
- Containerization
- Kubernetes Orchestration
- Cloud Native Deployment
- Scalable Microservice Architecture

---

# 🏗️ Three-Tier Architecture

The application follows a standard Three-Tier Architecture.

```
                User
                  │
                  ▼
     AWS Application Load Balancer
                  │
                  ▼
      Kubernetes Ingress Controller
                  │
        ┌─────────┴─────────┐
        │                   │
        ▼                   ▼
 Frontend Service      Backend Service
        │                   │
        ▼                   ▼
  React Frontend      Node.js API
                            │
                            ▼
                    MongoDB Service
                            │
                            ▼
                        MongoDB
```

All components run inside Kubernetes Pods and communicate internally through Kubernetes Services.

---

# 🛠️ Technology Stack

| Category | Technology |
|----------|------------|
| Cloud Platform | AWS |
| Containerization | Docker |
| Orchestration | Kubernetes (Amazon EKS) |
| Infrastructure as Code | Terraform |
| Package Manager | Helm |
| Database | MongoDB |
| Ingress | AWS Load Balancer Controller |
| Load Balancer | AWS Application Load Balancer |
| Version Control | Git & GitHub |

---

# ✨ Features

- Deploy Amazon EKS Cluster using Terraform
- Deploy React Frontend
- Deploy Node.js Backend API
- Deploy MongoDB Database
- Kubernetes Deployments & Services
- Kubernetes Ingress Resource
- AWS Application Load Balancer Integration
- Internal Service-to-Service Communication
- Scalable Containerized Architecture
- Infrastructure as Code (IaC)

---

# 📂 Project Structure

```
three-tier-web-app-eks
│
├── app/
│   ├── frontend/
│   ├── backend/
│   └── mongodb/
│
├── k8s_manifests/
│   ├── frontend-deployment.yaml
│   ├── api-deployment.yaml
│   ├── mongodb-deployment.yaml
│   ├── services.yaml
│   └── ingress.yaml
│
├── terraform/
│   ├── provider.tf
│   ├── vpc.tf
│   ├── eks.tf
│   ├── iam.tf
│   ├── monitoring.tf
│   └── variables.tf
│
└── README.md
```

---

# 🚀 Deployment Workflow

```
Terraform
     │
     ▼
Creates AWS Infrastructure
     │
     ▼
Amazon EKS Cluster
     │
     ▼
Deploy Kubernetes Manifests
     │
     ▼
Pods & Services Created
     │
     ▼
Ingress Controller
     │
     ▼
AWS Application Load Balancer
     │
     ▼
Access Application
```

---

# ☁️ AWS Services Used

- Amazon EKS
- Amazon EC2
- Amazon VPC
- IAM
- Application Load Balancer (ALB)
- Elastic Container Registry (Optional)

---

# 📖 Kubernetes Resources

- Namespace
- Deployment
- Service
- ReplicaSet
- Ingress
- Pods

---

# 📸 Project Demonstration

The application provides:

- Add a new task
- Display task list
- Delete tasks
- Store task data in MongoDB
- Frontend communicates with Backend API
- Backend communicates with MongoDB
- Public access through AWS Application Load Balancer

---

# 🎯 Learning Outcomes

Through this project, I learned:

- Provisioning infrastructure using Terraform
- Deploying applications on Amazon EKS
- Working with Kubernetes Deployments and Services
- Configuring AWS Load Balancer Controller
- Kubernetes Ingress Management
- Containerizing applications with Docker
- Managing cloud-native applications on AWS

---

# 👨‍💻 Author

**Blessvin Shibu**

DevOps & Cloud Enthusiast

GitHub: https://github.com/blessvin003

---

# ⭐ If you found this project useful, consider giving it a star.