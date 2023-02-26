### Describe Azure regions, region pairs, and sovereign regions

An **Azure region** is a geographical designation of several physical data centers. Some regions have **availability zones** which are themselves (smaller) geographical designations of one or more data centers. Each availability zone is able to run on its own, so that if one goes down, any data that's been replicated will still be available in another availability zone of the same region.  

**Region pairs** are two regions that, in the case of a natural disaster or some other occurrence that may affect an entire region, can compensate for the other when one goes down. Not all region pairs are two-way, some are one-way. Region pairs must be _at least_ 300 miles away from each other.  

**Sovereign regions** are Azure instances that are isolated from the "main" Azure instance, and are used for organizations that need to comply with certain regulations.  


### Describe Azure resources and resource groups
Resources are the "fundamental" unit in Azure. A VM instance is an Azure resource. Resource groups are collections of resources. 

- A resource must be part of a resource group
- A resource can _only_ be part of a single resource group
- Properties of the resource group get inherited by all the resources it contains
  
### Describe subscriptions
A way of organizing resources in terms of 
1. billing
2. access

Subscriptions can be comprised of multiple resouce groups, and any property assigned to a subscription will also be assigned to the resource groups.

### Describe management groups
Management groups have one or more subscriptions.

### Describe the hierarchy of resource groups, subscriptions, and management groups
In order of descending specificity:
resouce -> resouce group -> subscription -> management group
