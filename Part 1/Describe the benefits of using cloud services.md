# Table of Content

| SNo. | Unit                                                                         |
| ---- | ---------------------------------------------------------------------------- |
| 1.   | [[#Introduction]]                                                            |
| 2.   | [[#Describe the benefits of high availability and scalability in the cloud]] |
| 3.   | [[#Describe the benefits of reliability and predictability in the cloud]]    |
| 4.   | [[#Describe the benefits of security and governance in the cloud]]           |
| 5.   | [[#Describe the benefits of manageability in the cloud]]                     |
| 6.   | [[#Knowledge check]]                                                         |
# Introduction

You’ll be introduced to some of the **benefits that cloud computing offers**. You’ll learn **how** **cloud computing can help you meet variable demand** while providing a good experience for your customer. You’ll also learn about **security, governance, and overall manageability** in the cloud.
## Learning objectives

Upon completion of this module, you will be able to:

- Describe the benefits of high availability and scalability in the cloud.
- Describe the benefits of reliability and predictability in the cloud.
- Describe the benefits of security and governance in the cloud.
- Describe the benefits of manageability in the cloud.
# Describe the benefits of high availability and scalability in the cloud

Biggest Considerations on building or deploying a cloud application
- Uptime (or Availability)
- The ability to handle demand (or Scale)
## High Availability

- High availability focuses on ensuring maximum availability, regardless of disruptions or events that may occur.
- When you’re architecting your solution, you’ll need to account for service availability guarantees. Azure is a highly available cloud environment with uptime guarantees depending on the service. These guarantees are part of the **service-level agreements (SLAs).**
## Scalability

- **Scalability refers to the ability to adjust resources to meet demand.** If you suddenly experience peak traffic and your systems are overwhelmed, the ability to scale means you can add more resources to better handle the increased demand.
- **The other benefit of scalability is that you aren't overpaying for services**. Because the cloud is a consumption-based model, you only pay for what you use. If demand drops off, you can reduce your resources and thereby reduce your costs.

Scaling generally comes in two varieties: 
- **Vertical** -  Vertical scaling is focused on increasing or decreasing the capabilities of resources.
- **Horizontal** - Horizontal scaling is adding or subtracting the number of resources.
### Vertical Scaling

- With vertical scaling, if you were developing an app and you needed more processing power, you could vertically scale up to add more CPUs or RAM to the virtual machine. Conversely, if you realized you had over-specified the needs, you could vertically scale down by lowering the CPU or RAM specifications.
### Horizontal Scaling

- With horizontal scaling, if you suddenly experienced a steep jump in demand, your deployed resources could be scaled out (either automatically or manually). 
- For example, you could add additional virtual machines or containers, scaling out. In the same manner, if there was a significant drop in demand, deployed resources could be scaled in (either automatically or manually), scaling in.

----
# Describe the benefits of reliability and predictability in the cloud

Reliability and predictability are two crucial cloud benefits that help you develop solutions with confidence.
## Reliability

- Reliability is the ability of a system to recover from failures and continue to function. **It's also one of the pillars of the Microsoft Azure Well-Architected Framework.**
## Predictability

- Predictability in the cloud lets you move forward with confidence. Predictability can be focused on performance predictability or cost predictability. Both performance and cost predictability are heavily influenced by the **Microsoft Azure Well-Architected Framework.**
## Performance

Performance predictability focuses on predicting the resources needed to deliver a positive experience for your customers. Autoscaling, load balancing, and high availability are just some of the cloud concepts that support performance predictability. If you suddenly need more resources, autoscaling can deploy additional resources to meet the demand, and then scale back when the demand drops. Or if the traffic is heavily focused on one area, load balancing will help redirect some of the overload to less stressed areas.
## Cost

- Cost predictability is focused on predicting or forecasting the cost of the cloud spend. 
- With the cloud, you can track your resource use in real time, monitor resources to ensure that you’re using them in the most efficient way, and apply data analytics to find patterns and trends that help better plan resource deployments.
- By operating in the cloud and using cloud analytics and information, you can predict future costs and adjust your resources as needed. You can even use tools like the **Total Cost of Ownership (TCO) or Pricing Calculator** to get an estimate of potential cloud spend.

---
# Describe the benefits of security and governance in the cloud

Whether you’re deploying infrastructure as a service or software as a service, cloud features support governance and compliance.
- Set templates help ensure that all your deployed resources meet corporate standards and government regulatory requirements.
- Cloud-based auditing helps flag any resource that’s out of compliance with your corporate standards and provides mitigation strategies.

If you want patches and maintenance taken care of automatically, **platform as a service** or **software as a service** deployments may be the best cloud strategies for you.

---
# Describe the benefits of manageability in the cloud

 There are two types of manageability for cloud computing.
 - Management of the cloud
 - Management in the cloud
## Management of the cloud

Management of the cloud speaks to managing your cloud resources. In the cloud, you can:

- Automatically scale resource deployment based on need.
- Deploy resources based on a preconfigured template, removing the need for manual configuration.
- Monitor the health of resources and automatically replace failing resources.
- Receive automatic alerts based on configured metrics, so you’re aware of performance in real time.
## Management in the cloud

Management in the cloud speaks to how you’re able to manage your cloud environment and resources. You can manage these:

- Through a web portal.
- Using a command line interface.
- Using APIs.
- Using PowerShell.

---
# Knowledge check

1. Which type of scaling involves adding or removing resources (such as virtual machines or containers) to meet demand?
	Ans: Horizontal Scaling
	
2. What is characterized as the ability of a system to recover from failures and continue to function?
	Ans: Reliability