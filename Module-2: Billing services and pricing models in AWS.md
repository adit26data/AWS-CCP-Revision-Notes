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
As per Garter-Cloud computing services are intitally more expensive that the on premises ones, but become cost effective over period time with proper training and usage of the cloud resources.

#### AWS pricing calculator
Responsible for calculating and estimating the monthly costs, estimating the optimised lower costs and how we can reduce them. Explore the price points and determine the available instances that we might need in the future as well. It is a free tool and is used for helping in cloud migration
#### Migration Evaluator
A free service tool that extracts the data from your on premises resources to extract your AWS cloud cost in comparison to yout traditional on premises cost. Helps in cloud migration of a firm.

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
A service to pay bills, forecast expenditure, moditor usage and budget and recommend optimisation for costs of the services being used. Helps in viewing the data on monthly/daily level of granuality. It helps in with AWS Budgets reports to create usage and expenditure reports that can be categorised on multiple levels of granuality for the user convenience.
#### 2. AWS Cost and Usage Reports:
A service that helps in identifying the various techniques to optimise costs for various services being utilise by the account by analysing the usage trends. Generates the detailed spreadsheets that can be used by Athena and Quicksight for DB conversion and graphic visualisation.
#### 3. AWS Cost Explorer:
A part of the AWS Cost and Billing Management Console, it represents the costs of various AWS services for the last 3 months in visual format for report and analytics purpose. 
#### 4. AWS Bills Page:
List of all services that have been used by the linked account in the last 1 month.
#### 5. Spend Summary 
Shows the past expenditure and the forecasted budget with respect to all the services that are being used and can be used
#### 6. Month to Date Spend by Service
Shows the list of services in ration of the cost attributed to them over a certain period of time

### AWS Marketplace
Its a cureated digital catalogue of all the services being provided by various vendors on AWS platform You can deal and buy the services here for free or on a minimal associated charge. The charge becomes a part of AWS bill and once you pay that then the Marketplace pays the vendor. The platform is also meant for sale of services as well.

### AWS Support Models
AWS provides 4 plans- BASIC, DEVELOPER, BUSINESS AND ENTERPRISE.

The **Support Conceirge** has the THE AWS TECHNICAL ACCOUNT MANAGER on proactive guidance on billing, finance issues, architechtual reviews and information of latest trends. It helps on solving various technical issues, advocates for the customers, build solutions and ensures that the AWS environment remains operational and healthy. TAMs also collaborate with the developers for increased productivity and also understand the business needs and review any disruptions and metrics. They are available on the ENTERPRISE LEVEL ONLY.

The **AWS TRUSTED ADVISOR** is an automated service for recommending the best practices related to the billing and other aws aspects. Solves isses and checks for errors repeatedly.
There are five categories of the checklist supported by the TRUSTED ADVISOR:
1. Optimisation
2. Security
3. Performance
4. Fault Tolerance
5. Service Limits

The **AWS Partner Network** is basically a global partner program where organsatins open themselves for collaboration with AWS and to business oppoertunities including exclusive training and martketing events.

### Service Level Agreements
SLAS are formal committments made between the customer and the service provider regarding the expected service levels and if not met, the customer is entitled for compensation
### Service Level Indicators
SLIs are formal metrics that show the service levels that a customer is recieving in current time.
### Service Level Objective
The objectives that a provided service is to meet.
### Service Health Dashboard
Shows general status of the AWS services
### Personal Health Dashboard
provides guidance and alerts on AWS events that might harm the environment.
### AWS Abuse
The AWS Abuse team deals with attempts to damage the AWS environments like DDOS, DOS, intrustion, spamming and port scanning.

### Cost Allocation Tags
Optional metadata that when added to a service helps in better analysis of cost and usage tracking of that particular service.They are of 2 types- User and AWS defined.

### Billing Alarms
They are alerts to warn of over expense.










  
