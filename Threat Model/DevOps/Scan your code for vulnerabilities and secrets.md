**Principle:** Confidentiality and Integrity  
**Affected Asset:** Code  
**Threat:** Your code might contain vulnerabilities and sensitive information.

**Mitigation:**

Use CI/CD pipeline to scan your code.

1. Add static code analysis tools in CI/CD pipelines to gain security insights about the code being developed, gate insecure code from entering production, and generate an overall more secure and complete solution. 
2. Add dependency and supply chain scanning to CI/CD pipelines to ensure you are using the most current and secure libraries.
3. Add credential scanning to CI/CD pipelines to ensure secrets, key information, and passwords are not leaked into the open.

