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

Topics Covered

	•	Deployments – Manage NGINX pods and scaling
	•	Services – Internal application exposure with ClusterIP
	•	ConfigMaps & Secrets – Configuration management and sensitive data
	•	Environment Variables – Inject into containers via Pod spec
	•	Health Checks – Readiness & liveness probes to enhance reliability
	•	Autoscaling – Horizontal Pod Autoscaler to adapt to load

⸻

Usage

Apply manifests:

kubectl apply -f 01-deployment/nginx-deploy.yaml
kubectl get pods

Goal

Design for Kubernetes interview preparation and practical review of core concepts using real-world YAML examples.

⸻

✍️ Created by Pablo Sturm
