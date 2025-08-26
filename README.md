kubernetes-practice/
├── README.md
├── kustomization.yaml
├── namespaces/
│   └── dev-namespace.yaml
├── apps/
│   ├── frontend/
│   │   ├── deployment.yaml
│   │   ├── service.yaml
│   │   └── ingress.yaml
│   ├── backend/
│   │   ├── deployment.yaml
│   │   ├── service.yaml
│   │   └── configmap.yaml
│   └── database/
│       ├── statefulset.yaml
│       ├── service.yaml
│       └── pvc.yaml
├── security/
│   ├── rbac.yaml
│   └── networkpolicy.yaml
├── monitoring/
│   ├── prometheus.yaml
│   └── grafana.yaml
└── autoscaling/
    ├── hpa.yaml
    └── stress-test-pod.yaml

