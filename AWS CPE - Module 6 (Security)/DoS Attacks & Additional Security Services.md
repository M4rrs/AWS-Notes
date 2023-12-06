#AWS-piscine #AWS-Cloud-Practitioner-Essentials 

- [[#AWS Shield]]
- Additional Security Services
	- [[#AWS Key Management Service (AWS KMS)]]
	- [[#AWS WAF]]
	- [[#Amazon Inspector]]
	- [[#Amazon GuardDuty]]
------
## Denial-of-Service Attacks (DoS)
- Attempt to make a website or application unavailable to users,
- Attack originates from a **single** source.
## Distributed Denial-of-Service Attacks (DDoS)
- Attack from **multiple** sources.

## AWS Shield
- Protects applications against DDoS attacks.
##### ==AWS Shield Standard
- Automatically protects all AWS customers with no cost.
- Protects resources from most common DDoS attacks.
##### ==AWS Shield Advanced
- Paid service providing detailed attack diagnostics.
- Able to detect and mitigate sophisticated DDoS attacks.
- Integrated with services e.g. :
	- CloudFront
	- Route 53
	- Elastic Load Balancer
- Can be integrated with **AWS WAF** by writing custom rules to mitigate complex DDoS attacks.

------
## AWS Key Management Service (AWS KMS)
- **Cryptographic keys:** Random string of digits to encrypt and decrypt data.
- Perform encryption operations with ***cryptographic keys***.
- Create, manage, and use keys.
- Control use of keys across services and applications.
- Choose specific levels of access control.
	- Who can manage keys
	- Disable unused keys.
## AWS WAF
- **Web Application Firewall**
- Monitor network requests that come into your web-apps.
- Works with:
	- CloudFront
	- Application Load 
 - Similar to **Network ACLs**, but instead uses **==Web Access Control Lists (Web ACL)==**.
 - Allows access to requests unless the IP has been blocked.
## Amazon Inspector
- Performs automated security assessments.
- Provides a list of findings, prioritized by severity level + detailed description of the issue and recommendations to fix them.
- *However,* not guaranteed that the recommendations resolve all security issues.
## Amazon GuardDuty
- Provides intelligent threat detection for AWS infrastructure and resources.
- Continuously monitors network activity and account behavior.
- Analyzes data from multiple sources e.g. :
	- VPC Flow Logs
	- DNS Logs
- Provides detailed findings about detected threats.
- Includes remediation steps which can be automatically set in AWS Lambda.
- 
----
