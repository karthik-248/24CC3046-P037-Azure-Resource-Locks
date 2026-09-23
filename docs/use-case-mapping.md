# Use-Case Mapping

| Use Case | Implementation | Evidence |
|---|---|---|
| Prevent accidental deletion | CanNotDelete lock on production Storage Account | Blocked deletion screenshot |
| Safe change process | Review → lock check → authorized change → verify → restore → document | Workflow/document |
| Lock inheritance | Lock at Resource Group scope | Parent/child scope screenshots |
| Automation bottleneck | Analyze a deployment operation affected by a lock | CLI/Portal error evidence |
