## Chapter 7

### AWS Elastic Block Storage
It is a storage service that provides permanent block storage system to its users using EC2 instances. It provides SSD and HDD backed encrypted volumes that can be utilised for long term storage as well.
For EC2 instanes, normally SSD backed volumesa are chosen.
It has a pay for what you store per GB/Month model until you release the resources. 
It has 2 block storage kinds-
1. OBJECT STORAGE: cheaper and includes upadating everything for every change
2. BLOCK STORAGE: expensive and involves faster change of only the desired block where the change is demanded.

Scalable and Highly available in nature. We can also have snapshots for backups and creating new volumes in the future. The baseline snapshot is the first snapshot.

### AWS S3
It is an object storage service that stores data in form of S3 buckets that are logical containers for the objects storing data in encrypted manner across multiple facilities for data recovery and fault tolerance purposes.
Managed cloud service with 11 9's of durability and reliable and scalable in nature.The S3 buckets formed should be globally uniquely identified and have two types: path accessed and virtually accessed. Every bucket requires us to choose a region for it to store data.
Infinite storage is provided and has fine grained access using the IAM policies.
There are several classes to the S3:
1. Standard: High performance, High compliance and low laternt storage service for frequently accessed data
2. Standard IA: Highly performant, low latent and highly durable storage class for backups for infrequent accessed data
3. Standard Onezone IA: LOW COST storage service for secondary backups in one AZ
4. Intelligent Tiered: Optimised cost solution that moves objects to IA from standard to IA after 30 days of no access.
5. Glacier: Low cost solution for data archiving and long term backups of the infrequent accessed data
6. Glacier Deep Archive: Low cost solution for long term backups and data archiving.

### AWS EFS
Its a fully managed storage service that is beneficial for running analytical queries against petabytes of locally stored data in AWS. Implements storage that can be accessed by multiple ec2 instances over the cloud at once. Uses networked filed system for its implementation. Highly durable and scalable in nature.

### AWS S3 Glacier
It is a low cost storage solution by AWS for data archiving and long term backups of infrequently accessed data.. Provides 11 9's reliability and has encryption and vault-enforced access policy as well. It has 3 options for retrieval: expidited, standard and bulk.
The data retrieval is not immediate and takes time. 
Each vault has a vault access and vault lock policies.
Use cases involve: health data archiving, scientific data archiving, media asset archiving and digital preservation. Uses RESTful API and SDK(java and .NET) along with the CLI and console.


**When it comes to database services by AWS we have:**

### AWS RDS
AWS relational databse service is a fully cloud managed service that runs compatible MySQL/PostGreSQL/msSQL/Oracle/MariaDB in a cloud based environment woth automatic scaling.
This service is fast and simple to use as you have to only focus on cloud optimisation and not on other administrative access.
We also have database instances as the building blocks of the RDS and we can run several instances in this isolated environments.
We can configure RDS as-
1. run in VPC with a private subnet
2. generate standby copy of the db instance with synchronous replication in multiple AZ in the VPC for high availability feature
3. Read replicas for 6 engines where asynchronous replication is done.

Generally used for ecommerce apps, mobile apps and gaming apps where complex queries can be made and not simple PUT/GET requests. Should not be used in case of high sharded data and high read/write rates.
Clock hour billed pricing model.

### Amazon dynamoDB
A NoSQL service provided by the cloud with unlimited storage and low latency. Key value and file based DB. 

### Amazon RedShift
A CLASSIC AWS data warehousing service utilising SQL to run analytic queries against petabytes of data using columnar storage, parallel processing and query optimisation. The parallel processing is done using leader and compute nodes where the leader nodes assign the tasks to the compute nodes and integrate them on completion. Automates the management and monitoring of the nodes with strong encryption is also provided. Compatible with JDBC AND ODBC.

### Amazon Aurora
Enterprise class RDMS by AWS. MySQL/PostGreSQL compatible and mainly for automating time consuming tasks. Highly available, resilient, backed up, subsystem based and scalable in nature. Data is backed in S3.

