#AWS-piscine #AWS-Cloud-Practitioner-Essentials 

- [[#AWS Organizations]]
- Compliance:
	- [[#Compliance and Auditing]]
	- [[#Customer Compliance Center]]
-----
## AWS Organizations
- To consolidate and manage multiple AWS accounts in a central location.
- Features:
	- Centralized management of all accounts.
	- Group accounts into organizational units (OU).
##### Service Control Policies (SCPs)
- Can be applied to:
	- Organization root
	- Individual member accounts
	- OU
- Centrally control permissions for accounts in your OU.
- Can place restrictions on:
	- AWS services and resources
	- Individual API actions that users and roles can access
## Organizational Units (OU)
- Group accounts into OUs to manage accounts with similar business or security requirements.
- Easily isolate workloads or applications with specific security requirements.

---------
## Compliance and Auditing
- Depending on the industry, specific standards may need to be upheld.
- An audit or inspections ensures that said standards are met.
## AWS Artifact
- Provides on-demand access to AWS security and compliance reports and online agreements,
##### ==AWS Artifact Agreements
- Review, accept, and manage agreements for individual accounts and all accounts in an organization.
- Different types of agreements that address different customer regulations.
- e.g. Health Insurance Portability and Accountability Act (HIPPAA)
##### ==AWS Artifact Reports
- Provides compliance reports form third-party auditors.
- Auditors have tested and verified that AWS is compliant with global, regional. and industry specific security standards and regulations.
- Use example: If you team is building an app and requires information about their responsibility for complying with certain regulatory standards.

![[Screenshot_2023-12-06_at_15.12.09.png]]

-----
## Customer Compliance Center
- Contains resources to learn more about AWS compliance.
- Read customer compliance stories,
- Access compliance whitepapers and documentations e.g. :
	- AWS answers to key compliance questions
	- AWS risk and compliance overview
	- Auditing security checklist.
- Includes an auditor learning path.

------
