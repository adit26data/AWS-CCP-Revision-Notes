## Chapter 6

### AWS COMPUTE SERVICES
AWS provides several resizable and secure compute services like AWS EC2, Fargate, Lambda, EKS, ECS, ECR, Lightsail, EC2 autoscaling, Elastic Beanstalk AWS Batch and AWS Outposts

AWS services of the compute type help in deploying several applications across the internet. 

### AWS EC2
1. AWS EC2 is a service that provides with resizable compute capacity for deploying and running various applications in the cloud in form of VMs. Basically the VMs are provisioned using this service and they can then run in the cloud computing environment.
2. We can use AWS launch instances and AMI ie AMAZON MACHINE IMAGES to create the instances and launch them and control the in bound and out bound traffic as well.
3. When creating instances we must consider 9 factors always-

   a. **AMI choice**
       There are several AMI to choose from as they are the templates on which the instance is formed. We have several types like - proeconfigured, customised, standard, Quickstart and myAMI.
   
   b. **Instance Selection**
       There are several instance types that can be used as per our needs. We can have combination of CPU, RAM , Storage etc. There are several types- compute optimised, storage optimised, memory optimised, generalised and accelerated computing.We can also have instances based on size ie. 2xlarge, large, medium, small and micro.
       The t3 instances are mainly for development and testing purposes.
       The c5 instances are for workload intensive tasks where high performance is needed. Eg: scientific modelling
       The r5 instances are used for memory intensive tasks where high performance is required. eg: data mining
       We can also create a cluster of instances and also set network performance levels. We can also try combinations for best performance and lower latency and lower jitter.

   c. **Network setting specification**
       We can set network configurations of our own including VPCs and subnets. We can choose which Region to deploy the instance in. If no chosen VPC, then default is assigned.

   d. **IAM Role Attachment**
        Since the instances access the various services across the AWS we can also attach IAM roles to each of the instances to control the service access.

   e. **Using Data Scripts**
       We can attach user data scripts to each instance to determine their run time environment at the launch level. This also helps in automatic installation and configuration of the instance launch, patching OS, firewall configurations and fetching and installing additional software.

   f. **Specifying the storage options**
      We can configure the volumes where the data is stored and the OS involed/installed. We can also attach additional volume blocks. The various storage options are: AaWS EFS, EBS, S3, EC2 store etc.

   g. **Tag addition**
      The addition of optional tag metadata helps in resource categorisation of the instances. The tags are added for a purpose or by the user differentiation.They usually have key and value pair. Like Name: Webserver as example.

   h. **Security Group Settings**
      We can create security groups of the various EC2 instances to control the network traffic. The outbound traffic is enabled by default and the inbound has to be specified explicitly. We can create rules and for traffic and allowable sources of communication.

   i. **identify/create key pairs**
     AWS EC2 instances use the public key cryptography system for encryption and decryption. This enables the secure connection when this key pair is made publicly available.

### AWS EC2 PRICING MODELS
We have various pricing models based on instance types:

1. on demand instances: for flexible and cheap workloads. Pay by the hour model of pricing. Mainly for spiky workloads as well.
2. spot instances: based on spot price and how long they are available. For dynamic and large scale workloads like big data, API backends etc.
3. reserved and scheduled reserved instances: for long term workloads, with 1-3 yr planned prices.
4. dedicated hosts and dedicated instances: compliance and regulatory requirements like license tracking. No upfront payment.

4 factors for cost optimisation in ec2 instances are:
1. size
2. storage choice
3. price model choice
4. instance choice and increased elasticity


### AWS CONTAINER SERVICES

Containers are basically virtualises OS to quicky deploy applications without in regard for the environment. The containers run virtualised OS as resource isolated processes and are faster to launch and terminate than the VMs. A VM runs on hypervisor while a container runs on OS if the docker daemon is present with the right configurations. An active container based deployment can have one EC2 instance running multiple containers.

#### AWS ELASTIC CONTAINER SERVICE
AWS ECS is a container orchestration service that supports docker images, their execution, their management and deployment with automated administration. The features are - EBS , Load Balancing, EC2 Sec groups and IAM rules. We can specify the number of tasks to be run on the AWS ECS as well and we can group them in form of clusters for their easy management. We can have container based deployment backed by  EC2 instances or by AWS Fargate.

#### AWS ELASTIC KUBERNETES SERVICE
AWS EKS is an open source kubernetes conformant service that supports docker images, their execution and storage and administration. Supports Kubernetes tools and other related popular add ons.

#### AWS ECR
AWS Elastic container registry is basically a registry service for maintaining, storing, deploying and executing docker images on a larger scale with access control, third party management, team collaboratin and ECS integration.

#### AWS Lambda
AWS Lamda is a serverless compute option that runs code without having to provision servers and clusters by the user. Supports multiple languages and has built in fault tolerance thanks to distributed functions. Has pay per use pricing. Usin g step function it can be used to create long running backend processes. Can be accessed by CLS, SDK and Lambda console. They are activated by the means of triggers. We can configure each lamda function for a variety of parameters. They are monitored using CloudWatch.

#### AWS Elastic Beanstalk
AWS Elastic Beanstalk is a fully managed hosting service for web apps with inbuilt provisioning, logging,load balancing, scaling, health checks, analysis and debugging abilities.  Fast and simple and development compatible service.

       
        


       
