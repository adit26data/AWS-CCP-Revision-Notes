# Chapter 2

AWS Pricing and Billing Models

The main cost factors at AWS are: Compute, Storage and Outbound network traffic and data transfer.
The inbound data transfer/ traffic is free for all users. The AWS follows some core philosophies in its pricing model-

1.**PAY AS YOU GO PRICING:**
   You only pay for what you use, how much you use and how long you use the services. There is not additional upfront expense. This leads to econimical expenditure on the part of the client and there is reduced operational expenditure. Focus is on demand of the resources when needed.

2.**PAY LESS BY USING MORE:**
   We can realise the volume discounts of AWS in terms of tiered pricing and savings model. The volume discounts are economical in a nature and are cost controlling.

3.**PAY LESS AS AWS GROWS:**
    As the number of users increase the cost of a particular service decreases. As the services tools are enhanced, the faster high performing versions replace the current tools without extra charge as well.

4.**CUSTOM PRICING:**
    There is custom based pricing for specialised needs of the businesses as well

5.**AWS FREE TIER**:
   Beginner friendly pack for 1 year where multiple Amazon services are provided for free.

### Total Cost of Ownership
The traditional infrastructure of computing requires huge captial expense and needs the client to guess upfront all the requirements he or she needs. This makes it inflexible and less scalable. Unlike Cloud computing models, there is variable expense and the CSP is responsible for running and maintaining the services, will you are concerned only about using them for you applications and there is a provision of easy scalability and adaptablility. 
To evaluate the on premises expenditure and the same expenditure in cloud you need the TCO OR TOTAL COST OWNERSHIP.
TCO is basically a financial estimate of the helping in identifying the direct and indirect costs in a system. Used for budgeting and optimising the cost needs.
Considerations to be made are:
  1. **SERVER COSTS**- involves server administration costs, virtualisation costs, hardware costs and power, cooling and spacing costs.
  2. **NETWORKING COSTS**- involves load balancing, network adminstration and local area network setup costs
  3. **STORAGE COSTS**-involves the storage administration, disks and fibre channel switches.
  4. **IT LABOUR COSTS**- involves adminstration costs

#### AWS pricing calculator
Responsible for calculating and estimating the monthly costs, estimating the optimised lower costs and how we can reduce them. Explore the price points and determine the available instances that we might need in the future as well.

Addtional benefits to consider in TCO are:
1. **HARD BENEFITS**: reduction in expenditure of space and facility , procurement cycle of software and hardware resources and reduction in OpEx and administrative personnel.
2. **SOFT BENEFITS**: reuse of services along with increases developer productivity and agile business process and increased global reach

TCO takes in hard benefits as quantifiable physical benefits while soft benefits are value points that are not easily quantified.

### AWS ORGANISATIONS
Aws Organisation is a service to consolidate mutliple AWS accounts under one primary user/ organsational tree to consolidate the billing procedure and use organisational security features.
An OU is ORGANISATIONAL UNIT that has standard AWS account and only has one parent and belongs to one branch of the tree.
The key benefits are:
1. Group and Policy based account management policies
2. Automated account management using APIs
3. Consolidated billing
4. Service control policies and IAM roles and policies to control user access to services of Amazon.

The Setup involes:
1. Create an organisation with a primary account
2. Create OUs
3. Add accounts to the OUs
4. Create an SCP
5. Test the restictions using IAM simulator.

The Access is through- CLI , SDK, API and Management Console.

### AWS Billing and Cost Management
This is done using the AWS BILLING DASHBOARD that has the following tools-
#### 1. AWS Budgets: 
A service to pay bills, forecast expenditure, moditor usage and budget and recommend optimisation for costs of the services being used. Helps in viewing the data on monthly/daily level of granuality.
#### 2. AWS Cost and Usage Reports:
A service that helps in identifying the various techniques to optimise costs for various services being utilise by the account by analysing the usage trends.
#### 3. AWS Cost Explorer:
A part of the AWS Cost and Billing Management Console, it represents the costs of various AWS services for the last 3 months in visual format for report and analytics purpose. 
#### 4. AWS Bills Page:
List of all services that have been used by the linked account in the last 1 month.
#### 5. Spend Summary 
Shows the past expenditure and the forecasted budget with respect to all the services that are being used and can be used
#### 6. Month to Date Spend by Service
Shows the list of services in ration of the cost attributed to them over a certain period of time

### AWS Support Models
AWS provides 4 plans- BASIC, DEVELOPER, BUSINESS AND ENTERPRISE.

The **Support Conceirge** has the THE AWS TECHNICAL ACCOUNT MANAGER on proactive guidance on billing, finance issues, architechtual reviews and information of latest trends

The **AWS TRUSTED ADVISOR** is an automated service for recommending the best practices related to the billing and other aws aspects. Solves isses and checks for errors repeatedly.



  
