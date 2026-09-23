# Services / Technologies Required

| Service / Tool | Purpose |
|---|---|
| **Microsoft Azure Subscription** | Cloud environment in which the project is implemented |
| **Azure Resource Group** | Logical container for the project resources |
| **Azure Storage Account / Blob Storage** | Production resource used to demonstrate protection |
| **Azure Resource Locks** | Prevent accidental deletion or modification |
| **Azure Resource Manager (ARM)** | Management layer for Azure resources and deployments |
| **Microsoft Entra ID / Azure RBAC** | Identity and role-based access control for authorized operations |
| **Azure Activity Log** | Provides evidence/audit information for management operations |
| **Azure Monitor** | Optional monitoring and operational visibility |
| **Azure Cloud Shell / Azure CLI** | Command-line inspection and management of locks |
| **GitHub** | Source control, documentation, evidence, and project portfolio |
| **GitHub Actions** | Optional CI/CD demonstration for deployment-safety checks |

## Core Services vs Optional Services

### Core
Azure Subscription, Resource Group, Storage Account, Resource Locks, ARM, Azure RBAC/Entra ID, Azure CLI, GitHub.

### Optional for a stronger demonstration
Azure Activity Log, Azure Monitor, and GitHub Actions.

## Minimum Working Demonstration

The minimum implementation should contain:
1. `rg-governance-demo`
2. Production Storage Account
3. `CanNotDelete` Resource Lock
4. Deletion-blocking demonstration
5. Resource Group-level lock/inheritance demonstration
6. Safe change workflow documentation
7. GitHub repository containing abstract, architecture, service list, screenshots/evidence, and README.
