# 24CC3046-P037 — Azure Resource Locks and Deployment Safety Controls

## Project Overview

A practical Azure governance project that protects production resources from accidental deletion and establishes a safe, documented change process.

### Use Cases
- Prevent accidental deletion of production resources.
- Document a safe change process.
- Demonstrate lock inheritance.
- Study how governance controls can block legitimate automated operations.

### Bottlenecks Addressed
- Resource locks may block legitimate automated operations.
- Lock inheritance may be misunderstood.

## Architecture

See `architecture_diagram.png`.

## Main Azure Resources

```text
Azure Subscription
└── rg-governance-demo
    ├── Production Storage Account
    │   └── CanNotDelete Lock
    └── Test/Demo Resources
```

## Safe Change Workflow

```text
Change Request
      ↓
Review & Approval
      ↓
Check Resource Locks
      ↓
Perform Authorized Change
      ↓
Verify Deployment / Resource State
      ↓
Restore Required Protection
      ↓
Document Change
```

## Evidence to Upload

- Resource Group screenshot
- Storage Account screenshot
- Resource Lock screenshot
- Failed/blocked deletion screenshot
- Resource Group lock / inheritance screenshot
- Azure CLI lock-list output
- Safe-change workflow
- Git commit history

## Suggested Repository Structure

```text
24CC3046-P037/
├── README.md
├── ABSTRACT.md
├── SERVICES.md
├── architecture_diagram.png
├── docs/
│   ├── safe-change-process.md
│   ├── use-case-mapping.md
│   └── viva-notes.md
└── evidence/
    ├── 01-resource-group.png
    ├── 02-storage-account.png
    ├── 03-resource-lock.png
    ├── 04-deletion-blocked.png
    ├── 05-lock-inheritance.png
    └── 06-cli-lock-list.png
```
"# 24CC3046-P037-Azure-Resource-Locks" 
