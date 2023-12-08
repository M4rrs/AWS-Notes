#AWS-piscine #AWS-Cloud-Practitioner-Essentials #Module-7

- [[#Amazon CloudWatch]]
- [[#AWS CloudTrail]]
- [[#AWS Trusted Advisor]]

-----
## Amazon CloudWatch
- Web service to monitor and manage metrics and configure alarm actions based on metric data.
- Uses metrics to represent data points for resources.
- The metrics sent by AWS services are used to create performance graphs.
## CloudWatch Alarms
- Automatically perform actions if metric value goes above or below a predefined threshold.

----
## AWS CloudTrail
- API auditing tool.
- Records API call data.
- Updates within 15 minutes of an API call.
## CloudTrail Insights
- Optional feature allowing CloudTrail to automatically detect unusual API activities.

-----------
## AWS Trusted Advisor
- Web service that inspects your AWS environment and provides real-time recommendations.
- Compares findings to AWS best practice in terms of:
	- Cost optimization
	- Performance
	- Security
	- Fault tolerance
	- Service limits
## AWS Trusted Advisor Dashboard
- Accessible via Management Console

![[Screenshot_2023-12-06_at_19.16.30.png]]

- **Green check:** Number of items with no problems detected.
- **Orange triangle:** Number of recommended investigations.
- **Red circle:** Number of recommended actions.