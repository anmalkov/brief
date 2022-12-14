**Principle:** Confidentiality and Integrity  
**Affected Asset:** CI/CD Pipelines  
**Threat:** CI/CD Pipelines should always be cleansed of sensitive information being leaked.

**Mitigation:**

All secrets, key materials, and credentials stored in CI/CD Pipelines should always be cleansed of sensitive information that can be witnessed in plaintext.

1. Add pre-commit checks to ensure a secure pipeline cleansed of artifacts sensitive to the project.