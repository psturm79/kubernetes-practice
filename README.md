# 🚀 Kubernetes Practice

Clean and structured **Kubernetes manifests** for hands-on learning and interview prep.  
Includes realistic use cases: apps, configs, storage, security, autoscaling, and monitoring.

---

## 📂 Repository Structure

kubernetes-practice/
├── 01-namespace/        # Namespace definition
│   └── namespace.yaml
│
├── 02-frontend/         # Frontend app (nginx)
│   ├── deployment.yaml
│   ├── service.yaml
│   └── ingress.yaml
│
├── 03-backend/          # Backend app (API)
│   ├── deployment.yaml
│   ├── service.yaml
│   ├── configmap.yaml
│   └── secret.yaml
│
├── 04-database/         # Stateful database
│   ├── statefulset.yaml
│   ├── service.yaml
│   └── pvc.yaml
│
├── 05-security/         # Security policies
│   ├── rbac.yaml
│   └── networkpolicy.yaml
│
├── 06-autoscaling/      # HPA & stress testing
│   ├── hpa.yaml
│   └── stress-pod.yaml
│
├── 07-monitoring/       # Observability stack
│   ├── prometheus.yaml
│   └── grafana.yaml
│
├── kustomization.yaml   # Deploy all at once
└── README.md

---

## 🚀 Quick Start

Deploy everything with Kustomize:
```bash
kubectl apply -k .

Or deploy step by step:

kubectl apply -f 01-namespace/
kubectl apply -f 02-frontend/
kubectl apply -f 03-backend/
kubectl apply -f 04-database/
kubectl apply -f 05-security/
kubectl apply -f 06-autoscaling/
kubectl apply -f 07-monitoring/

🎯 Topics Covered

	•	Deployments, Services & Ingress
	•	ConfigMaps & Secrets
	•	StatefulSets with PVCs
	•	RBAC & Network Policies
	•	Readiness & Liveness Probes
	•	Horizontal Pod Autoscaler
	•	Prometheus & Grafana integration


