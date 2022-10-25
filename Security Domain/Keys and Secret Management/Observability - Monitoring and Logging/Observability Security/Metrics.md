Azure [Monitor](https://www.cwcwiki.com/wiki/Monitor) Metrics is a feature of Azure Monitor that collects numeric data from monitored resources into a time series database. Metrics are numerical values that are collected at regular intervals and describe some aspect of a system at a particular time. Metrics in Azure Monitor are lightweight and capable of supporting near real-time scenarios making them particularly useful for alerting and fast detection of issues. You can analyze them interactively with metrics explorer, be proactively notified with an alert when a value crosses a threshold or visualize them in a workbook or dashboard.

### Best Practices

**Azure Monitor**

- Implement Azure Monitor Metrics to collects numeric data from monitored resources into a time series database.
- Integrate metrics collection from Azure Resources and Application Insights.
- Define [custom metrics](https://docs.microsoft.com/en-us/azure/azure-monitor/app/api-custom-events-metrics) in your application that's monitored by Application Insights or create custom metrics for an Azure service using the custom metrics API.
- Enable guest OS metrics for Windows virtual machines with [Windows Diagnostic  Extension](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/diagnostics-extension-overview) (WAD) and for Linux virtual machines with [InfluxData Telegraf Agent](https://www.influxdata.com/time-series-platform/telegraf/) to collect VM metrics.