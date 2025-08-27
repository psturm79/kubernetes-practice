#  Kubernetes Practice

This repository contains hands-on Kubernetes manifests for practicing and preparing for interviews. It covers essential use cases every DevOps/SRE engineer should know.

---

##  Repository Structure

```text
kubernetes-practice/
├── 01-deployment/        # Basic NGINX Deployment
│   └── nginx-deploy.yaml
├── 02-service/           # ClusterIP Service for NGINX
│   └── nginx-service.yaml
├── 03-configmap-secret/  # Configuration & secrets
│   ├── configmap.yaml
│   └── secret.yaml
├── 04-pod-env/           # Pod with environment variables
│   └── app-pod.yaml
├── 05-healthchecks/      # Liveness & readiness probes
│   └── nginx-deploy-probes.yaml
└── 06-hpa/               # Horizontal Pod Autoscaler
    └── hpa.yaml
⸻

📝 New README.md

# 🚀 Kubernetes Practice

A practical collection of **Kubernetes manifests** for learning, testing, and interview preparation.  
Organized by topic with step-by-step examples for **apps, configs, storage, security, autoscaling, and monitoring**.

---

## 📂 Repository Overview

| Folder              | Description                                    |
|---------------------|------------------------------------------------|
| `manifests/apps`    | Frontend (NGINX) and Backend API deployments   |
| `manifests/database`| StatefulSet + PersistentVolume for DB          |
| `manifests/security`| RBAC roles, service accounts & network policies|
| `manifests/autoscaling` | Horizontal Pod Autoscaler with demo app    |
| `manifests/monitoring`  | Prometheus & Grafana stack                 |
| `kustomization.yaml`| Deploys everything at once                     |

---

## 🚀 Quick Start

Apply everything at once:

```bash
kubectl apply -k manifests/

Or apply a specific component:

kubectl apply -f manifests/apps/frontend/
kubectl apply -f manifests/database/

⸻

🎯 Topics Covered

✅ Deployments, Services & Ingress
✅ ConfigMaps & Secrets
✅ StatefulSets with PVCs
✅ RBAC & Network Policies
✅ Health Checks (Liveness & Readiness Probes)
✅ Horizontal Pod Autoscaler (HPA)
✅ Monitoring with Prometheus & Grafana

⸻

📖 How to Use This Repo

1. Clone the repo:

git clone https://github.com/psturm79/kubernetes-practice.git
cd kubernetes-practice

2. Deploy apps:

kubectl apply -f manifests/apps/frontend/
kubectl apply -f manifests/apps/backend/

3. Check pods:

kubectl get pods

4. Access NGINX frontend:

kubectl port-forward svc/nginx-service 8080:80

⸻

🛠️ Requirements

•	Kubernetes cluster (Minikube, Kind, Docker Desktop, or cloud provider)
•	kubectl installed
•	Optional: kustomize for multi-env deployments

⸻

👨‍💻 Author

Pablo Sturm
DevOps & Cloud Engineer | Azure | Kubernetes | Automation
GitHub • LinkedIn

⸻⸻
