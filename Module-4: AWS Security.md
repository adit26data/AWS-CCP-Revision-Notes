## Chapter 4

The CIA triad ie the confidentiality of data, integrity of the data, systems and the environment and availability of the services are key considerations to be made while planning the security of any IT infrastructure implementation. 
When it comes to AWS security , the shared responsibility model is followed
### SHARED RESPONSIBILITY MODEL
It states that some aspects of AWS are to be handled by Amazon and some aspects of security are to be handled by the customer. 
#### Security of the cloud: 
Means that the CSP is responsible for the physical security of datacenters, the services being provided, the edge locations and the availability zones. The CSP is focused in SECURING THE CLOUD.Responsible for logging, audititing, network intrustion detection and virtualisation infrastructure instance isolation.
#### Security in the cloud:
Means that the customer is responsible for what is deployed and stored in the cloud based environments and is accountable for encryption, configurations, OS , firewalls, network configurations, IAM policies,server and client safety , patching, maintainance and account management.

### AWS IDENTITY AND ACCESS MANAGEMENT SERVICE
AWS IAM is a service that helps in access control to various resources of the AWS by the the various users. It sets wo what resources/ services are available to who and what period of time. It is a global free service and uses policies.
It is used for authentication and authorisation of the accounts logging on the platform under one primary user as well.
4 major components are:
1. IAM USER: AWS authenticated user 
2. IAM ROLE: Temporary credentials given to the IAM user to access the service for a temporary period.
3. IAM GROUPS: A collection of similiar authenticated IAM users.
4. IAM POLICIES: JSON docs that specify what resources are accessed by which accounts. 2 types- Identity based and Resource based.Usually user independent in nature.

Authentication as an IAM user can be done by-

1.**Programmatic access**: Done using AWS CLI, SDK and access keys

2.**AWS management console** that uses 12 digit code, IAM username and password coupled with MFA to add an extra layer of security to the user accounts. 

### Securing new accounts on AWS
We can secure new accounts in various manners on AWS. The first identity always created is the root user. We must never use the root user account. Its usage should be limited to only changing the passwords, resetting IAM policies, changing account settings and updating support plans.
We must remove the root account access keys from the platform and store them somewhere else safely. We must create an IAM user account for ourself and create an IAM group to authorise under the root account. 
Also add MFA for both root account and the IAM accounts using hardware MFA, virtual MFA apps, U2F Encryption and MFA tools etc. 

You can also use CloudTrail for keeping track of the activities across all the accounts and also for monitoring the API usage. It has a 90 days retention policy and is disabled by default.User controlled in nature.
We should also enable billing reports to keep track of cost and usage associated with each service accessible by a particular amount.
Using AWS organisations helps in consolidated billing and also in easier centralised management of the IAM accounts and the policies over them. It helps in creation of SCP or server control policy.

#### SERVER CONTROL POLICY
   1. allows central control and limits permissons across various IAM accounts
   2. It sets the maximum permissions that can be given/set for an organisation
   3. It also ensures that the requirements and compliance guidelines are met by the user accounts.

### AWS KEY MANAGEMENT SERVICE
An AWS service that helps in creating and maintaining the encryption keys. It manages and monitors the key usage being done across the AWS accounts and using CloudTrail you can monitor across various IAM users. 
USER HSMs are validated using FIPS140-2 algorithm to protect the keys. The master keys can control all other keys and manipulate data and hence must be safeguarded. We can import keys of our own in the KMS as well.

### AWS COGNITO
An AWS service that adds signup, login , mfa and other authentication and authorisation mechanisms to web app and mobile apps. Scales to multiple users and meets majority of security compliance requirements.

### AWS Shield
A managed AWS DDOS protection service to keep AWS environments healthy. It also performs intrusion detection and has inline remediation strategies. Ensures minimum downtime and latency. If you are routing your traffic through route 53 service then you are definately using standard Shield. Can be coupled with a firewall for better protection

### AWS Inspector
A service for hardening your AWS environment by eliminating all possible risks. Runs specific security benchmarks against EC2 instances. CSI check has 699 checks!

### AWS Guard Duty
A service that continuously monitors the AWS environments for malware, unauthorised activities, vulnerabilities and other problems and alerts the user and provides suggestions for remedial actions.

### AWS Macie
A fully managed service that monitors S3 data access and looks for malware and suspicious activities and has various alerts for various threats. It is very user friendly and also provides alersts on inadverant data leaks. It is integrated with CloudFront in some cases as well.

**Both Guard Duty and Macie use ML to analyse the cloud trail logs, vpn logs, activities and other auditable information for their respective missions**

### AWS WEB APPLICATION FIREWALL
It is a protection tool to protect your web apps and mobile apps and blacklist the ips on the user choice. Attatched to cloudfront and load balancer usually.

### AWS CLOUD HSM
Hardware physical assets to store encrypted keys and passwords on memory rather than the disk. It is of single tenant type. Has option of backup, patching and high availability.


------------------------------------

We have 2 kinds of data in AWS-

**DATA AT REST**: secured using AES SHA256 algorithm that is used in creating an encrypted file system to store the data from outside attacks. We can use KMS integrated with this for key transparency.

**DATA IN TRANSIT**: We can secure the outbound/inbound data traffic using SSL / TLS open standard protocols. Using AWS Certified Manager, we can provide facility to manage,deploy and renew the TLS/SSL certificates. 

-------------------------------------
We can also secure the data stored in S3 buckets and control the access to the data using S3 Block policies, IAM , ACLS and AWS trusted advisor. 

------------------------------------

### Ensuring the compliance requirements are met
Customers are subjected to various compliance and security requirements and AWS engages in third party bodies and independent bodies to provide information about the policies of a region to a user.
AWS provides security features that meet the security compliance requirements of HIPAA, GDPR etc.

Using -
1. **AWS ARTIFACT**:
    Users have access to AWS compliance reports and documents on demand and also have access to online agreements. Can download a bunch of ISO certifications as well possessed by the AWS. The docs here can be used as guidelines for your own cloud environment as well. Also keeps tracks of business agreements, validates them, designates aws accounts to process legally restricted info when needed  and accept agreements on behalf of multiple accounts as well.

2. **AWS CONFIG**:
    Utilise to analyse, assess, audit and evaluate the AWS configurations and keep a history of all the modifications made. It simplifies all the compliance requirements to be met by the user and the AWS and also does security analysis.


    

