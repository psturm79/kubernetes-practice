
📂 New Folder Structure

kubernetes-practice/
│── manifests/
│   ├── apps/
│   │   ├── frontend/         # NGINX Deployment + Service + Ingress
│   │   └── backend/          # Backend API Deployment + Service
│   ├── database/             # Stateful DB with PVC
│   ├── security/             # RBAC + Network Policies
│   ├── autoscaling/          # Horizontal Pod Autoscaler examples
│   └── monitoring/           # Prometheus + Grafana stack
│
│── kustomization.yaml        # Deploy all at once
│── README.md                 # Main documentation


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
	•	✅ Deployments, Services & Ingress
	•	✅ ConfigMaps & Secrets
	•	✅ StatefulSets with PVCs
	•	✅ RBAC & Network Policies
	•	✅ Health Checks (Liveness & Readiness Probes)
	•	✅ Horizontal Pod Autoscaler (HPA)
	•	✅ Monitoring with Prometheus & Grafana

⸻

📖 How to Use This Repo
	1.	Clone the repo:

git clone https://github.com/psturm79/kubernetes-practice.git
cd kubernetes-practice


	2.	Deploy apps:

kubectl apply -f manifests/apps/frontend/
kubectl apply -f manifests/apps/backend/


	3.	Check pods:

kubectl get pods


	4.	Access NGINX frontend:

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

⸻