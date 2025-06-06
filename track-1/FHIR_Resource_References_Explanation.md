
# Why References Must Be Rewritten When Uploading FHIR Resources Individually

When FHIR resources are uploaded one at a time—rather than as part of a transaction bundle—managing references between them requires extra care. This is because each resource is created independently, and the server assigns a unique identifier (usually in the form of a URL like `Patient/12345`) at the time of creation.

In this scenario, any resource that depends on another (e.g., an `Observation` that refers to a `Patient`) cannot use temporary or placeholder identifiers like `urn:uuid:...`. Instead, it must reference the actual, server-assigned identifier of the target resource.

## Why This Matters

1. **No Shared Context**  
   Unlike a transaction bundle, where temporary identifiers can be resolved internally during processing, individual uploads lack a shared context. The server has no way to interpret placeholder references.

2. **Accurate Linking**  
   To maintain correct relationships, dependent resources must be updated to reference the actual identifiers of the resources they depend on. For example, after uploading a `Patient` and receiving its ID (`Patient/12345`), any `Condition` or `Encounter` that refers to that patient must use this exact ID.

3. **Avoiding Broken References**  
   If references are not updated, the server will treat them as invalid or unresolved, leading to broken links between resources and potential data integrity issues.

4. **Sequential Workflow**  
   This approach requires a step-by-step process:
   - Upload the independent (referenced) resource first.
   - Capture the server-assigned identifier from the response.
   - Update the dependent resource to use this identifier in its reference fields.
   - Upload the updated dependent resource.
