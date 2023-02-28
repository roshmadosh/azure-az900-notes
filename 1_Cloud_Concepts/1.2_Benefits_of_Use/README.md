# Benefits of Using Cloud Services

**Summary**: Be able to describe the difference between the benefits of availability, scalability, reliability, predictability, governence/security, and manageability.

### Describe the benefits of high availability and scalability in the cloud
**High Availability**  
Cloud-hosted applications are expected to be highly available.     

Availability can be measured in percent-uptime. The higher the percent, the more it costs.  

Depending on the service, Azure has different uptime guarantees. These guarantees are defined in documents called _Service Level Agreements_ (SLAs) that are published [periodically](https://www.microsoft.com/licensing/docs/view/Service-Level-Agreements-SLA-for-Online-Services?lang=1).  

If they don't meet this guarantee, they offer a _service credit_ as a percentage of the fees paid for that service. For example, if the monthly uptime percentage of the basic Azure Active Directory service falls under 99.9% but above 99%, you get a 25% service credit.  

99% monthly uptime = 7.2 hours per month downtime  
99.9% monthly uptime = 43.2 minutes per month downtime 

**Scalablity**  
Scalability refers to how CSPs can adjust the resources used to meet demand. If there's a sudden surge in demand, Azure can manually or automatically provision more resources to meet the demand. If resources are not being fully utilized, Azure can also scale down to cut costs.  

There are two types of scaling: 
1. Vertical: Increase/decrease the computing power of a single virtual machine.  
2. Horizontal: Adding/removing virtual machines or containers to meet demand.  

### Describe the benefits of reliability and predictability in the cloud
**Reliability**  
Copies of your resources are deployed to various regions, meaning that if any single region goes down, your resources are still available.  

The term "resilient" is also used to describe this feature.  

**Predictability**  
Predictable performance and cost.  

- Performance: auto-scaling, load-balancing (i.e. distribute network traffic "evenly" so that no single resource is stressed), being highly available.
- Cost: Track expenditures in real time, apply data analytics to forecast and plan resource. Azure has a _Total Cost of Ownership_ (TCO) [calculator](https://azure.microsoft.com/en-us/pricing/tco/calculator/) for figuring out how much your resource deployments would cost.  

### Describe the benefits of security and governance in the cloud
Azure offers ways for users to more easily adhere to corporate and government regulatory standards, for example by notifying if a service is out of compliance, or perfoming automatic software updates.  

PaaS and SaaS services manage the security software updates for you, while IaaS allow users to manage it themselves.  

### Describe the benefits of manageability in the cloud
The "what" and "how" of managing cloud resources. The training module calls these "management of" vs "management in" as the what and how, respecitively.  

**What**
- Autoscaling
- Preconfigured templates
- Health monitoring
- Alerts on performance metrics

**How**
- web portal
- CLIs
- APIs 
- PowerShell

## Additional Reading  

- [Building great solutions with Microsoft Azure Well-Architected Framework](https://learn.microsoft.com/en-us/training/paths/azure-well-architected-framework/) (learning module)
