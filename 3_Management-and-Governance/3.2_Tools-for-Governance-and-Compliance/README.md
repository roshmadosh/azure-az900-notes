### Describe the purpose of Azure Blueprints
They're ways to define a template on the subscription or resource group level.  

Blueprints are composed of _artifacts_. Artifacts are like the attributes of a blueprint, and can be a policy assignment, role assignment, or Azure Resource Manager template (kind of like a YAML that defines how to create a resource).  

Blueprints can be versioned to keep track of updates made to the blueprint.  

### Describe the purpose of Azure Policy
Enables you to define individual policies or groups of policies, aka initiatives. They help track whether any of your resources don't comply to a policy, or prevent noncompliant resources from being created in the first place. Azure Policies can be set at the resource, resource group, subscription, or management group level, and are inherited.  

### Describe the purpose of resource locks
Resource locks are intended to prevent the accidental deletion or update of a resource. There are two types of locks:
1. prevents update but allow deletion
2. read-only, prevents update and deletion.  

Resource locks can be removed, and must be removed to permit the prohibited behavior.  

### Describe the purpose of the Service Trust Portal
Contains documents on Microsoft security, privacy, and compliance practices. You may have to review and accept a non-disclosure agreement to access certain compliance materials.  