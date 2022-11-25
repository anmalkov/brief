**Principle:** Integrity  
**Affected Asset:** All services  
**Threat:** Sending malicious or unnecessary traffic to Azure resources can lead to a compromise of that resource or create a vector for the attacker to bypass other security controls.

**Mitigation:**

Use and configure firewalls to protect against malicious incoming and outgoing network traffic.

1. Use Application Gateway before publicly accessible Azure Services and enable the Web App Firewall (WAF). By default, the WAF will use Azure-managed rules such as the OWASP ruleset. Custom rules should be defined if the default rules do not meet the customer’s needs.
2. Turn on DDoS protection feature.