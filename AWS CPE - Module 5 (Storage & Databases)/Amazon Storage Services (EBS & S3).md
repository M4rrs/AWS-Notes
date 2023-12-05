#AWS-piscine #AWS-Cloud-Practitioner-Essentials 

- [[#Instance Stores]]
- [[#Amazon Elastic Block Store (EBS)]]
- [[#Object Storage]]
- [[#Amazon Simple Storage Service (S3)]]
- [[#EBS vs S3]]

------
## Instance Stores
- **Block-level storage volumes** behave like physical hard drives.
- **Instance Store:** temporary block-level storage for an EC2.
- Physically attached to the host computer for an EC2.
- Same lifespan as the instance. When the instance is stopped, all stored data is deleted.

----------
## Amazon Elastic Block Store (EBS)
- Block-level storage for EC2.
- All data **persists** after instance is terminated.
- To create EBS: Define configuration (volume size and type) and provision.
##### EBS Snapshots
- Incremental backups
- After first backup, subsequent backups only save blocks of data that have changed.

![[Screenshot_2023-12-05_at_13.47.57.png]]

-------
## Object Storage
- Objects consist of **data, metadata,** and a **key**.

- **Block-level storage:** When modified, only the parts that were changed are updated.
- **Object-level storage:** When modified, the entire object is updated.

## Amazon Simple Storage Service (S3)
- **Object-level storage.**
- Objects stored as **Buckets**. Max obj file size is **5TB**
- Unlimited storage space.
- Features:
	- Set visibility and access permissions.
	- Versioning feature to track object changes.
- Factors in choosing a storage class:
	- How often you plan to retrieve data.
	- How available the data should be.
##### ==S3 Standard
- For frequently accessed data.
- Stores data in at least three Availability Zones.
- Extremely high availability (99.99%)
- Most expensive.
- Use cases:
	- Websites.
	- Content distribution.
	- Data analytics.
##### ==S3 Standard-Infrequent Access (S3 Standard-IA)
- For infrequently accessed data.
- Similar to **S3 Standard**, but **lower storage price** and **higher retrieval price**.
- Use cases:
	- Store backups.
	- Disaster recovery.
	- Objects requiring long term storage.
##### ==S3 One Zone-Infrequent Access (S3 One Zone-IA)
- Same as S3 Standard-IA but only one Availability Zone.
- Lower storage price.
- Suitable if:
	- Want to save costs.
	- Reproduce data easily in event of AZ failure.
##### ==S3 Intelligent-Tiering
- For data with unknown or changing access patterns.
- Small fees for monthly monitoring and automation.
- Uses machine learning to automatically move objects to different storage tiers based on access patterns.
##### ==S3 Glacier Instant Retrieval
- For archived data requiring immediate access.
- Retrieve data in milliseconds.
##### ==S3 Glacier Flexible Retrieval
- Low cost data archiving.
- Slow retrieval (1 minute to 12 hours)
- Use case:
	- Archived customer records.
	- Old photos or video files.
##### ==S3 Glacier Deep Archive
- Lowest cost data archiving.
- Very slow retrieval (12-48 hours)
- Long term retention, data might only be accessed once or twice a year.
##### ==S3 Outposts
- Creates S3 Buckets on S3 Outposts.
- Easier to retrieve, store, and access data on AWS Outposts.
- Delivers object storage to on-premises AWS Outposts.
- Ideal for workloads with data that must be kept close to on-premises applications.

------------
## EBS vs S3

| **==Elastic Block Store (EBS)==** | **==Simple Storage Services (S3)==** |
|--|--|
| Sizes up to 16TiB | Unlimited storage |
| Survives EC2 termination | Individual objects up to 5TBs |
| Default solid state | Write once/read many |
| HDD options | 99.99% durability |

- **S3:** Better for **complete objects** or **occasional changes**.
- **EBS:** Better for complex read/write/change functions.

------------
[[EFS, RDS, DynamoDB, Redshift|Next -> EFS, RDS, DynamoDB]]

