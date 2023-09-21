# CICD
Comeplete CICD echo system with GithubActions and ArgoCd and Kustomize and Azure Kubernetes
Here is the complete repo structure is 
root
├── .github
│   ├── workflows
│   │   ├── dev-ci.yaml
│   │   ├── qa-ci.yaml
│   │   ├── uat-ci.yaml
│   │   ├── hf-ci.yaml
├── app
│   ├── source code files
├── kustomize
│   ├── base
│   │   ├── deployment.yaml
│   │   ├── service.yaml
│   ├── overlays
│   │   ├── dev
│   │   │   ├── kustomization.yaml
│   │   │   ├── deployment-patch.yaml
│   │   │   ├── service-patch.yaml
│   ├── qa
│   │   │   ├── kustomization.yaml
│   │   │   ├── deployment-patch.yaml
│   │   │   ├── service-patch.yaml
│   ├── uat
│   │   │   ├── kustomization.yaml
│   │   │   ├── deployment-patch.yaml
│   │   │   ├── service-patch.yaml
│   ├── hf
│   │   │   ├── kustomization.yaml
│   │   │   ├── deployment-patch.yaml
│   │   │   ├── service-patch.yaml
│   ├── prod
│   │   │   ├── kustomization.yaml
│   │   │   ├── deployment-patch.yaml
│   │   │   ├── service-patch.yaml
