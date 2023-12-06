#AWS-piscine #AWS-Cloud-Practitioner-Essentials

- [[#Amazon Elastic Compute Cloud (EC2)]]
- [[#EC2 Instance Types]]
- [[#EC2 Tenancy]]
- [[#EC2 Pricing]]
- [[#EC2 Auto Scaling]]

-----------
## Amazon Elastic Compute Cloud (EC2)

- **EC2** = AWS compute service that allows you to launch VMs, called instances.
- Only need to pay for *running* instances, not stopped or terminated instances.

- Multiple instances shared on a single host.
- The Hypervisor is responsible for **sharing the underlying physical resources** between VMs. 
	(**Multitenancy**)
#### Benefits of EC2

| ***Secure*** | Hypervisor is responsible for isolating the instances as they share resources. One EC2 is unaware of another EC2 on the same host. |
|--|--|
| ***Flexibility & Control*** | Choice of multiple instance types, OS, software packages, + configuration of memory, CPU, storage and partition size. |
| ***Elastic Scale Computing*** | Resizable instances (vertically scaling). |

------------------
## EC2 Instance Types

### General Purpose Instances
- **Balance** of compute, memory and networking resources.
- Use if app does not require optimization in single areas.
- Suitable for:
	- Application servers
	- Gaming Servers
	- Backend servers for enterprise apps
	- Small and medium databases
### Compute Optimized Instances
- Ideal for **compute-intensive** applications.
- Used when high processing power is needed.
- Similar use as General Purpose, but for high-performance.
### Memory Optimized Instances
- Used for workloads that process large datasets in memory.
- Suitable for:
	- High-performance Database
	- Workloads involving performing real-time processing large amounts of data.
### Accelerated Computing Instances
- Uses hardware accelerators or coprocessors to speed up data processing.
- e.g. :
	- Floating-point number calculations
	- Graphics processing
	- Data pattern matching
- Suitable for:
	- Graphic applications
	- Game streaming
	- Application streaming
### Storage Optimized Instances
- Ideal for **data-intensive** tasks.
- Used for workloads that require high read/write access to large datasets on local storage.
- e.g. :
	- Distributed file systems
	- Data warehousing applications
	- High-frequency online transaction processing (OLTP) systems

-------------
## EC2 Tenancy
- Allows for cost savings between customers.

| ***Shared (default)*** | Multiple AWS accounts on the same physical hardware. |
|--|--|
| ***Dedicated Instance*** | Instance runs on single-tenant hardware |
| ***Dedicated Hosts***| Instance runs on own physical server that you can control and configure |
## EC2 Pricing
##### ==On-Demand
- Only pay for the compute time you use.
- No upfront cost or minimum contracts.
- Ideal for short-term, irregular workloads that cannot be interrupted.
- e.g. :
	- Developing, testing, and running apps with unpredictable usage patterns.

##### ==Reserved Instances
- Billing discount applied to On-Demand Instances:
	- **Standard Reserved Instances**
	- **Convertible Reserved Instances**
- Can be purchased for a 1-year or 3-year purchase. Greater cost savings with 3 year option.
###### Standard Reserved Instances
- Suitable if you know the instance type, size needed, and Region planned to run.
- Required qualifications:
	- Instance type and size
	- Platform description (OS)
	- Tenancy: Default or Dedicated
- Can specify Availability Zone to reserve EC2 capacity.
###### Convertible Reserved Instances
- Suitable if running EC2 in different Availability Zones, or different EC2 types.
- Less discount rip.

##### ==EC2 Instance Savings Plans
- Provides discount when you make an hourly spend commitment to an instance family or Region for a 1-year or 3-year term.
- Up to 72% reduced rates.
- No need to specify qualifications like Reserved Instances.
##### ==Spot  Instances
- Ideal for workloads with flexible start and end times, or can withstand interruptions.
- Use unused EC2 capacity.
- Save costs up to 90% off On-Demand.
- Instance may be interrupted if capacity is unavailable.
##### ==Dedicated Hosts
- Physical servers with EC2 capacity fully dedicated to your use.
- Most expensive.
-------
## EC2 Auto Scaling
- **Scalability**: Designing architecture to **automatically respond to changing demand** by scaling in or out.
- **Amazon EC2 Auto Scaling**: Automatically adds or removes EC2 instances in response to changing demand.

| **Dynamic Scaling** | Responds to changing demand.|
|--|--|
| **Predictive Scaling** | Schedules right number of instances based on predicted demand.|

- Adds instances based on demand, decommissions instances when unneeded.

- Can set **minimum, desired,** and **maximum** capacity for your Auto Scaling group.

![[Screenshot_2023-12-02_at_18.34.09.png]]

--------
