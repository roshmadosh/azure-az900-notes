### Describe directory services in Azure, including Microsoft Azure Active Directory (Azure AD), part of Microsoft Entra and Azure Active Directory Domain Services (Azure AD DS)

**Azure AD** is a cloud based directory service. It's used to control access to cloud resources, uses OAuth or SAML authentication.  

**Azure AD DS** is a domain service that allows the use of older authentication methods (Kerberos/NTLM) for legacy applications. A domain service is a way of organizing resources into units that have a delegated "admin" user.   

### Describe authentication methods in Azure, including single sign-on (SSO), multifactor authentication, and passwordless
SSO requires you provide a username and password just once, without having to reauthenticate each time you use a different service.  

MFA adds an additional requirement to a username and password, such as a security question, code sent to a mobile device, or biometric data like a fingerprint or face-scan.  

Passwordless authentication requires you register your device, and from there you just provide a PIN or fingerprint to be authenticated. Microsoft Authenticator app has both MFA and passwordless functionality. 

### Describe external identities and guest access in Azure
Consumers of your Microsoft resources don't have to be part of your organization, or even have MS accounts. They can use credentials from some other provider to authenticate themselves. The maintainer of the MS resources is still responsible for authorization, which can be managed through Azure AD.  

### Describe Conditional Access in Microsoft Azure Active Directory (Azure AD)
Through Azure AD, access can be granted or revoked based off signals like the user's identity, device, or location. Instead of outright blocking the user, you can also require the user provide an additional form of authentication (MFA).

### Describe Azure role-based access control (RBAC)
Instead of assigning the same permissions to users manually, you can create roles belie a collection of permissions and then assign that role to a _scope_. A scope can be a management group, subscription, resource group, or resource.  

### Describe the concept of Zero Trust
Authenticate every time. Give minimal permissions required. Deny by default.  

### Describe the purpose of the defense in depth model
A layered approach to security. Starting from the outermost layer:
- Physical: secure the hardware
- Identity & Access: always authentiate
- Perimeter: protect from DDoS attacks
- Network: inbound and outbound internet access should be limited
- Compute: VM's should be protected (e.g. require SSH)
- Application: remove security vulnerabilities within your application 
- Data: protect the database or disk storage

### Describe the purpose of Microsoft Defender for Cloud
Built-in for cloud services. Three components:
1. Continuously Assess: automatically run vulnerability scans
2. Secure: set security policies and follow compliance best practices through Azure Security Benchmark
3. Alerts: get notified, suggested remediation steps, option to trigger logic in response to an alert.