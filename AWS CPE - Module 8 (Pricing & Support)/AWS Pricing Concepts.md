#AWS-piscine #AWS-Cloud-Practitioner-Essentials 

- [[#AWS Free Tier]]
- AWS Pricing Concepts
	- [[#How AWS Pricing Works]]
	- [[#AWS Pricing Examples]]

---
## AWS Free Tier
- Enables you to use services without incurring costs for the specified period.
##### ==Always Free
- Never expire.
- e.g.
	- AWS Lambda allows **1 million** free requests and **3.2 million seconds** of compute time **per month.**
	- DynamoDB allows 25GB free storage per month.
##### ==12 Months Free
- Free for 12 months following initial sign-up date to AWS
- e.g. :
	- Specific amounts of S3 Standard.
	- Thresholds for monthly hours of EC2 compute time.
	- Amount of CloudFront data transfers out.
##### ==Trials
- e.g. :
	- Amazon Inspector: 90-day free trial.
	- **Amazon Lightsail** (Service for running virtual private servers): 750 hours over a 30-day period.

-----
## How AWS Pricing Works
###### ==Pay for what you use
- Pay for the resource you actually use, without requiring long-term contracts or complex licensing.
###### ==Pay less when you reserve
- Some services offer reservation options that provide a significant discount.
###### ==Pay less with volume-based discounts when you use more
- Some services offer tiered pricing. Per-unit cost decreases with increased usage.
- E.g. The more Amazon S3 storage space you use, the less you pay per GB.

----
## AWS Pricing Calculator
- Explore AWS services and create and estimate for the cost of your use cases.
- Estimations can be saved and shared.

## AWS Pricing Examples
##### ==AWS Lambda
- Charged based on number of requests for your functions, and time taken to run.
- Save costs by signing up for **Compute Savings Plan**.
- **Compute Savings Plan:** Lower compute costs in exchange for committing to a consistent usage over a 1-year or 3-year term.
##### ==Amazon EC2
- Charged based on compute time used while instances are running.
- Save with spot instances, savings plans, and reserved instances.
##### ==Amazon S3
- Cost components:
	- **Storage:** Charged based on storage used. Rates are based on objects' sizes, storage classes, and duration of stored object in that month.
	- **Requests & Data Retrieval:** Pay for requests made to S3 objects.
	- **Data Transfer:** No cost for transfers from S3 to other services within the same Region. However, charged for data transfers in and out of S3 with exceptions:
			- No cost for data transferred into S3 from the internet, or out to CloudFront.
			- No cost for transfers out to an EC2 in the same Region.
	- **Management & Replication:** Pay for enabled management features.

---------
## AWS Billing & Cost Management Dashboard
- Pay AWS bills.
- Monitor usage
- Analyze and control costs.