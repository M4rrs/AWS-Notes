#AWS-piscine #AWS-Cloud-Practitioner-Essentials #Module-10

- [[#AWS Well-Architected Framework]]
- [[#Benefits of AWS Cloud]]
-----
## AWS Well-Architected Framework
[[Module 1 (Intro to AWS)#AWS Well-Architected Framework||Expanded from Module 1]]
- Understand how to design and operate reliable, secure, efficient and cost-effective systems.
##### ==Operational Excellence
- Limit human error.
- Automate if possible.
- Design principles include:
	- Performing operations as code.
	- Annotating documentation.
	- Anticipating failure.
	- Frequently making small, reversible changes.
##### ==Security
- Best practices:
	- Automate security practices when possible.
	- Apply security at all layers.
	- Protect data in transit and rest.
##### ==Reliability
- Consistently and correctly perform operations.
- Ability of the system to:
	- Recover from infrastructure or service disruptions.
	- Dynamically acquire computing resources to meet demand.
	- Mitigate disruptions e.g. misconfigurations or transient network issues.
##### ==Performance Efficiency
- Evaluating performance efficiency includes:
	- Often experimenting.
	- Using serverless architectures.
	- Designing systems to be able to go global in minutes.
##### ==Cost Optimization
- Includes:
	- Adopting a consumption model.
	- Analyzing and attributing expenditure.
	- Using managed services to reduce ownership costs.
##### ==Sustainability
- The ability to continually improve sustainability impacts by reducing energy consumption and increasing efficiency across all workload components.
- Maximizing benefits of resources, minimizing total resources required.
- To facilitate good sustainability design:
	- Understand impact.
	- Establish goals.
	- Maximize utilization.
	- Anticipate and adopt more efficient hardware and software.
	- Use managed services.
	- Reduce downstream impact of your cloud workloads.

-----
## Benefits of AWS
[[Getting Started with AWS#Advantages of AWS|Explained in Getting Started with AWS]]
###### Scalability
- **Vertical Scaling:** Scaling up. Upgrading current server to have more resources. 
- **Horizontal Scaling:** Scaling out. Adding separate servers in addition to current servers.
###### Elasticity
- Ability to automatically increase or decrease resources based on tracked metrics.
###### High Durability
- Ability to recover from disaster with minimal loss.
- Strategies:
	- **Recovery Time Objective (RTO):** Maximum downtime that can be afforded without substantial loss.
	- **Recovery Point Objective (RPO):** Maximum amount of data that can be lost.