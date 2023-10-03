## Chapter 3

### AWS Global Infrastructure
This is a model that is designed to provide flexible, scalable, reliable and secure cloud computing environment to the end users and give high quality services with high global network performance. It is basically an interconnection of physical hardware and datacenters.
It is structured as:

1. **AWS REGIONS**
These are physical geographic locations that are isolated from each other and in turn have several AVAILABILITY ZONES
2. **AWS AVAILABILITY ZONES**
These are distinct phyiscal locations consisting of data centers that are secure undisclosed buildings having thousands of computers that reduce the latency during content distribution to end users.
Each AZ has several data centers. Each Region as 3 AZs to ensure high availability, fault tolerance and data redundancy in case of natural disasters as well. Each AZ acts as a fault domain that is basiclly a section of network where the systems are vulnerable to critical failures but the dameage is limited to that geographic region only.

While choosing an availability zone or a region one must take in considretion-
1. legal requirements
2. latency
3. services available in that region
4. Cost of the availed service

The presence of multiple availability zones doesnt ensure data replication as that is user controlled. When turned on, it ensures synchronous replication to all selected regions. Mission critical workloads are backed up across multiple regions for high availability and fault tolerance. Each location is chosen with minimal environmental risk at hand. 
Infrasturture benefits are:
1. Elasticity
2. Scalability
3. Fault Tolerance
4. High Availability

AWS global network that is a part of this infrastructure utilises the edge locations and regional edge caches for lowering the latency of the content delivery. Edge locations act as on/off ramps for AWS global network services for faster CDN.
Edge locations store caches of data that are very popular and can be immediately delivered to the end user on demand with low latency. The Regional Edge caches used by CLOUDFRONT stores the data that is infrequent and not so popular.

**Points of Presence**: They are intermediate locations between the AWS Region and the end users that support low latency and faster content delivery. They are basically edge locations and edge caches.They are used for expedited workloads.
Here for low latency we use a service called **AWS ACCELERATOR** that redirects traffic to edge locations instead of web servers directly. 
We also have wavelength zones and local zones.
Wavelength zones are regions that support edge computing over 5G networks with low latency and high performance. We can create a subnet and tie it with a wavelength zone  and deplot it to target 5G locations.
Local zones are basically regions of high population where data centers are located to provide services.

### Gov Cloud
GovCloud is basically a CSP that provides customised cloud computing environments and regions to run FedRamp workloads. FedRamp is a custom, isolated US based cloud service used for military and other governmental purposes.

### AWS ground station
A fully managed service that helps in controlling data satellite communication and processes and scales your data and operations without having to build the physical infrastructure of the work station. Used in weather forecasting, surface imaging etc.

### AWS Core services Overview
1. **STORAGE SERVICES**
   
    a. AWS SIMPLE STORAGE SERVICE OR AWS S3: elastic, scalable, secure and reliable storage service by AWS
   
    b. AWS ELASTIC BLOCK STORAGE OR AWS EBS: a fully managed, elastic, reliable and scalable block storage service used with EC2 instances for transactional workloads
   
    c. AWS ELASTIC FILE SYSTEM OR AWS EFS: A fully managed networked file storage system for the cloud.

    d. AWS S3 GLACIER: Storage class for data archiving and long term backup

2. **COMPUTE SERVICES**

    a. AWS ELASTIC COMPUTE OR AWS EC2: provides resizable compute capacity as VMs in the cloud

    b. AWS EC2 SCALING: provides the facilities of adding/removing the EC2 instances based on the needs

    c. AWS ELASTIC CONTAINER SERVICE OR AWS ECS: fully managed container orchestration service that stores, deploys and manages docker images

    d. AWS ELASTIC CONTAINER REGISTRY OR AWS ECR: fully managed service that acts as a container registry system for docker images

    e. AWS ELASTIC BEANSTALK: a web app hosting service and also for provisioning EC2 based environments.

    f. AWS LAMBDA: a serverless compute option that helps in running code without need to provision or manage servers

    g. AWS ELASTIC KUBERNETES SERVICE OR AWS EKS: container orchesteration service making use of kubernetes engine

    h. AWS FARGATE: an EC2 engine that supports containers without server and cluste management

