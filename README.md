# CICD
$${\color{green}Comeplete  \space  CICD \space  echo \space  system \space  with \space  GithubActions \space  and  \space ArgoCd \space  and \space  Kustomize \space  and \space  Azure \space  Kubernetes}$$
## Comeplete CICD echo system with GithubActions and ArgoCd and Kustomize and Azure Kubernetes
## Here is the complete repo structure is 
## root
## ├── .github
## │   ├── workflows
## │   │   ├── dev-ci.yaml
## │   │   ├── qa-ci.yaml
## │   │   ├── uat-ci.yaml
## │   │   ├── hf-ci.yaml
## ├── app
## │   ├── source code files
## ├── kustomize
## │   ├── base
## │   │   ├── deployment.yaml
## │   │   ├── service.yaml
## │   ├── overlays
## │   │   ├── dev
## │   │   │   ├── kustomization.yaml
## │   │   │   ├── deployment-patch.yaml
## │   │   │   ├── service-patch.yaml
## │   ├── qa
## │   │   │   ├── kustomization.yaml
## │   │   │   ├── deployment-patch.yaml
## │   │   │   ├── service-patch.yaml
## │   ├── uat
## │   │   │   ├── kustomization.yaml
## │   │   │   ├── deployment-patch.yaml
## │   │   │   ├── service-patch.yaml
## │   ├── hf
## │   │   │   ├── kustomization.yaml
## │   │   │   ├── deployment-patch.yaml
## │   │   │   ├── service-patch.yaml
## │   ├── prod
## │   │   │   ├── kustomization.yaml
## │   │   │   ├── deployment-patch.yaml
## │   │   │   ├── service-patch.yaml


# GitHub Actions Workflows:

## I wil create different GitHub Actions workflows for different environments:

### Dev CI: Automatically deploys code to the Dev environment when a developer pushes changes to the Dev branch.
### QA CI: Similar to Dev CI but for the QA environment.
### UAT CI: Same as above, but for the UAT environment.
### HF CI: Allows manual promotion from Dev, QA, or UAT to the HF environment.

# ArgoCD Setup:

### I will configure ArgoCD to manage deployments:

### I will Create ArgoCD applications for each environment (Dev, QA, UAT, HF, and Prod).
### I will setup Set up sync policies to facilitate automatic promotions from UAT to Prod when changes are pushed to the release branch.
### I Enable manual promotion from Dev, QA, and UAT to HF and Prod environments.
## Enhanced Features:

### Scheduled Deployments: We can configure ArgoCD to schedule deployments, such as syncing changes from the Dev branch to the QA environment at specific times.
### Manual Promotion: Developers can manually trigger promotions from Dev, QA, and UAT to HF and Prod when needed..
### This setup ensures a robust CI/CD pipeline with efficient code promotion and deployment mechanisms across different environments while maintaining a clear separation between development and production.
