#AWS-piscine #AWS-Cloud-Practitioner-Essentials

- [[#Elastic Load Balancing (ELB)]]
- [[#Monolithic Applications & Microservices]]
- **Additional Compute Services**:
	- [[#AWS Lambda]]
## Elastic Load Balancing (ELB)
- Service that automatically distributes incoming application traffic across multiple resources (e.g. EC2 instances)
- All traffic (requests) are routed to the **load balancer** before being distributed to across the multiple instances.
##### Benefits of ELB

| **High Availability** | By distributing incoming traffic across multiple targets, if one target fails the load balancer automatically reroutes to healthy targets. |
|--|--|
| **Integration with other AWS Services** | e.g. Auto Scaling, CloudFormation, etc. |
| **Fault Tolerance** | By detecting unhealthy target instances and rerouting traffic away, preventing any failures. |

-----
## Monolithic Applications & Microservices

##### Monolithic Approach
- **Tightly Coupled Architecture** refers to components that directly communicate with each other in an application
-  If one component fails, the others fail too.
##### Microservices Approach
- **Loosely Coupled Architecture** refers to standalone components that interact with other components in an application.
-  If one fails, the rest can still communicate.

## Amazon Simple Notification Service (SNS)
- A publish/subscribe service.
- Via **Amazon SNS topics.** publisher publishes messages to subscribers.
- Subscribers can be **web-servers, email addresses, AWS Lambda functions** or other options.

## Amazon Simple Queue Service (SQS)
- Messaging queuing service.
- Send, store, and receive messages between components without losing messages or requiring other services to be available.
- Messages are sent into the queue, retrieved, processed, then deleted from the queue.

----

## Serverless Computing
- **Serverless** means code runs on servers, without needing to provision or manage the servers.
- Scales automatically.
- e.g. **AWS Lambda**

## AWS Lambda
- Pay for only the compute time used (when code runs).
- How Lambda works:
	1) Upload code to Lambda.
	2) Set code to trigger from event source (AWS services, apps, HTTP endpoints)
	3) Lambda runs code only when triggered.
	4) Pay only for compute time used.

## Containerized Applications
- **Containers** provide a standard way to package application code and dependencies into a single object.
- Also used for processes that require security, reliability, and scalability.
##### ==Amazon Elastic Container Service (Amazon ECS)
- Container management system for **Docker**.
##### ==Amazon Elastic Kubernetes Service (Amazon EKS)
- Container management system for **Kubernetes**.
##### ==AWS Fargate
- Serverless compute engine for containers.
- Works with both **ECS** & **EKS**