# Table of Content

| SNo | Unit                                        |
| --- | ------------------------------------------- |
| 1.  | [[#Learning objectives]]                    |
| 2.  | [[#What does Azure offer?]]                 |
| 3.  | [[#Get started with Azure accounts]]        |
| 4.  | [[#Exercise - Explore the Learn sandbox]]   |
| 5.  | [[#Describe Azure physical infrastructure]] |
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
