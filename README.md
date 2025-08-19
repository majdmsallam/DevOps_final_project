
# 🚀 DevOps Final Project

## 📌 Project Overview
This project demonstrates a complete DevOps pipeline designed to **build, test, and deploy a containerized application** on **Amazon EKS**.  
It highlights the use of modern DevOps practices, including:

- 🏗️ **Infrastructure as Code (IaC)**  
- ⚙️ **Continuous Integration & Delivery with GitHub Actions**  
- ☸️ **Kubernetes orchestration on AWS EKS**

---

## 🛠 Project Structure
- 📂 **EKS_Cluster/** → IaC configuration for provisioning the EKS cluster.  
- 📂 **k8s_manifests/** → Kubernetes YAML manifests (Deployments, Services, StatefulSets, etc.).  
- 📂 **namegen/** → Application source code + **Dockerfile** to build the container image.  
- 📂 **.github/workflows/** → GitHub Actions pipelines for automation (CI/CD).  

---

## 📋 Requirements
Before using this project, make sure you have:

- 🐳 **Docker** installed locally  
- ☁️ **AWS CLI** configured with access to manage EKS  
- 🔧 **kubectl** set up to communicate with your EKS cluster  
- 🔑 **GitHub Actions** enabled on your repository  

---

## 💻 Cluster Management

### 🚀 Create an EKS Cluster
```bash
eksctl create cluster -f ./EKS_Cluster/cluster.yaml
```

### 🚀 delete an EKS Cluster
```bash
eksctl delete cluster -f ./EKS_Cluster/cluster.yaml
```
