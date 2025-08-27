🚀 Kubernetes Practice

A clean and structured collection of Kubernetes manifests for learning, testing, and interview preparation.
Covers apps, configs, storage, security, autoscaling, and monitoring.

⸻

📂 Repository Structure
	•	01-namespace → Namespace definition
	•	02-frontend → Nginx Deployment + Service + Ingress
	•	03-backend → API Deployment + Service + ConfigMap + Secret
	•	04-database → StatefulSet + Service + PersistentVolumeClaim
	•	05-security → RBAC roles + Network Policies
	•	06-autoscaling → Horizontal Pod Autoscaler + Stress Pod
	•	07-monitoring → Prometheus + Grafana stack
	•	kustomization.yaml → Deploy everything at once
	•	README.md → Documentation

---

🚀 Quick Start

Deploy everything with Kustomize:

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

✅ Deployments, Services & Ingress
✅ ConfigMaps & Secrets
✅ StatefulSets with PVCs
✅ RBAC & Network Policies
✅ Readiness & Liveness Probes
✅ Horizontal Pod Autoscaler
✅ Prometheus & Grafana integration

⸻

✍️ Created by Pablo Sturm

