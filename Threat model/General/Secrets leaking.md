**Principle:** Confidentiality and Integrity  
**Affected Asset:** All services  
**Threat:** Secrets leaking into unsecured locations are an easy way for adversaries to gain access to a system. These secrets can be used to either spoof the owners of these secrets or, in the case of encryption keys, use them to decrypt data.

**Mitigation:**

Proper storage and management of secrets is critical in protecting systems from compromises, in most cases, with severe impact.

1. Never store secrets in code or configuration files. Instead, use a vault or any secure container (such as encrypted variables) to store secrets.
2. Separate application secrets by environment.
3. Rotate all secrets before turning over the application to the customer.