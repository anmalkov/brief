**Principle:** Confidentiality  
**Affected Asset:** All services  
**Threat:** Broken or non-existent authentication mechanisms may allow attackers to gain access to confidential information.

**Mitigation:**

All services within the Azure Trust Boundary must authenticate all incoming requests, including requests coming from the same network. Proper authorizations should also be applied to prevent unnecessary privileges.

- Whenever available, use Azure Managed Identities to authenticate services. Service Principals may be used if Managed Identities are not supported.
- External users or services may use Username + Passwords, Tokens, or Certificates to authenticate, provided these are stored on Key Vault or any other vaulting solution.
- For authorization, use Azure RBAC to segregate duties and grant only the least amount of access to perform an action at a particular scope.
