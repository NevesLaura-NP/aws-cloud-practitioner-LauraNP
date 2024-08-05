## Domain 3: Cloud Technology and Services (34% of scored content)

![AWS Cloud Practitioner Domains](https://github.com/emiliedionisio/aws-cloud-practitioner-C02/blob/main/3-cloudtech.png)

#### 3.1: Define methods of deploying and operating in the AWS Cloud
#### Knowledge of:
- Different ways of provisioning and operating in the AWS Cloud
- Different ways to access AWS services
- Types of cloud deployment models
- Connectivity options
#### Skills in:
- Deciding between options such as programmatic access (for example, APIs, SDKs, CLI), the AWS Management Console, and infrastructure as code (IaC)
- Evaluating requirements to determine whether to use one-time operations or repeatable processes
- Identifying different deployment models (for example, cloud, hybrid, on-premises)
- Identifying connectivity options (for example, AWS VPN, AWS Direct Connect, public internet)

#### 3.2: Define the AWS global infrastructure
#### Knowledge of:
- AWS Regions, Availability Zones, and edge locations
- High availability
- Use of multiple Regions
- Benefits of edge locations
- AWS Wavelength Zones and AWS Local Zones
#### Skills in:
- Describing relationships among Regions, Availability Zones, and edge locations
- Describing how to achieve high availability by using multiple Availability Zones
- Recognizing that Availability Zones do not share single points of failure
- Describing when to use multiple Regions (for example, disaster recovery, business continuity, low latency for end users, data sovereignty)
- Describing at a high level the benefits of edge locations (for example, Amazon CloudFront, AWS Global Accelerator)

#### 3.3 Identify AWS compute services
#### Knowledge of: AWS compute services
#### Skills in:
- Recognizing the appropriate use of different EC2 instance types (for example, compute optimized, storage optimized)
- Recognizing the appropriate use of different container options (for example, Amazon ECS, Amazon EKS)
- Recognizing the appropriate use of different serverless compute options (for example, AWS Fargate, Lambda)
- Recognizing that auto scaling provides elasticity
- Identifying the purposes of load balancers

#### 3.4: Identify AWS database services
#### Knowledge of:
- AWS database services
- Database migration
#### Skills in:
- Deciding when to use EC2 hosted databases or AWS managed databases
- Identifying relational databases (for example, Amazon RDS, Amazon Aurora)
- Identifying NoSQL databases (for example, DynamoDB)
- Identifying memory-based databases
- Identifying database migration tools (for example AWS Database Migration Service [AWS DMS], AWS Schema Conversion Tool [AWS SCT])

#### 3.5: Identify AWS network services
#### Knowledge of: AWS network services
#### Skills in:
- Identifying the components of a VPC (for example, subnets, gateways)
- Understanding security in a VPC (for example, network ACLs, security groups)
- Understanding the purpose of Amazon Route 53
- Identifying edge services (for example, CloudFront, Global Accelerator)
- Identifying network connectivity options to AWS (for example AWS VPN, Direct Connect)

#### 3.6: Identify AWS storage services
#### Knowledge of: AWS storage services
#### Skills in:
- Identifying the uses for object storage
- Recognizing the differences in Amazon S3 storage classes
- Identifying block storage solutions (for example, Amazon Elastic Block Store [Amazon EBS], instance store)
- Identifying file services (for example, Amazon Elastic File System [Amazon EFS], Amazon FSx)
- Identifying cached file systems (for example, AWS Storage Gateway)
- Understanding use cases for lifecycle policies
- Understanding use cases for AWS Backup

#### 3.7: Identify AWS artificial intelligence and machine learning (AI/ML) services and analytics services
##### Knowledge of:
- AWS AI/ML services
- AWS analytics services
##### Skills in:
- Understanding the different AI/ML services and the tasks that they accomplish (for example, Amazon SageMaker, Amazon Lex, Amazon Kendra)
- Identifying the services for data analytics (for example, Amazon Athena, Amazon Kinesis, AWS Glue, Amazon QuickSight)

#### 3.8: Identify services from other in-scope AWS service categories.
#### Knowledge of:
- Application integration services of Amazon EventBridge, Amazon Simple Notification Service (Amazon SNS), and Amazon Simple Queue Service (Amazon SQS)
- Business application services of Amazon Connect and Amazon Simple Email Service (Amazon SES)
- Customer engagement services of AWS Activate for Startups, AWS IQ, AWS Managed Services (AMS), and AWS Support
- Developer tool services and capabilities of AWS AppConfig, AWS Cloud9, AWS CloudShell, AWS CodeArtifact, AWS CodeBuild, AWS CodeCommit, AWS CodeDeploy, AWS CodePipeline, AWS CodeStar, and AWS X-Ray
- End-user computing services of Amazon AppStream 2.0, Amazon WorkSpaces, and Amazon WorkSpaces Web
- Frontend web and mobile services of AWS Amplify and AWS AppSync
- IoT services of AWS IoT Core and AWS IoT Greengrass
#### Skills in:
- Choosing the appropriate service to deliver messages and to send alerts and notifications
- Choosing the appropriate service to meet business application needs
- Choosing the appropriate service for AWS customer support
- Choosing the appropriate option for business support assistance
- Identifying the tools to develop, deploy, and troubleshoot applications
- Identifying the services that can present the output of virtual machines (VMs) on end-user machines
- Identifying the services that can create and deploy frontend and mobile services
- Identifying the services that manage IoT devices
- 
#### What is a VPC in AWS, and why is it important?
It is a logically isolated virtual network dedicated to your AWS Account where you can launch AWS Resources such as Amazon EC2 and Amazon RDS instances. You can use VPC to create managed networks in the cloud. It is a private environment and users have full control over its configurations. The Amazon VPC can handle all networking needs and offers elasticity to make changes based on business needs at most affordable rates.

#### What is a subnet, and how is it used in a VPC?
A subnet is a segment of a VPC’s IP address range where you can place your resources. Subnets help organize and partition your VPC network. They are often used to isolate resources based on their purpose or security requirements. For example, you might have public subnets for resources that need internet access and private subnets for resources that should not be directly accessible from the internet.
Subnets are chosen under certain availability zones.

When you create a subnet, you specify an Availability Zone (AZ) in which to place it. This helps ensure high availability by distributing resources across multiple AZs, which are isolated from one another but connected via high-speed, low-latency links.

#### What is an Internet Gateway, and what role does it play in a VPC?
An Internet Gateway (IGW) is a horizontally scaled, highly available VPC component that allows communication between instances in your VPC and the internet. It is necessary for instances in public subnets to access the internet and for internet-based services to reach your instances.

#### What is a NAT Gateway, and why would you use it in a VPC?
A NAT (Network Address Translation) Gateway enables instances in a private subnet to connect to the internet for outbound traffic while preventing unsolicited inbound traffic from the internet. It allows private resources to access the internet for updates or downloads without exposing them to direct internet access.

#### What is a Route Table, and how does it function in a VPC?
A Route Table contains a set of rules (routes) used to determine where network traffic from your subnet or gateway is directed. Each subnet in a VPC is associated with a route table that directs traffic to the appropriate destination, such as an internet gateway, NAT gateway, or a virtual private gateway.

#### What is a VPC Peering Connection, and what are its use cases?

A VPC Peering Connection is a network connection between two VPCs that allows them to communicate using private IP addresses. It can be used to share resources, such as databases or services, between VPCs that belong to the same or different AWS accounts, without using public IP addresses or traversing the internet.

#### What is a Security Group, and how does it enhance security in a VPC?
A Security Group acts as a virtual firewall for your EC2 instances, controlling inbound and outbound traffic based on rules you define. It enhances security by allowing or denying traffic based on IP protocol, port number, and source or destination IP address, and it is stateful, meaning that return traffic is automatically allowed if the initial request is allowed.

#### What is a Network ACL (Access Control List), and how does it differ from a Security Group?
A Network ACL is a stateless firewall that controls inbound and outbound traffic at the subnet level. Unlike Security Groups, which are stateful and applied to individual instances, Network ACLs apply to all resources within a subnet and evaluate rules for both inbound and outbound traffic. They provide an additional layer of security by allowing or denying traffic based on IP address, protocol, and port range.

#### How do you use Network ACLs to enhance security within a VPC?
Network ACLs can be used to implement additional layers of security by defining rules that control traffic at the subnet boundary. You can use them to block or allow traffic from specific IP addresses or ranges, add an extra layer of defense, and provide protections for both inbound and outbound traffic.

#### What is an Elastic IP Address, and how is it used in a VPC?

An Elastic IP Address (EIP) is a static IPv4 address designed for dynamic cloud computing. It is associated with your AWS account and can be allocated to and associated with an instance or a network interface. EIPs are used to ensure that your applications have a consistent public IP address even if the underlying instance is stopped or terminated.

#### What is a Virtual Private Gateway, and how does it function in a VPC?
A Virtual Private Gateway (VGW) is a VPC component that enables you to connect your VPC to an on-premises network via a VPN connection or Direct Connect. It provides the interface for routing traffic between the VPC and external networks and supports encrypted VPN connections.

#### What is Amazon Route 53, and what are its primary functions?
Amazon Route 53 is a scalable DNS web service that provides domain name registration, DNS routing, and health checking for applications. Its primary functions include translating domain names into IP addresses, routing traffic based on various routing policies, and monitoring the health of resources.

#### What is the purpose of DNS in the context of Route 53?
DNS (Domain Name System) translates human-readable domain names (like www.example.com) into IP addresses that computers use to identify each other on the network. Route 53 provides DNS services, enabling users to route internet traffic to their applications and services efficiently.

#### How does Route 53 provide high availability and reliability for DNS queries?
Route 53 provides high availability by using a global network of DNS servers to ensure that DNS queries are answered quickly and reliably. It also supports features like health checks and failover, which route traffic away from unhealthy resources to healthy ones.

#### What is geolocation routing in Route 53, and what are its benefits?
Geolocation routing in Route 53 allows you to route traffic based on the geographic location of the users making the DNS queries. This can improve user experience by directing users to the closest or most appropriate endpoint, reduce latency, and comply with regional regulations or content restrictions.

#### What is Amazon CloudFront, and what are its primary functions?
Amazon CloudFront is a content delivery network (CDN) service that caches and delivers your content (such as web pages, videos, and APIs) from edge locations around the world. Its primary functions include reducing latency, improving load times, and providing secure content delivery with integrated DDoS protection.

#### What are the benefits of using Amazon CloudFront?
Benefits include improved performance through low-latency delivery of content, reduced load on origin servers, enhanced security features (such as SSL/TLS and DDoS protection), and cost savings through edge caching that reduces data transfer costs.

#### What is AWS Global Accelerator, and what is its purpose?
AWS Global Accelerator is a service that improves the availability and performance of applications with global users. It directs traffic to optimal AWS endpoints based on health, geography, and routing policies, providing low-latency access and improving application availability.

#### What is the difference between Amazon CloudFront and AWS Global Accelerator?
Amazon CloudFront is focused on delivering content from edge locations to end-users, optimizing performance for static and dynamic content. AWS Global Accelerator improves application performance and availability by routing traffic to the best AWS endpoints and optimizing global network performance.

#### What is an edge location in the context of Amazon CloudFront?
An edge location is a data center that CloudFront uses to cache copies of your content closer to users, improving access speed and reducing latency. CloudFront has a global network of edge locations to ensure efficient and quick delivery of content.

#### What is AWS Direct Connect, and what are its primary benefits?
AWS Direct Connect is a service that provides a dedicated network connection between your on-premises data center and AWS. Its primary benefits include consistent network performance, lower latency, improved security, and reduced data transfer costs compared to using the internet.

#### What are common use cases for AWS Direct Connect?
Common use cases include transferring large volumes of data to and from AWS, integrating on-premises applications with AWS services, ensuring high-speed and low-latency connectivity, and maintaining private network connections for sensitive data.

#### What is AWS VPN, and how does it differ from AWS Direct Connect?
AWS VPN provides secure, encrypted connections over the internet between your on-premises network and AWS. Unlike Direct Connect, which uses a dedicated physical connection, AWS VPN operates over the public internet, providing flexibility and lower upfront costs but potentially less consistent performance.

#### What types of AWS VPN connections are available?
AWS offers two types of VPN connections:
Site-to-Site VPN: Connects an on-premises network to a VPC using an IPsec VPN connection.
Client VPN: Provides secure remote access to your VPC for individual users via VPN clients.

#### What is a Transit Gateway, and how does it benefit network connectivity?

AWS Transit Gateway is a network transit hub that enables you to connect multiple VPCs and on-premises networks through a single gateway. It simplifies network management by consolidating connections, reducing the complexity of managing multiple peering relationships, and providing scalable network interconnectivity.
