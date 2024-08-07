## Domain 3: Cloud Technology and Services (34% of scored content)

![AWS Cloud Practitioner Domains](https://github.com/emiliedionisio/aws-cloud-practitioner-C02/blob/main/3-cloudtech.png)

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


### What is object storage typically used for in cloud computing?
Object storage is used for storing large amounts of unstructured data, such as documents, images, videos, backups, and archives. It is designed for scalability, durability, and accessibility. Unlike file storage, object storage stores data as discrete units (objects) and is often used for data that needs to be accessed frequently or archived over long periods.
How does Amazon S3 handle durability and availability for object storage?

Amazon S3 provides high durability and availability by replicating data across multiple geographic regions and data centers. It achieves 99.999999999% (11 9's) durability by storing objects in multiple facilities and automatically handling the replication and recovery process. It offers 99.99% availability for objects in the Standard storage class.

### What are some typical use cases for Amazon S3?
Typical use cases include:
Backup and Restore: Storing backup copies of data.
Data Archiving: Long-term data storage, such as compliance data.
Big Data Analytics: Storing large datasets for analytics processing.
Static Website Hosting: Hosting static web assets like HTML, CSS, and JavaScript.
Media Storage and Distribution: Storing and distributing media files like images and videos.

### What is the main difference between Amazon S3 Standard and Amazon S3 Standard-IA storage classes?
Amazon S3 Standard: Designed for frequently accessed data with low latency and high throughput. It offers high durability and availability.
Amazon S3 Standard-IA (Infrequent Access): Designed for data that is less frequently accessed but requires rapid access when needed. It has a lower storage cost compared to S3 Standard but higher retrieval costs.
What is the Amazon S3 Glacier storage class used for?

Amazon S3 Glacier is used for long-term archival and backup of data that is rarely accessed. It offers very low-cost storage with retrieval times that range from minutes to hours, making it suitable for data that is infrequently accessed but needs to be preserved.

### How does Amazon S3 Intelligent-Tiering work, and what are its benefits?
Amazon S3 Intelligent-Tiering automatically moves data between two access tiers (frequent and infrequent) based on changing access patterns. It uses monitoring and automation to move objects between tiers to optimize cost. Benefits include cost savings without manual intervention and automated data management based on access patterns.
Explain the use case for Amazon S3 One Zone-IA.

Amazon S3 One Zone-IA is used for data that is infrequently accessed but does not require multiple availability zone resilience. It is ideal for cost-effective storage of non-critical data that can be recreated or does not need to be highly durable.

### What is Amazon Elastic Block Store (Amazon EBS) and what are its primary use cases?
Amazon EBS is a block storage service that provides persistent storage volumes for Amazon EC2 instances. It is used for storing data that requires frequent read and write operations, such as database data, application logs, and file systems. It offers low-latency performance and is well-suited for use cases requiring high IOPS.

### What are the main types of EBS volumes and their characteristics?
General Purpose SSD (gp3/gp2): Balanced price and performance, suitable for a wide range of applications.
Provisioned IOPS SSD (io2/io1): High performance for I/O-intensive applications with provisioned IOPS.
Throughput Optimized HDD (st1): Low-cost, high-throughput for large, sequential workloads like big data.
Cold HDD (sc1): Lowest-cost storage for infrequent access with large amounts of data.
What is the difference between Amazon EBS and instance store?

Amazon EBS: Provides persistent storage that remains available even if the EC2 instance is stopped or terminated. It supports snapshots for backup and data durability.
Instance Store: Provides temporary storage that is physically attached to the host machine and is lost if the instance is stopped or terminated. It is suitable for temporary data that can be recreated, such as caches or buffers.

### What are some common use cases for instance store volumes?
Common use cases include:
Temporary Storage: For caching and buffering data.
Ephemeral Data: Data that is not needed after the instance is stopped or terminated.
High-Performance Computing: Applications that require high IOPS and low-latency access to data.

### Can you attach an EBS volume to multiple EC2 instances at the same time?
Generally, an EBS volume can only be attached to a single EC2 instance at a time. However, an EBS volume can be attached to multiple instances using the EBS Multi-Attach feature for specific volume types, which allows read-write access from multiple instances.
What is the maximum size of a single Amazon EBS volume?

The maximum size of a single Amazon EBS volume is 64 TiB.

### How do you ensure the durability of data stored in Amazon EBS?
Durability is ensured through the following:
Snapshots: Regular snapshots create backups of EBS volumes to Amazon S3, providing durability and recoverability.
Replication: EBS volumes are replicated within the availability zone to protect against hardware failure.

### What is Amazon EBS Snapshots and how are they used?
Amazon EBS Snapshots are backups of EBS volumes stored in Amazon S3. They are used to create point-in-time copies of volumes, which can be restored or used to create new volumes. They are useful for data protection, backup, and recovery.

### Can you change the volume type of an existing Amazon EBS volume?
Yes, you can change the volume type of an existing EBS volume by modifying the volume’s attributes. This process may require the volume to be detached and reattached or the instance to be stopped and restarted, depending on the volume type change.

### What is Amazon Elastic File System (Amazon EFS) and what are its primary use cases?
Amazon EFS is a fully managed, scalable, and elastic file storage service that provides shared access to file systems across multiple EC2 instances. Primary use cases include:
Content Management: Shared file storage for applications.
Big Data and Analytics: Shared access to data for processing.
Web Serving and Content Management: Serving dynamic content with scalability.

### What are the key features of Amazon EFS?
Key features include:
Scalability: Automatically scales capacity up or down.
Elasticity: Grows and shrinks based on the amount of data stored.
Shared Access: Multiple EC2 instances can access the file system concurrently.
Durability: Data is redundantly stored across multiple AZs.

### What is Amazon FSx and what file systems does it support?
Amazon FSx is a service that provides fully managed file systems with the capabilities of traditional file systems. It supports:
Amazon FSx for Windows File Server: Windows-compatible file system with Active Directory integration.
Amazon FSx for Lustre: High-performance file system optimized for compute-intensive workloads.

### What are common use cases for Amazon FSx for Windows File Server?
Common use cases include:
Enterprise Applications: Applications requiring Windows file system features.
Home Directories: Centralized storage for user profiles and home directories.
Application Development: Development environments for Windows applications.

### Can Amazon EFS be accessed from on-premises environments?
Yes, Amazon EFS can be accessed from on-premises environments through AWS Direct Connect or VPN connections, allowing for hybrid cloud scenarios where on-premises systems interact with cloud-based file systems.

### What is the difference between Amazon EFS and Amazon FSx for Windows File Server?
Amazon EFS provides a Linux-native NFS file system suitable for general-purpose file storage and sharing.
Amazon FSx for Windows File Server provides a Windows-native file system compatible with SMB and supports features like Active Directory integration, making it suitable for Windows-based applications and environments.

### What are the performance modes available in Amazon EFS?
General Purpose Mode: Optimized for latency-sensitive use cases where throughput is important, such as web serving and content management.
Max I/O Mode: Optimized for applications requiring high throughput and high IOPS, such as big data and analytics. It scales to accommodate large numbers of instances accessing the file system concurrently.


### What is Amazon RDS, and what are its key features?
Amazon RDS is a managed relational database service provided by AWS that simplifies the setup, operation, and scaling of relational databases in the cloud. It supports multiple database engines, including Amazon Aurora, MySQL, MariaDB, PostgreSQL, Oracle, and Microsoft SQL Server.

Key Features:

Automated Backups: RDS automatically takes backups and allows you to restore data to any point within the backup retention period.
Multi-AZ Deployments: Provides high availability and failover support by automatically replicating data across multiple Availability Zones.
Read Replicas: Helps in scaling read-heavy database workloads.
Automatic Software Patching: RDS automatically applies patches to the database engine.
Security: Integrated with AWS Identity and Access Management (IAM), and supports encryption at rest and in transit.

### What are the benefits of Amazon RDS?
Ease of Management: Reduces administrative overhead such as hardware provisioning, database setup, patching, and backups.
Scalability: Easily scale the compute and storage resources as needed.
High Availability: Built-in features for high availability and disaster recovery.
Cost-Effective: Pay-as-you-go pricing model helps in managing costs effectively.

### What is Amazon DynamoDB, and what are its use cases?
Amazon DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability. It is designed to handle large amounts of unstructured data with low-latency performance.

Use Cases:

Gaming: For real-time data storage and processing.
IoT Applications: Handling high-velocity data from connected devices.
Mobile Backends: Managing user data, session data, and application state.
Retail: Managing inventory, customer data, and transactions.

### What is Amazon Aurora, and how does it differ from other RDS engines?
Amazon Aurora is a relational database engine designed for high performance and availability. It is compatible with both MySQL and PostgreSQL, but offers significant improvements over standard MySQL and PostgreSQL in terms of speed and reliability.

Differences from Other RDS Engines:

Performance: Aurora is designed to deliver up to five times the performance of standard MySQL and twice the performance of standard PostgreSQL.
Storage: Aurora uses a distributed, fault-tolerant storage system that replicates data across multiple Availability Zones.
Scaling: Automatically scales storage capacity up to 128 TiB without manual intervention.

### What is Amazon Redshift, and what is it used for?
Amazon Redshift is a fully managed data warehouse service that allows you to analyze large volumes of data quickly and cost-effectively. It is optimized for online analytical processing (OLAP).

Uses:

Data Warehousing: Consolidates large datasets from various sources.
Business Intelligence: Supports complex queries and large-scale data analytics.

### What is AWS Database Migration Service (DMS), and what are its benefits?
AWS Database Migration Service (DMS) helps migrate databases to AWS quickly and securely. It supports homogeneous (same database engine) and heterogeneous (different database engines) migrations.

Benefits:

Minimal Downtime: Allows for continuous data replication during migration.
Wide Database Support: Supports a variety of source and target databases.
Cost-Effective: You only pay for the resources you use during the migration.

### What is the Schema Conversion Tool (SCT) used for in AWS database migrations?
The AWS Schema Conversion Tool (SCT) is used to convert database schema objects from one database engine to another. It helps in migrating schema from one database engine (e.g., Oracle) to another (e.g., Amazon Aurora).

Uses:

Schema Migration: Converts database objects like tables, indexes, and views.
Compatibility Assessment: Identifies and helps resolve issues related to schema compatibility.

### What are the common steps involved in a database migration using AWS DMS?
Assessment and Planning: Evaluate source and target databases, and plan the migration.
Set Up Source and Target Endpoints: Configure the source and target databases for the migration.
Schema Conversion: Use SCT to convert the schema if necessary.
Create and Configure a Migration Instance: Launch a replication instance to handle data migration.
Start Data Migration: Perform initial data load and configure ongoing replication.
Testing: Validate that the data has been migrated correctly and the application works as expected.
Cutover: Redirect application traffic to the new database.
Monitor and Optimize: Monitor the performance and optimize as needed.

### What are the benefits of using AWS managed databases over EC2-hosted databases?
Operational Efficiency: Reduced administrative tasks such as patching and backups.
High Availability: Built-in features for high availability and failover.
Automatic Scaling: Managed databases can scale automatically based on demand.
Security: Integrated security features and compliance certifications.

### What are some of the AWS managed database services available?
Amazon RDS: Managed relational databases.
Amazon DynamoDB: Managed NoSQL databases.
Amazon Aurora: High-performance managed relational database.
Amazon Redshift: Managed data warehousing.
Amazon Neptune: Managed graph database.
Amazon DocumentDB: Managed document database.

### How does Amazon Aurora differ from Amazon RDS?
Aurora is a specific engine within RDS that offers higher performance and scalability compared to other RDS engines.
RDS includes multiple database engines (MySQL, PostgreSQL, MariaDB, Oracle, SQL Server), whereas Aurora is optimized for performance and high availability beyond what standard RDS engines offer.

### Why might you choose Amazon DynamoDB for your application?
Performance: Consistent, single-digit millisecond response times.
Scalability: Automatically scales up and down based on demand.
Managed Service: No need to manage hardware or software.
Flexible Data Model: Supports both key-value and document data models.

### What are the benefits of using Amazon Redshift for data warehousing?
Performance: High query performance with columnar storage and parallel query execution.
Scalability: Can handle petabyte-scale data.
Cost-Effectiveness: Pay-as-you-go pricing model and options to use reserved instances.
Integration: Seamless integration with other AWS services for data loading, querying, and analytics.



