Ensuring healthy network traffic to both user and application activity utilize management and monitoring tools to monitor your network's security. Most cloud monitoring tools are used to monitor, diagnose, view metrics, and enable or disable logs for resources in a cloud virtual networks.

### Best Practices

**Monitoring**

- Configure connection monitor capability monitors communication at a regular interval and informs you of reachability, latency, and network topology changes between the VM and the endpoint.
- Enable Network Performance Monitor which is a cloud-based hybrid network monitoring solution that helps you monitor network performance between various points in your network infrastructure. It also helps you monitor network connectivity to service and application endpoints and monitor the performance of Azure ExpressRoute.

**Diagnostics**

- When you deploy a VM, Azure applies several default security rules to the VM that allow or deny traffic to or from the VM. You might override Azure's default rules or create additional rules.
- Override Azure's default routes or create additional routes when you create a virtual network, Azure creates several default outbound routes for network traffic. The outbound traffic from all resources, such as VMs, deployed in a virtual network, are routed based on Azure's default routes.
- Configure [Security Group View Capability rules](https://docs.microsoft.com/en-us/azure/network-watcher/network-watcher-security-group-view-overview). This view shows you all security rules applied to the network interface, the subnet the network interface is in, and the aggregate of both. With an understanding of which rules are applied to a network interface, you can add, remove, or change rules, if they are allowing or denying traffic that you want to change.

**Metrics**

- Configure [Limits](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/azure-subscription-service-limits?toc=/azure/network-watcher/toc.json#azure-resource-manager-virtual-networking-limits) to the number of network resources that you can create within an Azure subscription and region. If you meet the limits, you are unable to create more resources within the subscription or region. The network subscription limit capability provides a summary of how many of each network resource you have deployed in a subscription and region, and what the limit is for the resource.

**Logs**

- Configure Network Security Groups (NSG) allow or deny inbound or outbound traffic to a network interface in a VM. The NSG flow log capability allows you to log the source and destination IP address, port, protocol, and whether traffic was allowed or denied by an NSG. You can analyze logs using a variety of tools, such as PowerBI and the Traffic Analytics Capability You should enable diagnostic logging for Azure networking resources such as network security groups, public IP addresses, load balancers, virtual network gateways, and application gateways. The Diagnostic logs capability provides a single interface to enable and disable network resource diagnostic logs for any existing network resource that generates a diagnostic log. You can view diagnostic logs using tools such as Microsoft Power BI and Azure Monitor logs. To learn more about analyzing Azure network diagnostic logs, see Azure Network Solutions in Azure Monitor logs.

**Automatic Enablement**

- When you create or update a virtual network in your subscription, Network Watcher will be enabled automatically in your Virtual Network's region. There is no impact on your resources or associated charge for automatically enabling Network Watcher. For more information, see Network Watcher Create.