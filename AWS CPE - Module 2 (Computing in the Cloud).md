#AWS-piscine #AWS-Cloud-Practitioner-Essentials 
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

## EC2 Pricing

