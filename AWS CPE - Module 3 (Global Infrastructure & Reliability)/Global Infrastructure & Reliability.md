#AWS-piscine #AWS-Cloud-Practitioner-Essentials

- [[#AWS Regions]]
- [[#Availability Zones]]
- [[#Edge Locations]]
- [[#Amazon Outposts]]
- Resource Provision:
	- [[#Ways to interact with AWS Services]]
	- [[#AWS Elastic Beanstalk]]
	- [[#AWS CloudFormation]]

------------------------
## AWS Regions
- Regions are built closest to where business traffic demands.
- Regions are connect via high speed fiber network
#### Selecting Regions
###### ==Compliance with data governance & legal requirements
- Location-specific.
- e.g. If company data is required to reside in the UK, should choose the London Region.
###### ==Proximity to your customers
- Lower latency.
- Selecting a Region closer to customers will help get content to them faster.
###### ==Available Services in a Region
- Choosing a Region that offers the services you need, if the closest one to you does not.
###### ==Pricing
- Varying costs in different Regions.
## Availability Zones
- A single data center or group of data centers within a Region.
- Located miles away from each other but close enough for low latency.
- Distance minimizes chances of affecting other zones in a disaster.

![[Screenshot_2023-12-03_at_14.25.29.png]]

-----------
## Edge Locations
- **Edge Locations** are sites used by **Amazon CloudFront** to store caches copies of content closer to customers.
- If EC2 instance is running in a Region further away from customers, an Edge Location can help reduce the latency.

![[Screenshot_2023-12-03_at_14.38.59.png]]

## Amazon Outposts
- Fully operational **'mini Region'**, inside your own data center.
- Isolated within your own building.

-------
## Ways to interact with AWS Services
> [[Getting Started with AWS#Developer Tools|AWS Developer Tools]]
##### AWS Elastic Beanstalk
- Provisions resources and builds environment based on the application code and configurations that you provide.
- Saves environment configurations so they can be easily deployed again.
##### AWS CloudFormation
- Global content delivery service.
- **Infrastructure as code** tool.
- Define AWS resources using JSON or YAML documents (**CloudFormation Templates**).
- **Benefits:**
	- Provisions resources in safe, repeatable manner.
	- Frequently build infrastructure and apps without performing manual actions.
	- Determines operations to performs.
	- Rolls back changes when error is detected.

------------
