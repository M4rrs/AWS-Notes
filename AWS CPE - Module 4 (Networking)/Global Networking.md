#AWS-piscine #AWS-Cloud-Practitioner-Essentials 

- [[#Domain Name System (DNS)]]
- [[#Amazon Route S3]]

-------
## Domain Name System (DNS)
- **DNS resolution:** Process of translating domain names to IP addresses.

![[Screenshot_2023-12-04_at_17.15.59.png]]

1) When you search a domain name, the request is sent to a DNS resolver.
2) The DNS resolver asks the DNS server for that domain IP address.
3) The server responds with the IP address.

-------
## Amazon Route S3
- A **DNS web service**.
- Connects users to running AWS infrastructure (EC2 or Load Balancers)
- More features:
	- Manages DNS records for domain names.
	- Can register new domains names.
	- Transfer records for existing domain names.
- Works together with [[Module 3 (Global Infrastructure & Reliability)#Edge Locations|Amazon CloudFront]].
##### ==e.g. Amazon Route 53 and Amazon CloudFront

![[Screenshot_2023-12-04_at_17.23.18.png]]

1) Customer requests application data from website.
2) **Route 53** uses DNS resolution to identify website IP address, send info back to customer.
3) Customer request is sent to the nearest **Edge Location** via **CloudFront**
4) **CloudFront** connects to the Application Load Balancer, which sends the incoming packet to an EC2.

------