3. **DATABASE SERVICES**

    a. AWS RDS : a fully automated, reliable and scalable RDBMS service on AWS

    b. AWS Aurora: a fully managed service supporting mysql and postgresql dbs

    c. AWS Redshift: a fully managed service that runs queries for analytics against petabytes of locally stored AWS data

    d. AWS dynamoDB: a fully elastic NoSQL db service for key-value and document type of storage with security, in memory caching and recoverability.

4. **NETWORKING SERVICES**

    a. Amazon VPN: service that helps in creation of private networks for business to increase their network experience and provide security

    b. Route 53: A DNS service that routes end users to internet applications making use of edge locations and translates the website domain names to registered ip addresses.

    c. Amazon VIRTUAL PRIVATE CONTAINERS OR VPCs: A fully managed service provisions isolated sections of the cloud to store resources and launch them in the virtual network

    d. AWS DIRECT CONNECT: Service that helps in creating a direct private tunnel between the data center and AWS to support better networking

    e. AWS ELASTIC LOAD BALANCER: A fully managed service that helps in traffic distribution

    f. AWS Cloudfront: secure content delivery service

    g. AWS TRANSIT GATEWAY: service that connects VPCs to on premises network using a primary managed gateway

5. **SECURITY SERVICES**

    a. AWS IAM: service that helps in access control to various AWS services from various accounts

    b. AWS Organisations: Helps in implementing similiar IAM policies to all the user accounts under a primary account and also helps in consolidated billing

    c. AWS Cognito: Add user authentication and authorization to web and mobile apps

    d. AWS Artifact: provides on demand AWS security and compliance reports and online agreements

    e. AWS KEY MANAGEMENT SYSEM OF AWS KMS: responsible for creation, management and security of encryption keys

    f. AWS Shield: safeguards AWS environment from DDOS attacks

6. **AWS COST MANAGEMENT SERVICES**

    a. AWS BUDGETS: an automated service that helps in billing process, tracking usage and monitoring costs associated to each service being used with analysis of past expenditure and forecasted budgets

    b. AWS COST EXPLORER: an automated service that helps in cost optimisation by helping in visual analysis and management of the AWS cost and usage.

    c. AWS COST AND USAGE REPORTS: helps in generating detailed analytical report on the past budgets, billing data and pricing and how we can lower the cost for the future

    d. AWS PRICING CALCULATOR:Responsible for calculating and estimating the monthly costs, estimating the optimised lower costs and how we can reduce them. Explore the price points and determine the available instances that we might need in the future as well. It is a free tool and is used for helping in cloud migration


7. **AWS GOVERANCE AND MANAGEMENT SERVICES**

   a. AWS Cloudwatch: helps in monitoring the services, their levels and the deployed applications

   b. AWS Config: service that helps tracking resources and inventory changes

   c. AWS Trusted Advisor

   d. AWS WAT: helps in reviewing the architectural tools and improve the workload

   e. AWS CloudTrail: tracks user activity and API usage across AWS accounts.

   f. AWS Outposts:AWS Outposts is a family of fully managed solutions delivering AWS infrastructure and services to virtually any on-premises or edge location. Basically server racks in the data centers are provided here that are fully managed by the AWS and are basically to provide virtual AWS infrastructure at your own building

   g. AWS CloudFormation: you can treat your infrastructure as code. This means that you can build an environment by writing lines of code instead of using the AWS Management Console to individually provision resources. AWS CloudFormation provisions your resources in a safe, repeatable manner, enabling you to frequently build your infrastructure and applications without having to perform manual actions. It determines the right operations to perform when managing your stack and rolls back changes automatically if it detects errors.
     
   

