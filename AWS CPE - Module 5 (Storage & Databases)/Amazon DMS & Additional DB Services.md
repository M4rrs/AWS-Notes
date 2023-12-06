#AWS-piscine #AWS-Cloud-Practitioner-Essentials 

- [[#AWS Database Migration Service (DMS)]]
- [[#Additional Database Services]]

-------
## AWS  Database Migration Service (DMS)
- Migrate relational databases, non-relational databases, and other data storage types.
- Data is moved between a **source database** and **target database.**
- Source and target can be same or different types.
- Database remains operational during migration, reducing downtime.
##### Other AWS DMS use cases
- **==Development and test database migrations==**:  To test applications against production data without affecting production users.
- **==Database consolidation==**: Combining multiple databases into one.
- **==Continuous replication==**:  Sending ongoing copies of data to target sources, instead of one-time migration.

------
## Additional Database Services

##### ==Amazon DocumentDB
- Document database service that supports MongoDB workloads.
- Suitable for:
	- Content management
	- Catalogs
	- User profiles
##### ==Amazon Neptune
- Graph database service
- Suitable for (highly connected datasets):
	- Social networking
	- Recommendation engines
	- Fraud detection
	- Knowledge graphs
##### ==Amazon Managed Blockchain
- Create and manage blockchain networks with open-source frameworks.
##### ==Amazon Quantum Ledger Database (QLDB)
- Ledger database service (stores accounting values)
- Can be used to review history of changes to your application data.
##### ==Amazon ElastiCache
- Adds caching layers on top of databases to improve read times of common requests.
- Supported data stores:
	- Memcached
	- Redis
##### ==Amazon DynamoDB Accelerator (DAX)
- In-memory cache for DynamoDB
- Improves response times from milliseconds to microseconds.

-------
