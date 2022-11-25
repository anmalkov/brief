**Principle:** Integrity  
**Affected Asset:** All services  
**Threat:** Container images may contain unknown vulnerabilities, security issues and malicious applications.

**Mitigation:**

Only run containers from trusted registries. When using ACR, enable Azure Defender to scan your registry for security vulnerabilities on each pushed container image and expose detailed findings per image.

Use container scanning tools within your CI/CD pipelines to detect vulnerabilities earlier. 