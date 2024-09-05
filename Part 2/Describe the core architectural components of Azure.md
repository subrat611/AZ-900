# Table of Content

| SNo | Unit                                          |
| --- | --------------------------------------------- |
| 1.  | [[#Learning objectives]]                      |
| 2.  | [[#What does Azure offer?]]                   |
| 3.  | [[#Get started with Azure accounts]]          |
| 4.  | [[#Exercise - Explore the Learn sandbox]]     |
| 5.  | [[#Describe Azure physical infrastructure]]   |
| 6.  | [[#Describe Azure management infrastructure]] |
## Learning objectives

- Describe Azure regions, region pairs, and sovereign regions.
- Describe Availability Zones.
- Describe Azure datacenters.
- Describe Azure resources and Resource Groups.
- Describe subscriptions.
- Describe management groups.
- Describe the hierarchy of resource groups, subscriptions, and management groups.

---
# What does Azure offer?

**Limitless innovation.** Build intelligent apps and solutions with advanced technology, tools, and services to take your business to the next level. Seamlessly unify your technology to simplify platform management and to deliver innovations efficiently and securely on a trusted cloud.

- **Bring ideas to life:** Build on a trusted platform to advance your organization with industry-leading AI and cloud services.
- **Seamlessly unify:** Efficiently manage all your infrastructure, data, analytics, and AI solutions across an integrated platform.
- **Innovate on trust:** Rely on trusted technology from a partner who's dedicated to security and responsibility.

---
# Get started with Azure accounts

![[Pasted image 20240903005530.png]]

## What is the Azure free account?

The Azure free account includes:

- Free access to popular Azure products for 12 months.
- A credit to use for the first 30 days.
- Access to more than 25 products that are always free.
## What is the Microsoft Learn sandbox?

Sandbox, which creates a temporary subscription that's added to your Azure account. This temporary subscription allows you to create Azure resources during a Learn module. Learn automatically cleans up the temporary resources for you after you've completed the module.

---
# Exercise - Explore the Learn sandbox

Use the PowerShell Get-date command to get the current date and time.
```powershell
Get-date
```

Most Azure specific commands will start with the letters `az`.

```powershell
az version
```
## Use the BASH CLI

```powershell
bash
```
## Use Azure CLI interactive mode

- Another way to interact is using the Azure CLI interactive mode. 
- This changes CLI behavior to more closely resemble an integrated development environment (IDE). 
- Interactive mode provides autocompletion, command descriptions, and even examples.

```bash
az interactive
```

Once initialized, you can use the arrow keys or tab to help complete your commands. Interactive mode is set up specifically for Azure, so you don't need to enter `az` to start a command (but you can if you want to or are used to it).

```
version
```

```
upgrade
```

```
exit
```
## Use the Azure portal

---
# Describe Azure physical infrastructure

The core architectural components of Azure may be broken down into **two main groupings**:
- The physical infrastructure
- The management infrastructure.
## Physical infrastructure

- The physical infrastructure for Azure starts with datacenters. 
- Conceptually, the datacenters are the same as large corporate datacenters. They’re facilities with resources arranged in racks, with dedicated power, cooling, and networking infrastructure.
- As a global cloud provider, Azure has datacenters around the world. However, these individual datacenters aren’t directly accessible. 
- Datacenters are grouped into Azure Regions or Azure Availability Zones that are designed to help you achieve resiliency and reliability for your business-critical workloads.
### Regions

- A region is a geographical area on the planet that contains at least one, but potentially multiple datacenters that are nearby and networked together with a low-latency network.
- Azure intelligently assigns and controls the resources within each region to ensure workloads are appropriately balanced.

> Some services or virtual machine (VM) features are only available in certain regions, such as specific VM sizes or storage types. There are also some global Azure services that don't require you to select a particular region, such as Microsoft Entra ID, Azure Traffic Manager, and Azure DNS.
### Availability Zones

- Availability zones are physically separate datacenters within an Azure region.
- Each availability zone is made up of one or more datacenters equipped with independent power, cooling, and networking.
- An availability zone is set up to be an isolation boundary. If one zone goes down, the other continues working. Availability zones are connected through high-speed, private fiber-optic networks.

![[Pasted image 20240905214944.png]]

> To ensure resiliency, a minimum of **three separate availability zones** are present in all availability zone-enabled regions. However, not all Azure Regions currently support availability zones.

Availability zones are primarily for VMs, managed disks, load balancers, and SQL databases. Azure services that support availability zones fall into three categories:

- Zonal services: You pin the resource to a specific zone (for example, VMs, managed disks, IP addresses).
- Zone-redundant services: The platform replicates automatically across zones (for example, zone-redundant storage, SQL Database).
- Non-regional services: Services are always available from Azure geographies and are resilient to zone-wide outages as well as region-wide outages.
### Region pairs

Most Azure regions are paired with another region within the same geography (such as US, Europe, or Asia) at least 300 miles away. This approach allows for the replication of resources across a geography that helps reduce the likelihood of interruptions because of events such as natural disasters, civil unrest, power outages, or physical network outages that affect an entire region.

> Not all Azure services automatically replicate data or automatically fall back from a failed region to cross-replicate to another enabled region. In these scenarios, recovery and replication must be configured by the customer.

![[Pasted image 20240905224159.png]]

#### Additional advantages of region pairs

- If an extensive Azure outage occurs, one region out of every pair is prioritized to make sure at least one is restored as quickly as possible for applications hosted in that region pair.
- Planned Azure updates are rolled out to paired regions one region at a time to minimize downtime and risk of application outage.
- Data continues to reside within the same geography as its pair (except for Brazil South) for tax- and law-enforcement jurisdiction purposes.

> Most regions are paired in two directions, meaning they are the backup for the region that provides a backup for them (West US and East US back each other up). However, some regions, such as West India and Brazil South, are paired in only one direction. In a one-direction pairing, the Primary region does not provide backup for its secondary region. So, even though West India’s secondary region is South India, South India does not rely on West India. West India's secondary region is South India, but South India's secondary region is Central India. Brazil South is unique because it's paired with a region outside of its geography. Brazil South's secondary region is South Central US. The secondary region of South Central US isn't Brazil South.

### Sovereign Regions

Sovereign regions are instances of Azure that are isolated from the main instance of Azure. You may need to use a sovereign region for compliance or legal purposes.

Azure sovereign regions include:

- US DoD Central, US Gov Virginia, US Gov Iowa and more: These regions are physical and logical network-isolated instances of Azure for U.S. government agencies and partners. These datacenters are operated by screened U.S. personnel and include additional compliance certifications.
- China East, China North, and more: These regions are available through a unique partnership between Microsoft and 21Vianet, whereby Microsoft doesn't directly maintain the datacenters.

---

# Describe Azure management infrastructure

- The management infrastructure includes **Azure resources and resource groups, subscriptions, and accounts**. Understanding the hierarchical organization will help you plan your projects and products within Azure.
## Azure resources and resource groups

- A resource is the basic building block of Azure.
- Anything you create, provision, deploy, etc. is a resource. Virtual Machines (VMs), virtual networks, databases, cognitive services, etc. are all considered resources within Azure.

- Resource groups are simply groupings of resources. When you create a resource, you’re required to place it into a resource group. While a resource group can contain many resources, a single resource can only be in one resource group at a time.
- Some resources may be moved between resource groups, but when you move a resource to a new group, it will no longer be associated with the former group. Additionally, resource groups can't be nested, meaning you can’t put resource group B inside of resource group A.
## Azure subscriptions

![[Pasted image 20240905224649.png]]

- An Azure subscription links to an Azure account, which is an identity in Microsoft Entra ID or in a directory that Microsoft Entra ID trusts.
- An account can have multiple subscriptions, but it’s only required to have one.

There are two types of subscription boundaries that you can use:

- **Billing boundary**: This subscription type determines how an Azure account is billed for using Azure. You can create multiple subscriptions for different types of billing requirements. Azure generates separate billing reports and invoices for each subscription so that you can organize and manage costs.
- **Access control boundary**: Azure applies access-management policies at the subscription level, and you can create separate subscriptions to reflect different organizational structures. An example is that within a business, you have different departments to which you apply distinct Azure subscription policies. This billing model allows you to manage and control access to the resources that users provision with specific subscriptions.

 You organize subscriptions into containers called management groups and apply governance conditions to the management groups.
 
 ![[Pasted image 20240905224926.png]]

Some examples of how you could use management groups might be:
- Create a hierarchy that applies a policy.
- Provide user access to multiple subscriptions.

Important facts about management groups:

- 10,000 management groups can be supported in a single directory.
- A management group tree can support up to six levels of depth. This limit doesn't include the root level or the subscription level.
- Each management group and subscription can support only one parent.