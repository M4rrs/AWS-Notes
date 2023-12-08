#AWS-piscine #AWS-Cloud-Practitioner-Essentials #Module-6

- [[#AWS Shared Responsibility Model (Expanded)]]
- [[#AWS Identity and Access Management (IAM)]]

----
## AWS Shared Responsibility Model (Expanded)

[[Getting Started with AWS#AWS Shared Responsibility Model|Expanded from Getting Started with AWS]]
- Similar to dividing responsibilities between home***builder*** and home***owner***.
- AWS == builder: Responsible for construction of the infrastructure and environment.
- Customer == owner: Responsible for the security of the data in the environment.
##### ==Customers (Security IN the Cloud)
- Protects everything created and put *in* AWS Cloud.
- Manage security requirements for content:
	- What you want to store.
	- What services you use.
	- Access rights.
- Security steps depend on:
	- Services used
	- System complexity
	- Company operational and security needs
##### ==AWS (Security OF the Cloud)
- Protects the global infrastructure that runs all AWS services.
- Operates, manages, controls and **protects** all components of the infrastructure:
	- Hardware and software infrastructure.
	- Virtualization infrastructure
	- Physical security of the data centers
	- Network infrastructure

-------
## AWS Identity and Access Management (IAM)
- Manage access to AWS services and resources.
- Flexibility to configure access based on company operational and security needs.
- Features:
	- IAM users, groups, roles
	- IAM policies
	- Multi-factor authentication
## AWS Account Root User
- Access to all services and resources.
## IAM Users
- New user in AWS.
- By default has **no permissions.**
## IAM Policies
- Document that allows or denies permissions to AWS services and resources.
- Customize users' level of access to resources.
- *Best practice*:
	1) Principle of **least privilege** when granting permissions.
	2) Only give permission to what the user needs.
## IAM Groups
- Collection of IAM users. Pretty straightforward.
## IAM Roles
- Identity to gain **temporary** access to permissions.
- When assuming and IAM role:
	1) User must be granted permission for the role.
	2) Abandons all previous permissions under previous role.
	3) Takes up new permissions.
## Multi-factor Authentication (MFA)
- Extra layer of security for AWS account.

---------
