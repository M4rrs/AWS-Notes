
#AWS-piscine 

- [[#What is Cloud Computing?]]
- [[#Advantages of Cloud Computing]]
- [[#Cloud Computing Service Models]]
- [[#AWS Global Infrastructure]]
- [[#Developer Tools]]
- [[#Infrastructure as Code (IaC)]]
- [[#AWS Shared Responsibility Model]]

--------
## What is Cloud Computing?

- On-demand delivery of compute power, storage, database, applications, and other IT resources through a cloud services platform (CSP).
- Delivery is done through internet with **pay-as-you-go pricing**.

- A CSP provides rapid access to flexible & low-cost IT resources to build & maintain software and databases, and create applications.
- No large investments on hardware needed, you can access as many resources as you need, and only pay for what is used.

- **"Undifferentiated heavy lifting of IT"**. Common, repetitive, time-consuming tasks are what AWS wants to help with.
## Advantages of AWS

| ***Pay-as-you-go*** | Pay only when you use computing resources, and how much is used. Trade CapEx for OpEx|
|----|----|
| ***Scalability*** | Access as much or as little capacity as needed, and scale as required.|
| ***Increase speed & agility*** | Instantly available resources. Increased agility because time and cost to experiment and develop is significantly lower.
| ***Cost Savings*** | Companies can focus more on business projects instead of maintaining data centers. More focus for customers instead of hardware.|
| ***Go global quickly*** | Deploy apps globally quickly and with lower latency. Better customer experience at minimal cost.|
| ***Benefit from massive economies of scale*** | **Larger scale == lower prices.** AWS aggregates usage from hundreds to thousands of customers leading to higher economies of scale. |

-----------
## Cloud Computing Service Models
* Each service provides different levels of abstraction, control, flexibility, & management.
##### IaaS (Infrastructure as a Service)
- Mainly to do with hardware.
- Typically provides access to networking features, computers (virtual or dedicated hardware) & data storage space.
- Highest level of flexibility and management control over resources.
- Most like existing IT resources, most familiar.
##### PaaS (Platform as a Service)
- Removes the need to manage underlying infrastructure (hardware & OS) and allows more focus on deployment and management of applications.
- Helps you be efficient because no need to worry abt resource procurement, capacity planning, maintenance, patching, etc.
##### SaaS (Software as a Service)
- Provides you with completed product that is run & managed by service provider.
- No need to worry about how its maintained or the underlying infrastructure; only about how you will **use** that software.

----------
## AWS Global Infrastructure
- AWS cloud infrastructure is built around AWS Regions and Availability Zones.
- **Regions:** Physical location with multiple availability zones.
- **Availability Zones:** One or more discreet data centers, with redundant power, networking & connectivity and housed in separate facilities.
- ^ offers the ability to operate applications and databases that are more highly available, fault tolerant, & scalable

[[Module 3 (Global Infrastructure & Reliability)|Expanded in Module 3]]

----
## Developer Tools
- When infrastructure becomes virtual, instead of physically managing it, you logically manage it.
- via AWS Application Programming Interface (AWS API)
##### AWS Management Console
- Web-based interface.
- Comprises of a broad collection of service consoles for managing AWS resources.
##### AWS CLI
- Can run in normal shell programs or;
- Using **AWS Cloudshell**: A browser based shell. Pre-authenticated with your console credentials.
- **Benefit of the CLI:** Can create single commands to create multiple AWS resources, reducing chances of human error when configuring resources.
##### IDE & Toolkits
- Pretty straight-forward.
##### Software Development Kits (SDK)
- Handy when you want to integrate application source code with AWS services.
- E.g. Using **Python SDK** to write code to store files in **Amazon Simple Storage Services (Amazon S3)** instead of on your local hard drive.
##### Access Keys
- Enables access to AWS resources outside the console.
- Can be deactivated and regenerated.

--------
## Infrastructure as Code (IaC)

##### AWS Cloud Development Kit (CDK)

- Framework for defining cloud infrastructure in code and provisioning it through **AWS CloudFormation**
- Uses the familiarity of programming languages for modelling your applications
- Provides high level components (constructs) that preconfigure cloud resources with proven defaults, to help build applications with ease.
- Provisions resources in a safe, repeatable manner via **AWS CloudFormation**
![[Screenshot_2023-12-01_at_14.55.32.png]]

##### AWS CloudFormation
- Helps model and set up AWS resources so you spend less time managing resources and more time focusing on applications.
- With CloudFormation, you create templates describing the resources you want (EC3 or RDS DB etc.). CloudFormation handles provisioning and configuration of the resources.
- Helps simplify infrastructure management, quickly replicates, and easily controls and tracks changes to infrastructure.
![[Screenshot_2023-12-01_at_14.56.06.png]]
---------------------
## AWS Shared Responsibility Model
[[Shared Responsibility Model & User Permissions|Expanded in Module 6]]
###### AWS
- Hardware/Global infrastructure
- Software for computing, storage, database, networking services.
###### Client
- Securing data via client/server encryption
- Configuration of virtual infrastructure and systems
- Configuration of managed services or third-party software.

![[Screenshot_2023-12-02_at_12.30.43.png]]

-----
