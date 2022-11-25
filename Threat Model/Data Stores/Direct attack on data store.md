**Principle:** Confidentiality  
**Affected Asset:** All data stores  
**Threat:** Data is a valuable target for most threat actors and attacking the data store directly, as opposed to stealing it during transit, allows data exfiltration at a much larger scale.

**Mitigation:**

All customer or confidential data must be encrypted before being written to non-volatile storage media (encrypted at-rest) per the following requirements.

1. Use approved algorithms. This includes AES-256, AES-192, or AES-128.
2. Leverage SQL TDE whenever available.
3. Encryption must be enabled before writing data to storage.
