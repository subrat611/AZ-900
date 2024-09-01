# Table of Content

| SNo. | Unit                                              |
| ---- | ------------------------------------------------- |
| 1.   | [[#Introduction to Microsoft Azure Fundamentals]] |
| 2.   | [[#Introduction to cloud computing]]              |
| 3.   | [[#What is Cloud Computing?]]                     |
| 4.   | [[#Describe the shared responsibility model]]     |
| 5.   | [[#Define Cloud Models]]                          |
| 6.   | [[#Describe the consumption-based model]]         |
| 7.   | [[#Knowledge Check]]                              |
# Introduction to Microsoft Azure Fundamentals

In this series, you’ll cover **cloud computing basics**, be **introduced to some of the core services** provided by Microsoft Azure, and will learn more about the **governance and compliance services** that you can use.
## What is Azure Fundamentals ?

Whether you're interested in compute, networking, or storage services; learning about cloud security best practices; or exploring governance and management options, think of Azure Fundamentals as your curated guide to Azure.

---
# Introduction to cloud computing
## Learning objectives

- Define cloud computing.
- Describe the shared responsibility model.
- Define cloud models, including public, private, and hybrid.
- Identify appropriate use cases for each cloud model.
- Describe the consumption-based model.
- Compare cloud pricing models.

---
# What is Cloud Computing?

- It is the delivery of computing services over the internet. (include common IT infrastructure such as virtual machines, storage, databases and networking)
- It also offers IoT, ML, AI.

---
# Describe the shared responsibility model

*What the mean of Shared responsibility model or How it impacts cloud computing*
#### Shared Responsibility Model

- The Responsibilities get shared between the **cloud provider** and the **consumer**.
- **Cloud Provider Responsible for:** Physical security, Power, cooling and network connectivity.
- **Consumer Responsible for:** Data, access security (meaning you only give access to those who need it) and the information stored in the cloud. (You wouldn’t want the cloud provider to be able to read your information).

>Then, for some things, the responsibility depends on the situation. If you’re using a cloud SQL database, the cloud provider would be responsible for maintaining the actual database. However, you’re still responsible for the data that gets ingested into the database. If you deployed a virtual machine and installed an SQL database on it, you’d be responsible for database patches and updates, as well as maintaining the data and information stored in the database.

Consumer are responsible for everything with an **on-premises datacenter**.

The **shared responsibility** model is heavily tied into the **cloud service types**

| Cloud Service Type                 |
| ---------------------------------- |
| Infrastructure as a service (IaaS) |
| Platform as a service (PaaS)       |
| Software as a service (SaaS)       |
- IaaS places the most responsibility on the consumer, with the cloud provider being responsible for the basics of physical security, power, and connectivity.
- SaaS places most of the responsibility with the cloud provider.
- PaaS, being a middle ground between IaaS and SaaS, rests somewhere in the middle and evenly distributes responsibility between the cloud provider and the consumer

![[shared-responsibility-b3829bfe.svg]]

When using a cloud provider, you’ll always be responsible for:
- The information and data stored in the cloud
- Devices that are allowed to connect to your cloud (cell phones, computers, and so on)
- The accounts and identities of the people, services, and devices within your organization

The cloud provider is always responsible for:
- The physical datacenter
- The physical network
- The physical hosts

Your service model will determine responsibility for things like:
- Operating systems
- Network controls
- Applications
- Identity and infrastructure

---
# Define Cloud Models

- It define the deployment type of cloud resources.
- Types: **Private**, **Public** and **Hybrid**
## Private Cloud

- A private cloud is, in some ways, the natural evolution from a corporate datacenter. 
- It’s a cloud (delivering IT services over the internet) that’s used by a single entity. 
- Private cloud provides much greater control for the company and its IT department.
## Public cloud

- A public cloud is built, controlled, and maintained by a third-party cloud provider. 
- With a public cloud, anyone that wants to purchase cloud services can access and use resources.
## Hybrid cloud

- A hybrid cloud is a computing environment that uses both public and private clouds in an inter-connected environment. 
- A hybrid cloud environment can be used to allow a private cloud to surge for increased, temporary demand by deploying public cloud resources.

|**Public cloud**|**Private cloud**|**Hybrid cloud**|
|---|---|---|
|No capital expenditures to scale up|Organizations have complete control over resources and security|Provides the most flexibility|
|Applications can be quickly provisioned and deprovisioned|Data is not collocated with other organizations’ data|Organizations determine where to run their applications|
|Organizations pay only for what they use|Hardware must be purchased for startup and maintenance|Organizations control security, compliance, or legal requirements|
|Organizations don’t have complete control over resources and security|Organizations are responsible for hardware maintenance and updates|
## Multi-cloud

A fourth, and increasingly likely scenario is a multi-cloud scenario. In a multi-cloud scenario, you use multiple public cloud providers. Maybe you use different features from different cloud providers. Or maybe you started your cloud journey with one provider and are in the process of migrating to a different provider.

## Azure Arc

Azure Arc is a set of technologies that helps manage your cloud environment. Azure Arc can help manage your cloud environment, whether it's a public cloud solely on Azure, a private cloud in your datacenter, a hybrid configuration, or even a multi-cloud environment running on multiple cloud providers at once.

## Azure VMware Solution

What if you’re already established with VMware in a private cloud environment but want to migrate to a public or hybrid cloud? Azure VMware Solution lets you run your VMware workloads in Azure with seamless integration and scalability.

---
# Describe the consumption-based model

Comparing IT infrastructure models, there are two types of expenses to consider
- **Capital Expenditure (CapEx)**
- **Operational Expenditure (OpEx)**

**CapEx** is typically a one-time, up-front expenditure to purchase or secure tangible resources.
Ex - A new building, repaving the parking lot, building a datacenter, or buying a company vehicle.

**OpEx** is spending money on services or products over time.
Ex - Renting a convention center, leasing a company vehicle, or signing up for cloud services.

**Cloud computing falls under OpEx because cloud computing operates on a consumption-based model**.
With cloud computing, you don’t pay for the physical infrastructure, the electricity, the security, or anything else associated with maintaining a datacenter. Instead, you pay for the IT resources you use. If you don’t use any IT resources this month, you don’t pay for any IT resources.

This consumption-based model has many benefits, including:

- No upfront costs.
- No need to purchase and manage costly infrastructure that users might not use to its fullest potential.
- The ability to pay for more resources when they're needed.
- The ability to stop paying for resources that are no longer needed.
## Compare cloud pricing models

You typically pay only for the cloud services you use, which helps you:
- Plan and manage your operating costs.
- Run your infrastructure more efficiently.
- Scale as your business needs change.

---
# Knowledge Check

1. What is cloud computing?
	Ans: Delivery of computing services over the internet.
	
2. Which cloud model uses some datacenters focused on providing cloud services to anyone that wants them, and some data centers that are focused on a single customer?
	Ans: Hybrid Cloud
	
3. According to the shared responsibility model, which cloud service type places the most responsibility on the customer?
	Ans: PaaS