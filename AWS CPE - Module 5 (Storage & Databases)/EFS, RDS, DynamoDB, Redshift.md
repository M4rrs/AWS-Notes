#AWS-piscine #AWS-Cloud-Practitioner-Essentials 

- [[#File Storage]]
- [[#EBS vs EFS]]
- [[#Amazon Relational Database Service (RDS)]]
- [[#==Amazon Aurora|Amazon Aurora]]
- [[#Amazon DynamoDB]]
- [[#Amazon Redshift]]

---------
## File Storage
- Multiple clients can access data stored in shared file folders.
- The storage servers use block storage with a local file system.
- Data is accessed through file paths.

- Ideal for cases where large number of services and resources need to access the same data at the same time.
- **Amazon Elastic File System (EFS):** Scalable file system used with AWS services and on-premises resources.
- EFS scales up to petabytes.

## EBS vs EFS

| **==Amazon EBS==** | **==Amazon EFS==** |
|--|--|
| Stores data in **single** AZ | Stores data in and across **multiple** AZs |
| Both the AC2 and the EBS volume must reside in the same AZ | Duplicate storage enables access to data from all AZs in the Region the file is located.|
|| On-premises servers can access EFS via Amazon Direct Connect |

--------
## Relational Databases
- Data is stored such that it relates to other pieces of data.
- Uses **Structured Query Language (SQL)**.
## Amazon Relational Database Service (RDS)
- Automates tasks e.g. :
	- Hardware provisioning.
	- Database setup, patching, backups.
- Can be integrated with other AWS services.
- Security options:
	- Encryption at rest (protected while stored).
	- Encryption in transit.

## RDS Database Engines
- Supported engines:
	- **Amazon Aurora**
	- **PostgreSQL**
	- **MySQL**
	- **Oracle Database**
	- **Microsoft SQL Server**

##### ==Amazon Aurora
- Enterprise-class relational database.
- Compatible with MySQL and PostgreSQL
- Up to 5 times faster than MySQL, 3 times faster than PostgreSQL.
- Helps reduce database costs by reducing unnecessary I/O operations, while ensuring resources remain reliable and available.
- Continuously backs up data to S3.

----
## Non-relational Databases
- A.k.a. NoSQL Databases.
- Example of a non-relational DB: Key-value pairs.
	- Data is organized into items (key) and each item has attributes (value).
## Amazon DynamoDB
- Key-value database service.
- Delivers single-digit millisecond performance.
- **Features:**
	- Serverless
	- Automatic scaling

----

- **RDS:** Better for complex relational joins. E.g. Business analytics.
- **DynamoDB:** Simple and powerful database. E.g. Simple look-up tables.

----
## Amazon Redshift
- **Data Warehouse:** Larger relational database. Used for extremely complex and large queries.
- **Amazon Redshift:** Data warehousing service.

-------

[[Amazon DMS & Additional DB Services|Next -> Amazon DMS & Additional DB Services]]

