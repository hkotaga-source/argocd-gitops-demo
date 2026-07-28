# ArgoCD GitOps Demo

Simple but complete GitOps setup using ArgoCD.

## What you get

- ArgoCD Application example
- ApplicationSet for multi-environment
- Progressive delivery ideas (canary / blue-green notes)
- Folder structure ready for real apps

## Quick Start

```bash
# Install ArgoCD (one-time)
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

# Apply the demo Application
kubectl apply -f argocd/application.yaml
```

## Structure

```
├── argocd/
│   ├── application.yaml
│   └── applicationset.yaml
├── apps/
│   └── sample-app/
└── README.md
```

Created for SRE/DevOps portfolio – https://github.com/hkotaga-source
