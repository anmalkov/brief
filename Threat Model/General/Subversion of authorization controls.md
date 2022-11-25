**Principle:** Confidentiality  
**Affected Asset:** All services  
**Threat:** Authorization controls could be subverted to allow an authenticated user/service to access unauthorized information. Worse, this weakness could be used to elevate privileges.

**Mitigation:**

Audit identities and their roles to determine least privileges.

1. Use Azure RBAC on services to segregate duties and grant only the least amount of access to perform an action at a particular scope.
2. Use Azure services role-based authorization feature.
3. Grant the appropriate permissions and roles to service principals.