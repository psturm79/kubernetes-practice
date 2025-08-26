kubernetes-practice/
├── 00-namespace/           # Workspace separation
│   └── namespace.yaml
│
├── 01-frontend/            # Frontend app (nginx)
│   ├── deployment.yaml
│   ├── service.yaml
│   └── ingress.yaml
│
├── 02-backend/             # Backend app (API)
│   ├── deployment.yaml
│   ├── service.yaml
│   ├── configmap.yaml
│   └── secret.yaml
│
├── 03-database/            # Stateful database
│   ├── statefulset.yaml
│   ├── service.yaml
│   └── pvc.yaml
│
├── 04-security/            # Security policies
│   ├── rbac.yaml
│   └── networkpolicy.yaml
│
├── 05-autoscaling/         # HPA & stress testing
│   ├── hpa.yaml
│   └── stress-pod.yaml
│
├── 06-monitoring/          # Observability stack
│   ├── prometheus.yaml
│   └── grafana.yaml
│
├── kustomization.yaml       # Deploy all at once
└── README.md


