**Principle:** Integrity  
**Affected Asset:** All services  
**Threat:** Exploitation of insufficient logging and monitoring is the bedrock of nearly every major incident.
Attackers rely on the lack of monitoring and timely response to achieve their goals without being detected.

**Mitigation:**

Logging of critical application events must be performed to ensure that, should a security incident occur, incident response and root-cause analysis may be done. Steps must also be taken to ensure that logs are available and cannot be overwritten or destroyed through malicious or accidental occurrences.

At a minimum, the following events should be logged.

1. Login/logout events
2. Password change events (if not integrated into SSO)
3. Privilege delegation events
4. Security validation failures (e.g., input validation or authorization check failures)
5. Application errors and system events
6. Application and system startups and shutdowns, as well as logging initialization

- Implement a monitoring solution such as Azure Monitor or Log Analytics to monitor the web applications, security events, analytics, and workloads, respectively.
- If incident management is a concern of the customer, implement Microsoft Sentinel to act as the SIEM and make incident response more efficient.
- Use an alerting system to provide notifications when things need direct action.
- Install an Azure Monitor agent on critical VMs to allow ingestion of events into Azure Monitor.
