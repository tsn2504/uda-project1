# Write-up Template

### Choose, and justify the appropriate resource option for deploying the app.
- App service is my choice (PaaS).

- In my opinion, the CMS software is rather straightforward, with its primary function being saving an article's information.

- PaaS is the ideal infrastructure for a CMS application. It can simply connect with Azure Active Directory because it supports all of the dependencies, is fairly simple to maintain, and does not require extensive setup time from scratch like virtual machines (IaaS).

### Analyze the appropriate resource option for deploying the app.
#### Cost
- Virtual machines: Depending on their size and configuration, virtual machines have a fixed cost. costly for simple applications like CMS.
- App Service: Based on usage, app services use a pay-as-you-go business model. Appropriate for small projects or applications with few users, like CMS.
#### Scalability
- Virtual machines: IT and Devops need to manually scale the VMs.
- App Service: Scalability is made simpler if I select App Service because it supports automated scaling when traffic hits a specific threshold.

#### Availability
- Virtual machines: These need more monitoring and upkeep. But when the manager has greater freedom and control, this is also the purpose of VMs in comparison to App Service.
- App Service: I think that App Service has strong availability due to its built-in load balancing and fault tolerance.

#### Workflow
- Virtual machines: Compared to the App Service, the installation will require a few additional steps since the virtual machine is an IaaS itself.
- App Service: With Azure Portal config, it's easier to setup and use.

### Assess app changes that would change your decision.
For improved scalability, availability, and cost control, it could be important to consider moving from Azure App Service to Virtual Machines (VMs) if my CMS Application grows to be a very large application with, for example, a million of users per day. Let me provide some examples to back up my assertion:

#### Cost
- App Service is not the most economical choice in circumstances with exceptionally heavy traffic. When managing large-scale applications, VMs can be more cost-effective and offer more flexibility in resource distribution.

#### Scalability
- I'll need an infrastructure that is highly scalable as my CMS expands to support millions of users per day. By adding more instances to handle greater traffic, I can scale horizontally with VMs. I have more control over scalability with VMs, and I can tailor it to the needs of my application. Due to this flexibility, I can effectively manage the increased demand.

#### Availability
- When paired with Azure Availability Sets or Availability Zones, VMs can offer more availability than the App Service. I can make sure that my application is available despite hardware failures or scheduled maintenance by spreading my VM instances across a number of fault domains and update domains.
#### Workflow
- Because VMs are IaaS (Infrastructure as a Service), I will have more control over the underlying infrastructure, including OS setup, networking, and load balancing. This improved control may require more setup and management procedures, such as installing virtual networks, load balancers, and monitoring tools.