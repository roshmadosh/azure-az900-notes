### Compare compute types, including container instances, virtual machines (VMs), and functions
VMs require an OS to be "bundled" with it, so it takes longer to spin up than a container. Containers offer less control but are easier to scale than VMs because they're lighter weight. Azure functions are event-driven and a serverless compute service. They can be cheaper than VMs or containers because they don't need to be constantly up and running. You're only charged for when the Azure function has to respond to an event.  

### Describe VM options, including Azure Virtual Machines, Azure Virtual Machine Scale Sets, availability sets, and Azure Virtual Desktop

Azure VMs is an IaaS service that provides the ability to create virtual machines. 

**VM Scale Sets** allow for having multiple VMs that are configured the same, are load balanced, and are provisioned/de-provisioned according to demand (automatically or on a pre-configured schedule).   

**VM Availability Sets** are groupings of VMs to promote high availability. The two ways it groups VMs are by 
- update domain: Group VMs so that every VM in the group can reboot at the same time during an update without compromising availability. Only one update domain would be rebooted at a time.  
- fault domain: Group VMs so that each group has a separate power source and network switch. Protects against power and network failures.

**Azure Virtual Desktop** 
Hosts a Windows desktop on the cloud that's accessible across devices and OS's.  

- User login to this desktop can be managed from Azure AD.
- Supports multi-session windows 10 or 11 deployment, which regular VMs can't do.

### Describe application hosting options, including the Web Apps feature of Azure App Service, containers, and virtual machines
If you want to host a web application, web api, or mobile application, you can do so using VM's or containers.  

You can also use Azure App Service, which will come with the following things built in:
- continuous deployment from a Git repo
- secured endpoints
- auto-scaling
- load balancing
- supports multiple programming languages
  
### Describe virtual networking, including the purpose of Azure Virtual Networks, Azure virtual subnets, peering, Azure DNS, Azure VPN Gateway, and Azure ExpressRoute
Virtual networks are what allow your resources to communicate with each other, and to your on-premises servers.  

An **Azure Virtual Network** (Azure vNet) is one of the first things you have to create because other resources must assign themselves to a vNet. Each vNet is designated a bunch of IP addresses. 

Each vNet is specific to a region. If you need an application to be available across regions you need to create multiple vnNets.  

Azure virtual **subnets** are ways to split up your vNet. Each subnet has its own subset of IP addresses designated to it from the vNet. The resources you deploy, such as virtual machine, has to be assigned to a specific subnet.  

**VNet peering** and **Azure VPN Gateway** are means by which Azure vNets can communicate with each other. The latter can also connect an onsite vnet to an Azure vnet and encrypts messages passed between them.  

**Azure ExpressRoute** is a way to connect vnets without using the public internet. 

Vnets also allow you to filter network traffic using **security groups**. You can specify which IP addresses and protocols can access a subnet by configuring the security group it's assigned to.  

**Azure DNS** is a domain hosting service. It offers the benefits of 
- anycast networking: DNS queries are answered by the closest available DNS server.
- control who has access via Azure role-based access control
- logs to monitor modifications to a resource
- resource locking
- private DNS domains so you can come up with custom domain names in your VPNs

Azure DNS hosts domains for record management, **but you can't register a domain name using Azure DNS**. 

### Describe Virtual Private Networks (VPNs)
A VPN is an encrypted tunnel over within another network, usually an untrusted one like the internet. VPN Gateways are VPN implementations that come in two forms:
- policy-based
- route-based

Only a single VPN gateway can be deployed per VNet, but it can connect to multiple targets (i.e. other VNets, on-premises data centers).  

To maintain high availability, VPN gateways have several configuration options. By default, they are configured to be `active/standby` where two instances of VPN gateways are deployed, one that's active and another that's a "backup".

