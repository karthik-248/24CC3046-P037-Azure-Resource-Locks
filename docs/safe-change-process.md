# Safe Change Process

1. Submit a change request.
2. Identify the target Azure resource and environment.
3. Check the resource and parent scopes for active locks.
4. Confirm authorization and business/academic approval.
5. Determine whether the requested operation conflicts with the lock.
6. If the change is legitimate, follow the approved exception/change procedure.
7. Execute the change.
8. Verify the resource state and deployment result.
9. Restore the required protection.
10. Record the change, reason, result, and evidence.

**Important:** A lock should not be removed simply because a deployment failed. First determine which operation is blocked and whether the operation is actually required.
