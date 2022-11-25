**Principle:** Integrity  
**Affected Asset:** All services  
**Threat:** Container images may contain unknown vulnerabilities, security issues and malicious applications.

**Mitigation:**

Only run containers from trusted registries. When using ACR, enable Azure Defender to scan your registry for security vulnerabilities on each pushed container image and expose detailed findings per image.


1. Use container scanning tools within your CI/CD pipelines to detect vulnerabilities earlier. 
2. Use Microsoft Defender for Containers to secure clusters, containers, and applications. Also scan your images for vulnerabilities with Microsoft Defender or any other image scanning solution.