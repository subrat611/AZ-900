### Table of Content

| SNo. |                                                   |
| ---- | ------------------------------------------------- |
| 1.   | [[#Introduction to Microsoft Azure Fundamentals]] |
| 2.   | [[#Introduction to cloud computing]]              |
| 3.   | [[#What is Cloud Computing?]]                     |
| 4.   | [[#Describe the shared responsibility model]]     |
| 5.   | [[#Define Cloud Models]]                          |
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
