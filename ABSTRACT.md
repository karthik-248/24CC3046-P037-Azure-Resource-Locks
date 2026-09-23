# Abstract — Azure Resource Locks and Deployment Safety Controls

**Project Code:** 24CC3046-P037  
**Domain:** Governance  
**Team:** T037 / T139 / T241 (use your actual allotted team ID)

## Abstract

Production cloud resources can be accidentally deleted or modified during manual administration, infrastructure changes, or automated deployments. This project implements an Azure governance solution using **Azure Resource Locks** and a documented **deployment safety control process**.

A production Azure Storage Account is protected using a **CanNotDelete** lock so that authorized users and deployment processes can continue permitted operations while accidental deletion is prevented. The project also demonstrates **lock inheritance** by applying protection at the Resource Group scope and studying how parent-scope locks affect resources beneath them.

A controlled change workflow is defined for legitimate changes: change request, review and approval, lock inspection, controlled execution, verification, and restoration of protection. Azure CLI and Azure Portal are used to inspect and manage locks, while GitHub is used to maintain project documentation and deployment/change evidence.

The final outcome is a practical governance model that reduces accidental destructive operations while keeping legitimate deployment activities manageable and auditable.

## Use Cases

1. Prevent accidental deletion of production Azure resources.
2. Document and demonstrate a safe change/deployment process.
3. Demonstrate the effect of Resource Group-level lock inheritance.
4. Identify how locks can interfere with legitimate automated operations.
5. Maintain configuration, documentation, and evidence in GitHub.

## Expected Outcome

The project should demonstrate that:
- A protected production resource cannot be accidentally deleted while a CanNotDelete lock is active.
- Locks can be applied at resource and Resource Group scopes.
- Parent-scope locks can affect child resources.
- Legitimate changes require a controlled and documented process.
- Deployment failures caused by governance controls can be diagnosed rather than bypassed blindly.
