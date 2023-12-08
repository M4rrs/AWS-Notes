#AWS-piscine #AWS-Cloud-Practitioner-Essentials #Module-9

- [[#AWS Snow Family]]
- [[#Innovation with AWS]]
----
## AWS Snow Family
- Physical devices that help to physically transport data into and out of AWS.
- Devices offer different capacity points, and mostly include built-on computing abilities.
##### ==AWS Snowcone
- Small, rugged, and secure edge computing and data transfer device.
- Shipped to you, plug it in and copy your data.
- Features:
	- 2CPUs
	- 4GB memory
	- 12TB usable storage.
##### ==AWS Snowball==
- Fits into existing server racks.
- Can be clustered for greater computing needs.
- Usually used by customers in remote areas where computing power is scarce.
- Use cases e.g. :
	- Capturing streams from IoT devices.
	- Image compression.
	- Video transcoding.
	- Industrial signaling.
###### Snowball Edge Storage Optimized
- Suited for large-scale data migrations and recurring transfer workflows + local computing with higher capacity needs.
- **Storage:**
	- 80TB hard disk drive (HDD) for block volumes and Amazon S3 compatible object storage.
	- 1TB SATA solid state drive (SSD) for block volumes.
- **Compute:**
	- 40 vCPUs
	- 80GiB of memory to support EC2 sbe1 instances.

###### Snowball Edge Compute Optimized
- Provides computing resources for cases e.g. :
	- Machine learning
	- Full motion video analysis
	- Analytics
	- Local computing stacks
- **Storage:**
	- 80TB usable HDD capacity for Amazon S3 compatible storage or EBS compatible block volumes.
	- 28TB usable NVMe SSD capacity for EBS compatible block volumes.
- **Compute:**
	- 104 vCPUs
	- 416GiB memory
	- optional NVIDIA Tesla V100 GPU
	- Devices run EC@ sbe-c and sbe-g instance (equivalent to C5, M5a, G3, P3 instances)
##### ==AWS Snowmobile
- Exabyte scale data transfer service to move large amounts of data to AWS.
- Transfer up to 100 petabytes of data per Snowmobile.
- Literally stored in a shipping container.

-----
## Innovation with AWS
- When using AWS, it's important to focus on desired outcomes.
- Articulate: What is the current state? The desired state? And what are the problems to be solved?
## Ways to innovate with AWS
##### ==Serverless Applications
- AWS handles managing and maintenance.
- Enables developers to focus on the core product instead of server management.
- E.g. : **AWS Lambda**
##### ==Artificial Intelligence
- E.g. :
	- Convert speech to text: **Amazon Transcribe**
	- Discover text patterns: **Amazon Comprehend**
	- Identify potential fraudulent activities: **Amazon Fraud Detector**
	- Build voice and text chatbots: **Amazon Lex**
##### ==Machine Learning
- Traditional ML is complex, expensive, time consuming and error prone.
- **Amazon Sagemaker:** removes the difficult work process.

---

