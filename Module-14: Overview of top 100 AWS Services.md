# Chapter 14: top 100 services are:


**1.AWS IDENTITY AND ACCESS MANAGEMENT SERVICE**

AWS IAM is a service that helps in access control to various resources of the AWS by the the various users. It sets wo what resources/ services are available to who and what period of time. It is a global free service and uses policies. It is used for authentication and authorisation of the accounts logging on the platform under one primary user as well.

**2.AWS KEY MANAGEMENT SERVICE**

An AWS service that helps in creating and maintaining the encryption keys. It manages and monitors the key usage being done across the AWS accounts and using CloudTrail you can monitor across various IAM users. USER HSMs are validated using FIPS140-2 algorithm to protect the keys. The master keys can control all other keys and manipulate data and hence must be safeguarded. We can import keys of our own in the KMS as well.

**3.AWS COGNITO**

An AWS service that adds signup, login , mfa and other authentication and authorisation mechanisms to web app and mobile apps. Scales to multiple users and meets majority of security compliance requirements.

**4.AWS Shield**

A managed AWS DDOS protection service to keep AWS environments healthy. It also performs intrusion detection and has inline remediation strategies. Ensures minimum downtime and latency. If you are routing your traffic through route 53 service then you are definately using standard Shield. Can be coupled with a firewall for better protection

**5.AWS Inspector**

A service for hardening your AWS environment by eliminating all possible risks. Runs specific security benchmarks against EC2 instances. CSI check has 699 checks!

**6.AWS Guard Duty**

A service that continuously monitors the AWS environments for malware, unauthorised activities, vulnerabilities and other problems and alerts the user and provides suggestions for remedial actions.

**7.AWS Macie**

A fully managed service that monitors S3 data access and looks for malware and suspicious activities and has various alerts for various threats. It is very user friendly and also provides alersts on inadverant data leaks. It is integrated with CloudFront in some cases as well.

**Both Guard Duty and Macie use ML to analyse the cloud trail logs, vpn logs, activities and other auditable information for their respective missions**

**8.AWS WEB APPLICATION FIREWALL**

It is a protection tool to protect your web apps and mobile apps and blacklist the ips on the user choice. Attatched to cloudfront and load balancer usually.

**9.AWS CLOUD HSM**

Hardware physical assets to store encrypted keys and passwords on memory rather than the disk. It is of single tenant type. Has option of backup, patching and high availability.

**10.AWS ARTIFACT:**

Users have access to AWS compliance reports and documents on demand and also have access to online agreements. Can download a bunch of ISO certifications as well possessed by the AWS. The docs here can be used as guidelines for your own cloud environment as well. Also keeps tracks of business agreements, validates them, designates aws accounts to process legally restricted info when needed and accept agreements on behalf of multiple accounts as well.

**11.AWS CONFIG:**

Utilise to analyse, assess, audit and evaluate the AWS configurations and keep a history of all the modifications made. It simplifies all the compliance requirements to be met by the user and the AWS and also does security analysis.