# Table of Content

| SNo. | Unit                                      |
| ---- | ----------------------------------------- |
| 1.   | Introduction                              |
| 2.   | [[#Describe Infrastructure as a Service]] |
| 3.   | [[#Describe Platform as a Service]]       |
| 4.   | [[#Describe Software as a Service]]       |
| 5.   | [[#Knowledge Check]]                      |
# Introduction
## Learning objectives

After completing this module, you’ll be able to:

- Describe infrastructure as a service (IaaS).
- Describe platform as a service (PaaS).
- Describe software as a service (SaaS).
- Identify appropriate use cases for each cloud service (IaaS, PaaS, SaaS).
# Describe Infrastructure as a Service

- Infrastructure as a service (IaaS) is the most flexible category of cloud services, as it provides you the maximum amount of control for your cloud resources.
- In an IaaS model, the cloud provider is responsible for maintaining the hardware, network connectivity (to the internet), and physical security.
- You’re responsible for everything else: operating system installation, configuration, and maintenance; network configuration; database and storage configuration; and so on.
## Shared responsibility model

- IaaS places the largest share of responsibility with you. The cloud provider is responsible for maintaining the physical infrastructure and its access to the internet. You’re responsible for installation and configuration, patching and updates, and security.

![[shared-responsibility-b3829bfe (1) 1.svg]]

## Scenarios
- Lift-and-shift migration: You’re setting up cloud resources similar to your on-prem datacenter, and then simply moving the things running on-prem to running on the IaaS infrastructure.
- Testing and development: You have established configurations for development and test environments that you need to rapidly replicate. You can start up or shut down the different environments rapidly with an IaaS structure, while maintaining complete control.

---
# Describe Platform as a Service

- Platform as a service (PaaS) is a middle ground between renting space in a datacenter (infrastructure as a service) and paying for a complete and deployed solution (software as a service).
- In a PaaS environment, the cloud provider maintains the physical infrastructure, physical security, and connection to the internet. They also maintain the operating systems, middleware, development tools, and business intelligence services that make up a cloud solution.
- You don't have to worry about the licensing or patching for operating systems and databases.
## Shared responsibility model

- PaaS splits the responsibility between you and the cloud provider. The cloud provider is responsible for maintaining the physical infrastructure and its access to the internet, just like in IaaS. In the PaaS model, the cloud provider will also maintain the operating systems, databases, and development tools.
## Scenarios

- **Development framework**: PaaS provides a framework that developers can build upon to develop or customize cloud-based applications. Similar to the way you create an Excel macro, PaaS lets developers create applications using built-in software components. Cloud features such as scalability, high-availability, and multi-tenant capability are included, reducing the amount of coding that developers must do.
- **Analytics or business intelligence**: Tools provided as a service with PaaS allow organizations to analyze and mine their data, finding insights and patterns and predicting outcomes to improve forecasting, product design decisions, investment returns, and other business decisions.

---
# Describe Software as a Service

- Software as a service (SaaS) is the most complete cloud service model from a product perspective.
- With SaaS, you’re essentially renting or using a fully developed application. Email, financial software, messaging applications, and connectivity software are all common examples of a SaaS implementation.
## Shared responsibility model

SaaS is the model that places the most responsibility with the cloud provider and the least responsibility with the user. 
In a SaaS environment you’re responsible for the data that you put into the system, the devices that you allow to connect to the system, and the users that have access. 
Nearly everything else falls to the cloud provider. The cloud provider is responsible for physical security of the datacenters, power, network connectivity, and application development and patching.
## Scenarios

- Email and messaging.
- Business productivity applications.
- Finance and expense tracking.

---
# Knowledge Check

1. Which cloud service type is most suited to a lift and shift migration from an on-premises datacenter to a cloud deployment?
	Ans: IaaS
2. What type of cloud service type would a Finance and Expense tracking solution typically be in?
	Ans: 