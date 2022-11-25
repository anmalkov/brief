**Principle:** Confidentiality and Integrity  
**Affected Asset:** All services  
**Threat:** A large attack surface, particularly those that are exposed on the internet, will increase the probability of a compromise.

**Mitigation:**

Minimize the application attack surface by limiting publicly exposed services.

1. Use strong network controls by using Azure Virtual Networks, Network Security Groups (NSG), or Private Endpoints to protect against unsolicited traffic.
2. Use Azure Private Endpoints to block all internet connections to services that do not need to be publicly exposed.
3. Turning on Azure Defender will provide a list of vulnerabilities associated with your subscription, it is advised to turn on this feature (free 30-day trial) to obtain a list of security measures and mitigate through that list.