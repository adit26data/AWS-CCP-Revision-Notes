## Chapter 3

### AWS global infrastructure
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

### AWS services Overview
1. **STORAGE SERVICES**
   
    a. AWS SIMPLE STORAGE SERVICE OR AWS S3: elastic, scalable, secure and reliable storage service by AWS
   
    b. AWS ELASTIC BLOCK STORAGE OR AWS EBS: a fully managed, elastic, reliable and scalable block storage service used with EC2 instances for transactional workloads
   
    c. AWS ELASTIC FILE SYSTEM OR AWS EFS: A fully managed networked file storage system for the cloud.

    d. AWS S3 GLACIER: Storage class for data archiving and long term backup

2. **COMPUTE SERVICES**

   
