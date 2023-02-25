# Introduction to Cloud Computing


### Define cloud computing.
Computing services provided over the internet.

### Extra: Give examples of computing services.
1. Compute power: Pay for the amount of RAM and quality of processor.
2. Storage: Pay for how much disk space you use. Added bonus of easily replicating data across several servers. 

### Extra: Difference between RAM and processor.
RAM is the maximum "quantity" of work your computer can do at any given time. The processor is the speed at which you do the work.

### Extra: Why would I use a cloud service provider?
- Pay only for the services used. 
- Don't have to manage your own hardware resources.
- Scale or de-scale quickly.

### Describe the shared responsibility model.
The responsibilities of maintaining your cloud-hosted applications are shared between you and the cloud service provider.  

How those responsibilities are split depend on the service you use.  

The consumer will _always_ be responsible for the data you store, as well as who can access the data and on what kind of device (e.g. cell phone, computer, etc.).  

The CSP will _always_ be responsible for the physical data center, physical host (i.e. the computer itself, I think), and physical network.

_Infrastructure as a Service (IaaS)_ is a service giving minimal responsiblity to the CSP.  
_Software as a Service (SaaS)_ gives minimal responsiblity to the user.  
_Platform as a Service (PaaS)_ falls somewhere in between.  

### Extra: What responsibilities fall "in-between" a IaaS and SaaS?
1. Identity infrastructue management (e.g. if you use Azure Active Directory vs Auth0 for identity management)
2. Applications
3. Network controls (i.e. who can access your cloud-hosted resources on a network level)
4. Operating System (i.e. choosing the underlying OS, updating it, etc.)

### Extra: Is the Azure Virtual Machines (VM) service SaaS, PaaS, or IaaS?
IaaS because the user must update and secure the OS, manage network-level accessibility, provide any applications hosted on the VM, and specify how identity management will be provided.

### Define cloud models, including public, private, and hybrid.
Cloud models "define the deployment type of cloud resources." They're the "types" of clouds, where a cloud is just a collection of services provided via the internet. 

1. private: A private cloud is only used by a single organization. 
	- The data centers can be hosted on-site or by a third-party. 
	- You data isn't colocated with data from other orgs, which may be required (e.g. HIPAA).
	- More control but also more costly.
2. public: A cloud built, controlled, and maintained by a CSP.
	- Less control but cost advantages from economies of scale (i.e. hardware resources purchased in "bulk" by CSP, savings distributed to consumers)
3. hybrid: A cloud utilizing both private and public clouds.
	- Start with private cloud, then surges in demand can be handled by public cloud (because they're quicker to set up).

### Extra: What is multicloud?
Using multiple CSPs. You may want to use a mish-mash of services. Or you may be migrating from one CSP to another.  

### Compare cloud pricing models.
2 types:

1. Capital expenditure: Pay up-front, saves money if you know your costs ahead of time.
2. Operational expenditure: On-demand payment, can pay for more resources if needed and stop paying for resources that aren't used.

CSPs are OpEx.

