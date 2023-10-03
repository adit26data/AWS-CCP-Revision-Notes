## Chapter 5

### Amazon VPC
Amazon Virtual Private Cloud is basically a service that helps in provisioning logically isolated section of the AWS cloud where you can deploy your resources and run them in a virtual private network that you can define. This gives you control over the range of ip addresses selected, networking configurations, subnet creation and configuration of network gateways.
It helps in creating subnets under a AZ that can have private and public nature. 
VPC is basically Virtual Private Cloud that is user controlled and defined. The ipv4 and ipv6 addresses supported here help in communication between the VPC instance and also over the internet. VPCs result in assigning of a CIDR block that has 5 reserved addresses out of the selected range.They are reserved for-

1. Network broadcast address
2. Network address
3. internal communication
4. DNS resolution
5. future use

When we create a VPC we create a public ip address that is assigned to the CIDR block by the means of an elastic ip address. The elastic ip address is a static ipv4 address attatched to every AWS account that can remapped anytime. It masks the failures of the VPC instances by remapping it immediately to another instance. 
The largest ip address is of subnet /16 and smallest is /28.

### Elastic Network Gateway
These are easily detachable/attachable network interfaces related to a VPC instance. When a network gateway is moved from one instance to another the attributes are also shifted from one instance to another and diversion of traffic also happens. Each VPC instance has a default gateway where ipv4 addresses are stored and created initially.

### Route Table
A set of rules that you can configure your network with to direct network traffic to your subnet. Every Route has a target.
By default it has only the targets of internal communication in your VPC. You have to add additional ipv4 addresses manually. Each Subnet created must be assigned to at most 1 route table only.

### VPC Networking
Internet gateway is a scalable redundant and highly available VPC component that helps in communication of private VPC instances with the public network. It provides a target for yout VPC route table for internet traffic that is directed to your subnet. To make a subnet public , attach a route table to it and a route entry to be associated with the subnet to the internet gateway. Using NAT we specify the public subnet to which the NAT gateway will live and then specify elastic ip addresses and then update the route tables and security tables for the same.

### VPC Sharing
Allows multiple accounts under one organisation to share their subnets and create centralised VPCs to run their applications and store their application resources.

### VPC Peering
Connect VPCs between different accounts and regions.The restrictions are:-
 1. No ip overlap
 2. no transistive peering
 3. one resource per peering connection only for sharing

### AWS SITE TO SITE VPN
By default the VPC instance cannot communicate with your own remote private network. To do so, we use a VPN to create a custom user network gateway and update the route and security tables.

### Amazon Direct Connect
It helps in connecting datacenters privately to AWS regions and provide a better networking experience.

### VPC Endpoints
We need to connect the VPC resources to their target regional services and for that we need VPC Enfpoints that is used to connect privately to them. They are of 2 types- Gateways and Interfaces.

### AWS Transit Gateway
A fully Managed AWS TRANSIT HUB where we can connect multiple VPCs together and connect on premises networks as well. The topology is a hub here and performance depends on the number of connections.

------------------------
When it comes to VPC security you can use-
1. Network ACLs- These are created at the subnet level and have a one to one relation with them. Specify ports and protocols. Either a custom or a default ACL is used for a VPC instance.
2. Firewalls- virtual firewalls at instance levels. Control outbound and inbound traffic. By default the security groups are sealed shut to inbound traffic.Only outbound is allowed. Stateful in nature.


### ROUTE 53
A fully managed DNS resolution service by AWS that helps in rerouting the end users to end locations and internet applications by translating web page names to numeric ip addresses. Compliant with both ipv4 and ipv6 addresses. Features network traffic and is also good for DOMAIN NAME REGISTRATION.
It is used in cases of -

1.Simple Routing
2.Weighted Routing
3.Geoproximity Routing[based on resource location]
4.Geolocation Routing[based on user location]
5.latency routing
6.failover routing[for redirecting to redundant zones in case of data failure or some primary resource failure]
7.multivalue answer routing

### AWS CloudFront
A high speed and high availability content delivery network service that makes use of edge location and edge caches with route 53 geolocation routing to deliver content to its end users.

