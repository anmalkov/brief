**Principle:** Confidentiality and Integrity  
**Affected Asset:** All services  
**Threat:** Secrets leaking into unsecured locations are an easy way for adversaries to gain access to a system. These secrets can be used to either spoof the owners of these secrets or, in the case of encryption keys, use them to decrypt data.

**Mitigation:**

Proper storage and management of secrets is critical in protecting systems from compromises, in most cases, with severe impact.

1. Never store secrets in code, configuration files or databases. Instead, use a vault or any secure container (such as encrypted variables) to store secrets.
2. Separate application secrets by environment.
3. Rotate all secrets before turning over the application to the customer.

- Store all secrets, encryption keys and certificates in Key Vault.
- You can use multiple Key Vaults to separate secrets for different and critical services to minimize secrets leaking
- Define and implement secrets rotation strategy. All items in the vault should have expiration dates.
