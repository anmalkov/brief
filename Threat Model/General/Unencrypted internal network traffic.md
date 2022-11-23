**Principle:** Confidentiality and Integrity  
**Affected Asset:** Internal network traffic  
**Threat:** Unencrypted network traffic within the tenant boundary may cause compliance issues if it contains sensitive data.

**Mitigation:**

Encrypt all communication channels using TLS.

---
**Thread ID:** 5  
**Principle:** Confidentiality and Integrity  
**Affected Asset:** All services  
**Threat:** A large attack surface, particularly those that are exposed on the internet, will increase the probability of a compromise.

**Mitigation:**

Minimize the application attack surface by limiting publicly exposed services.

- Use strong network controls by using Azure Virtual Networks, Network Security Groups (NSG), or Private Endpoints to protect against unsolicited traffic.
- Use Azure Private Endpoints to block all internet connections to services that do not need to be publicly exposed.
