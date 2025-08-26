# 🚀 Kubernetes Practice  

This repository contains **hands-on Kubernetes manifests** for practicing and preparing for interviews.  
It covers the most common use cases every DevOps / SRE engineer should know.  

---

# 📂 Repository Structure

```yaml
kubernetes-practice/
├── 01-deployment/          # Basic NGINX Deployment
│   └── nginx-deploy.yaml
├── 02-service/             # ClusterIP Service for NGINX
│   └── nginx-service.yaml
├── 03-configmap-secret/    # Store configuration & secrets
│   ├── configmap.yaml
│   └── secret.yaml
├── 04-pod-env/             # Pod with environment variables
│   └── app-pod.yaml
├── 05-healthchecks/        # Liveness & Readiness Probes
│   └── nginx-deploy-probes.yaml
└── 06-hpa/                 # Horizontal Pod Autoscaler
    └── hpa.yaml

---

## 📘 Topics Covered

- 📦 **Deployments** – Run and manage NGINX Pods  
- 🌐 **Services** – Expose applications inside the cluster  
- ⚙️ **ConfigMaps & Secrets** – Manage configuration and sensitive data  
- 🌱 **Pod Environment** – Inject environment variables into containers  
- 🩺 **Health Checks** – Liveness & Readiness probes  
- 📈 **Autoscaling** – Horizontal Pod Autoscaler (HPA)  

---

## 🛠️ Usage

Apply any manifest using:

```bash
kubectl apply -f <file>.yaml

Example:

kubectl apply -f 01-deployment/nginx-deploy.yaml
kubectl get pods

🎯 Goal

This repository is designed for Kubernetes interview preparation and for anyone who wants to quickly review the most common Kubernetes concepts with practical YAML manifests.

⸻

✍️ Created by Pablo Sturm
