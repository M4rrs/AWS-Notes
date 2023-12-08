#AWS-piscine #AWS-Cloud-Practitioner-Essentials #Module-4

- [[#Subnets]]
- [[#VPC Network Traffic]]
- [[#Network ACLs]]
- [[#Security Groups]]
- [[#Stateless & Stateful Packet Filtering]]

---------------
## Subnets
- Sections of a VPC that you can group resources based on security or operational needs.
- Public and Private subnets can communicate with each other.
###### ==Public Subnets
- Resources are accessible to the public.
- e.g. Online store website.
###### ==Private Subnets
- Resources are only accessible through private networks.
- e.g. Database.

--------------

## VPC Network Traffic
- **Packet:** Unit of data sent over the internet or network.
- When a request is sent to the app in AWS Cloud, it is sent as a packet.

- **Network Access Control List:** Checks packet permissions for entering or exiting subnets.
## Network ACLs
- **Virtual Firewall** that controls inbound and outbound traffic at **subnet levels**.
- Performs ***Stateless Packet Filtering.***
###### ==Default Network ACL
- Allows all inbound and outbound traffic.
- Can modify to add your own rules.
###### ==Custom Network ACL
- Denies all inbound and outbound traffic.
- Must add rules to specify allowed traffic.
## Security Groups
- **Virtual Firewall** that controls inbound and outbound traffic for **EC2 Instances**
- Performs ***Stateful Packet Filtering.***
- By default:
	- Denies all inbound traffic
	- Allows all outbound traffic.
- Customize rules to configure allowed traffic; other traffic will be denied.

- Multiple EC2 Instances in a VPC can be associated in the same Security Group or use different Groups.

![[Screenshot_2023-12-04_at_16.58.36.png]]

-----------------------
## Stateless & Stateful Packet Filtering

| **==Stateless Packet Filtering==** | **==Stateful Packet Filtering==** |
|--|--|
| Performed by Network ACLs | Performed by Security Groups |
| Remember nothing and check packet permissions that cross subnets each way. | Remembers previous packet permissions for incoming packets.|

----
