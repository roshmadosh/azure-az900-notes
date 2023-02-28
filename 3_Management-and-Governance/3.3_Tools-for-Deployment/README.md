### Describe the Azure portal
A GUI for managing your resources and deployments on Azure. You can create custom dashboards to focus on the services most important to you. Since they're present in every data center, they are highly resilient and available.  

### Describe Azure Cloud Shell, including Azure CLI and Azure PowerShell
**Cloud Shell** is a browser-based shell. You can access this shell from the Azure portal. Since you'll already be logged in from the portal, you won't have to authenticate yourself when doing stuff.  

Azure Cloud Shell provides two different interfaces: **Azure Powershell** and **Azure CLI** (bash-based). Besides the syntax, there's supposedly no significant difference between using Powershell and CLI.  

### Describe the purpose of Azure Arc
**Azure Arc** allows you to manage resources outside of Azure in one place, such as on-premises servers in a hybrid environment or resources from other Cloud providers in a multicloud environment.  

### Describe Azure Resource Manager and Azure Resource Manager templates (ARM templates)
**Azure Resource Manager** (ARM) is the API used for managing any and all resources, whether it's a request made from the portal, Azure Shell, or SDKs.  

**ARM templates** allow for infrastructure as code, where a single or collection of JSON files can declare how you want your resources deployed. This enables consistent deployments (i.e. if you had to deploy some resources more than once, you can be confident they're set up the same each time).  

