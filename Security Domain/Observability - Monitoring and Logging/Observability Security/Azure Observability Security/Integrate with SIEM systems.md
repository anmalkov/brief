Security Information and Event Management (SIEM) is a type of software that gathers log data and real-time event data generated from systems throughout an organization?s technology infrastructure and turns it into actionable information. Important uses of SIEM tools include alerting security staff about immediate security issues that need to be dealt with, and automated monitoring for compliance with important regulations such as HIPAA, PCI/DSS, and GDPR.

Among the systems that a SIEM solution collates data from are antivirus software, firewalls, host systems, database servers, web filters, network switches, and more. The SIEM tool takes all this information and aggregates it for a broad end-to-end view. The software then analyzes the aggregate data to find patterns and correlations and provide reports on security-related incidents and events.

### Best Practices

Below contain some SIEM Azure technologies that we recommend be implemented in your environment. Not all the recommended technologies should be adopted, only the solutions that work best for you and your customer.

**Azure Sentinel**

- Adopt [Azure Sentinel](https://docs.microsoft.com/en-us/azure/sentinel/tutorial-detect-threats-built-in) for a scalable, cloud-native, security information and event management (SIEM) and security orchestration automated response (SOAR) solution. Azure Sentinel provides intelligent security analytics and threat intelligence via alert detection, threat visibility, proactive hunting, and automated threat response.
- Increase the speed and scalability of your SIEM solution by using a cloud based SIEM.
- Find the most serious security vulnerabilities so you can prioritize investigation with [Azure secure score](https://docs.microsoft.com/en-us/azure/security-center/secure-score-security-controls) to see the recommendations resulting from the Azure policies and initiatives built into Azure Security Center.
- Connect [Azure Sentinel](https://docs.microsoft.com/en-us/azure/sentinel/connect-data-sources) to data sources.
- Continuously monitor with Azure Sentinel using Azure Sentinel integration with [Azure Monitor Workbooks](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/workbooks-overview).
- Implement notifications when something suspicious occurs by configuring Azure Sentinel