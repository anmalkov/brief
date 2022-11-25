**Principle:** Confidentiality  
**Affected Asset:** All data stores  
**Threat:** Data is a valuable target for most threat actors and attacking the data store directly, as opposed to stealing it during transit, allows data exfiltration at a much larger scale.

**Mitigation:**

All customer or confidential data must be encrypted before being written to non-volatile storage media (encrypted at-rest) per the following requirements.

1. Use approved algorithms. This includes AES-256, AES-192, or AES-128.
2. Leverage SQL TDE whenever available.
3. Encryption must be enabled before writing data to storage.
4. Azure Storage, Cosmos DB, Azure SQL Database and Azure Database for MySQL encryption for data at rest is always on and uses AES-256.
5. Transparent Database Encryption (TDE) (to encrypt data at rest) with service managed keys are enabled by default for any Azure SQL databases.
6. Azure SQL Database backup data is automatically encrypted using Azure platform-managed keys.
7. If utilizing IaC products, ensure the configuration files are stored in a storage account or other safe location and not in your repository.