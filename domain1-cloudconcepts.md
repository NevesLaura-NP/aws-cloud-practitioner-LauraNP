## Domain 1: Cloud Concepts (24% of scored content)

![AWS Cloud Practitioner Domains]((https://cdn.wallpapersafari.com/51/42/9ghfao.jpg))

#### 1.1: Define the benefits of the AWS Cloud
#### Knowledge of: Value proposition of the AWS Cloud
#### Skills in:
- Understanding the economies of scale (for example, cost savings)
- Understanding the benefits of global infrastructure (for example, speed of deployment, global reach)
- Understanding the advantages of high availability, elasticity, and agility

<!-- Type your questions and answers below -->
#### What is Cloud Computing? 
Cloud computing offers pay-as-you-go IT resource delivery over the internet on demand. This enables businesses to invest only the necessary resources in accordance with demand, rather than having to purchase all technology resources up front.

#### What are the three deployment models for cloud computing, their definitions, and uses?

  Cloud-based deployment model:
  Where one can migrate existing applications to the cloud, or you can design and build new applications in the cloud. You can build those applications on low-level infrastructure that requires your IT staff to manage them. Alternatively, you can build them using higher-level services that reduce the management, architecting, and scaling requirements of the core infrastructure.
  On-premises deployment/rivate cloud deployment:
  In this model, resources are deployed on premises by using virtualization and resource management tools.For example, you might have applications that run on technology that is fully kept in your on-premises data center. Though this model is much like legacy IT infrastructure, its incorporation of application management and virtualization technologies helps to increase resource utilization.
  Hybrid deployment:
  Cloud-based resources are connected to on-premises infrastructure. You might want to use this approach in a number of situations. For example, you have legacy applications that are better maintained on premises, or government regulations require your business to keep certain records on premises.

#### When would you consider a hybrid deployment model?
One can utilize the hybrid model when there is a need to utilize on premises technology and also utilize softwares and process in the cloud.For example, suppose that a company wants to use cloud services that can automate batch data processing and analytics. However, the company has several legacy applications that are more suitable on premises and will not be migrated to the cloud. With a hybrid deployment, the company would be able to keep the legacy applications on premises while benefiting from the data and analytics services that run in the cloud.

#### What are the Benefits of cloud computing and their definitions?
  
.Exchange upfront expense for variable expense
Upfront expense refers to data centers, physical servers, and other resources that you would need to invest in before using them. Variable expense means you only pay for computing resources you consume instead of investing heavily in data centers and servers before you know how you’re going to use them.By taking a cloud computing approach that offers the benefit of variable expense, companies can implement innovative solutions while saving on costs.

.Stop spending money to run and maintain data centers
Computing in data centers often requires you to spend more money and time managing infrastructure and servers. 
A benefit of cloud computing is the ability to focus less on these tasks and more on your applications and customers.

.Stop guessing capacity
With cloud computing, you don’t have to predict how much infrastructure capacity you will need before deploying an application. 
For example, you can launch Amazon EC2 instances when needed, and pay only for the compute time you use. Instead of paying for unused resources or having to deal with limited capacity, you can access only the capacity that you need. You can also scale in or scale out in response to demand.

.Benefit from massive economies of scale
By using cloud computing, you can achieve a lower variable cost than you can get on your own.
Because usage from hundreds of thousands of customers can aggregate in the cloud, providers, such as AWS, can achieve higher economies of scale. The economy of scale translates into lower pay-as-you-go prices. 


.Speed and agility
The flexibility of cloud computing makes it easier for you to develop and deploy applications.
This flexibility provides you with more time to experiment and innovate. When computing in data centers, it may take weeks to obtain new resources that you need. By comparison, cloud computing enables you to access new resources within minutes.


.Go global in minutes
The global footprint of the AWS Cloud enables you to deploy applications to customers around the world quickly, while providing them with low latency. This means that even if you are located in a different part of the world than your customers, customers are able to access your applications with minimal delays. 



#### What are the Amazon EC2 instance types and their definitions?
General purpose instances
Provides a balance of compute, memory, and networking resources. You can use them for a variety of workloads, such as:

application servers
gaming servers
backend servers for enterprise applications
small and medium databases
Suppose that you have an application in which the resource needs for compute, memory, and networking are roughly equivalent. You might consider running it on a general purpose instance because the application does not require optimization in any single resource area.

Compute optimized instances
Ideal for compute-bound applications that benefit from high-performance processors. Like general purpose instances, you can use compute optimized instances for workloads such as web, application, and gaming servers.
However, the difference is compute optimized applications are ideal for high-performance web servers, compute-intensive applications servers, and dedicated gaming servers. You can also use compute optimized instances for batch processing workloads that require processing many transactions in a single group.


Memory optimized instances
They are designed to deliver fast performance for workloads that process large datasets in memory. In computing, memory is a temporary storage area. It holds all the data and instructions that a central processing unit (CPU) needs to be able to complete actions. Before a computer program or application is able to run, it is loaded from storage into memory. This preloading process gives the CPU direct access to the computer program.
Suppose that you have a workload that requires large amounts of data to be preloaded before running an application. This scenario might be a high-performance database or a workload that involves performing real-time processing of a large amount of unstructured data. In these types of use cases, consider using a memory optimized instance. Memory optimized instances enable you to run workloads with high memory needs and receive great performance.

Accelerated computing instances
Accelerated computing instances use hardware accelerators, or coprocessors, to perform some functions more efficiently than is possible in software running on CPUs. Examples of these functions include floating-point number calculations, graphics processing, and data pattern matching.
In computing, a hardware accelerator is a component that can expedite data processing. Accelerated computing instances are ideal for workloads such as graphics applications, game streaming, and application streaming.

Storage optimized instances
They are designed for workloads that require high, sequential read and write access to large datasets on local storage. Examples of workloads suitable for storage optimized instances include distributed file systems, data warehousing applications, and high-frequency online transaction processing (OLTP) systems.
In computing, the term input/output operations per second (IOPS) is a metric that measures the performance of a storage device. It indicates how many different input or output operations a device can perform in one second. Storage optimized instances are designed to deliver tens of thousands of low-latency, random IOPS to applications. 
You can think of input operations as data put into a system, such as records entered into a database. An output operation is data generated by a server. An example of output might be the analytics performed on the records in a database. If you have an application that has a high IOPS requirement, a storage optimized instance can provide better performance over other instance types not optimized for this kind of use case.

#### What is a Load Balancer?
Elastic Load Balancing is the AWS service that automatically distributes incoming application traffic across multiple resources, such as Amazon EC2 instances. 
A load balancer acts as a single point of contact for all incoming web traffic to your Auto Scaling group. This means that as you add or remove Amazon EC2 instances in response to the amount of incoming traffic, these requests route to the load balancer first. Then, the requests spread across multiple resources that will handle them. For example, if you have multiple Amazon EC2 instances, Elastic Load Balancing distributes the workload across the multiple instances so that no single instance has to carry the bulk of it. 
Although Elastic Load Balancing and Amazon EC2 Auto Scaling are separate services, they work together to help ensure that applications running in Amazon EC2 can provide high performance and availability. 

#### What is Amazon EC2? 
It stands for Amazon Elastic Compute Cloud (Amazon EC2) provides secure, resizable compute capacity in the cloud as Amazon EC2 instances. 

Imagine you are responsible for the architecture of your company's resources and need to support new websites. With traditional on-premises resources, you have to do the following:

Spend money upfront to purchase hardware.
Wait for the servers to be delivered to you.
Install the servers in your physical data center.
Make all the necessary configurations.
By comparison, with an Amazon EC2 instance you can use a virtual server to run applications in the AWS Cloud.

#### What is Amazon EC2 and its primary benefits?
You can provision and launch an Amazon EC2 instance within minutes.
You can stop using it when you have finished running a workload.
You pay only for the compute time you use when an instance is running, not when it is stopped or terminated.
You can save costs by paying only for server capacity that you need or want.

#### What is the importance of tagging in EC2?
A tag is a label that you can assign to an AWS resource, it consists  of a Key and a Value. The name of the instance is a default tag. Benefits can include: filtering, automation, cost allocation and access control.

#### How does EC2 pricing work?
  With Amazon EC2, you pay only for the compute time that you use. Amazon EC2 offers a variety of pricing options for different use cases. For example, if your use case can withstand interruptions, you can save with Spot Instances. You can also save by committing early and locking in a minimum level of use with Reserved Instances.

On-Demand
On-Demand Instances are ideal for short-term, irregular workloads that cannot be interrupted. No upfront costs or minimum contracts apply. The instances run continuously until you stop them, and you pay for only the compute time you use.

Sample use cases for On-Demand Instances include developing and testing applications and running applications that have unpredictable usage patterns. On-Demand Instances are not recommended for workloads that last a year or longer because these workloads can experience greater cost savings using Reserved Instances.

Reserved Instances
Reserved Instances are a billing discount applied to the use of On-Demand Instances in your account. There are two available types of Reserved Instances:
Standard Reserved Instances
Convertible Reserved Instances
You can purchase Standard Reserved and Convertible Reserved Instances for a 1-year or 3-year term. You realize greater cost savings with the 3-year option. 
Standard Reserved Instances: This option is a good fit if you know the EC2 instance type and size you need for your steady-state applications and in which AWS Region you plan to run them. Reserved Instances require you to state the following qualifications:
Instance type and size: For example, m5.xlarge
Platform description (operating system): For example, Microsoft Windows Server or Red Hat Enterprise Linux
Tenancy: Default tenancy or dedicated tenancy
You have the option to specify an Availability Zone for your EC2 Reserved Instances. If you make this specification, you get EC2 capacity reservation. This ensures that your desired amount of EC2 instances will be available when you need them. 

Convertible Reserved Instances: If you need to run your EC2 instances in different Availability Zones or different instance types, then Convertible Reserved Instances might be right for you. Note: You trade in a deeper discount when you require flexibility to run your EC2 instances.
At the end of a Reserved Instance term, you can continue using the Amazon EC2 instance without interruption. However, you are charged On-Demand rates until you do one of the following:
Terminate the instance.
Purchase a new Reserved Instance that matches the instance attributes (instance family and size, Region, platform, and tenancy).

EC2 Instance Savings Plans
AWS offers Savings Plans for a few compute services, including Amazon EC2. EC2 Instance Savings Plans reduce your EC2 instance costs when you make an hourly spend commitment to an instance family and Region for a 1-year or 3-year term. This term commitment results in savings of up to 72 percent compared to On-Demand rates. Any usage up to the commitment is charged at the discounted Savings Plans rate (for example, $10 per hour). Any usage beyond the commitment is charged at regular On-Demand rates.
The EC2 Instance Savings Plans are a good option if you need flexibility in your Amazon EC2 usage over the duration of the commitment term. You have the benefit of saving costs on running any EC2 instance within an EC2 instance family in a chosen Region (for example, M5 usage in N. Virginia) regardless of Availability Zone, instance size, OS, or tenancy. The savings with EC2 Instance Savings Plans are similar to the savings provided by Standard Reserved Instances.
Unlike Reserved Instances, however, you don't need to specify up front what EC2 instance type and size (for example, m5.xlarge), OS, and tenancy to get a discount. Further, you don't need to commit to a certain number of EC2 instances over a 1-year or 3-year term. Additionally, the EC2 Instance Savings Plans don't include an EC2 capacity reservation option.
Later in this course, you'll review AWS Cost Explorer, which you can use to visualize, understand, and manage your AWS costs and usage over time. If you're considering your options for Savings Plans, you can use AWS Cost Explorer to analyze your Amazon EC2 usage over the past 7, 30, or 60 days. AWS Cost Explorer also provides customized recommendations for Savings Plans. These recommendations estimate how much you could save on your monthly Amazon EC2 costs, based on previous Amazon EC2 usage and the hourly commitment amount in a 1-year or 3-year Savings Plan.

Spot Instances
Spot Instances are ideal for workloads with flexible start and end times, or that can withstand interruptions. Spot Instances use unused Amazon EC2 computing capacity and offer you cost savings at up to 90% off of On-Demand prices.
Suppose that you have a background processing job that can start and stop as needed (such as the data processing job for a customer survey). You want to start and stop the processing job without affecting the overall operations of your business. If you make a Spot request and Amazon EC2 capacity is available, your Spot Instance launches. However, if you make a Spot request and Amazon EC2 capacity is unavailable, the request is not successful until capacity becomes available. The unavailable capacity might delay the launch of your background processing job.
After you have launched a Spot Instance, if capacity is no longer available or demand for Spot Instances increases, your instance may be interrupted. This might not pose any issues for your background processing job. However, in the earlier example of developing and testing applications, you would most likely want to avoid unexpected interruptions. Therefore, choose a different EC2 instance type that is ideal for those tasks.

Dedicated Hosts
They are physical servers with Amazon EC2 instance capacity that is fully dedicated to your use. 
You can use your existing per-socket, per-core, or per-VM software licenses to help maintain license compliance. You can purchase On-Demand Dedicated Hosts and Dedicated Hosts Reservations. Of all the Amazon EC2 options that were covered, Dedicated Hosts are the most expensive.


#### What is an AWS Availability Zone?
  An Availability Zone is a single data center or a group of data centers within a Region. Availability Zones are located tens of miles apart from each other. This is close enough to have low latency (the time between when content requested and received) between Availability Zones. However, if a disaster occurs in one part of the Region, they are distant enough to reduce the chance that multiple Availability Zones are affected.

#### How do AWS Edge locations enhance the performance of Amazon CloudFront?
  Edge locations are separate from Regions, so you can push content from inside a Region to a collection of Edge locations around the world, in order to accelerate communication and content delivery. AWS Edge locations, also run more than just CloudFront. They run a domain name service, or DNS, known as Amazon Route 53, helping direct customers to the correct web locations with reliably low latency. here's the key points. Number one, Regions are geographically isolated areas, where you can access services needed to run your enterprise. Number two, Regions contain Availability Zones, that allow you to run across physically separated buildings, tens of miles of separation, while keeping your application logically unified. Availability Zones help you solve high availability and disaster recovery scenarios, without any additional effort on your part, and number three, AWS Edge locations run Amazon CloudFront to help get content closer to your customers, no matter where they are in the world.

#### What is AWS Elastic Beanstalk used for?
  AWS Elastic Beanstalk is a service that helps you provision Amazon EC2-based environments. Instead of clicking around the console or writing multiple commands to build out your network, EC2 instances, scaling and Elastic Load Balancers, you can instead provide your application code and desired configurations to the AWS Elastic Beanstalk service, which then takes that information and builds out your environment for you. AWS Elastic Beanstalk also makes it easy to save environment configurations, so they can be deployed again easily. 
  

Amazon EC2 instance types(opens in a new tab) are optimized for different tasks. When selecting an instance type, consider the specific needs of your workloads and applications. This might include requirements for compute, memory, or storage capabilities.
Each instance type is grouped under an instance family and are optimized for certain types of tasks. Instance types offer varying combinations of CPU, memory, storage, and networking capacity, and give you the flexibility to choose the appropriate mix of resources for your applications. The different instance families in EC2 are general purpose, compute optimized, memory optimized, accelerated computing, and storage optimized. 
General purpose instances provide a good balance of compute, memory, and networking resources, and can be used for a variety of diverse workloads like web service or code repositories. 
Compute optimized instances are ideal for compute-intensive tasks like gaming servers, high performance computing or HPC, and even scientific modeling. 
Similarly, memory optimized instances are good for memory-intensive tasks. Accelerated computing are good for floating point number calculations, graphics processing, or data pattern matching, as they use hardware accelerators.
And finally, storage optimized are good for, can you guess it? Workloads that require high performance for locally stored data.

#### What is an Amazon Machine Image (AMI)?
AMIs are a required element to creating a EC2. It has three components. Templates for the Root Volume: Operating System (OS), Applications Serves, Applications. It also permits some Launch Permission Controls and Block Device Mapping.

#### What is a Security Group in EC2?
A security group serves as a virtual firewall that controls access to your instances. It is a way for you to filter the traffic that is allowed to reach your instances. Security Groups are based on rules that you can configure, it blocks all access unless one allow rule is in place for that traffic. The rules can be modified at any time and the new rule updates are automatically applied to all instances associated with the security group immediately


#### What is Amazon ECS? 

The Amazon Elastic Container Service (Amazon ECS) is highly scalable and high-performance container management system. It helps costumers new containers and manage them accross EC2 instances. Amazon ECS supports Docker containers. Docker is a software platform that packages software into containers. To manage your containers, you must install an open source Amazon ECS container agent on your EC2 instances. This agent is referred to as a container instance. You can run this agent on both Linux and Windows Amazon Machine Images(AMIs). Amazon ECS uses API calls to control Docker-enabled applications.

#### What is AWS Lambda?
   It is a serverless computing service that helps you to run code without provisioning or managing servers. You will pay only for the consumed compute time, and when your code ins't running you will pay no charges. With AWS Lambda one can run code for virtually any type of application or backend service, all with zero administration. You need only to upload your code, and Lambda manages everything required to run and scale your code with high availability. You can set up your code to automatically launch from other AWS services or call it directly from any web or mobile app.

#### How does AWS Fargate differ from Amazon EC2?
  AWS Fargate is a serveless compute engine for containers. It allocates the right amount of compute, which reduces the need to manage EC2 instances, cluster capacity, and scaling.

#### What are the benefits of using AMIs?
  Repeatability:
  Instances that are launched from the same AMI are exact replicas of one another. As a result, it greatly facilitates building clusters of similar instances or recreating compute environments.
  Reusability:
  AMIs package the full configuration and content of an EC2 instance such that it can be used over and over again, with efficiency and precision.
  Recoverability:
  An AMI is perfect for replacing failed machines with new instances that are created from the same AMI
  Marketplace Solutions:
  Suppose that you are looking for software solution from a specific vendor. An AMI probably exists on the marketplace that you can launch to implement that solution on an EC2 instance. Additionally, authorized software vendors can create AMIs and also sell them there
  Backups:
  AMIs provide a great way to back up a complete EC2 instance configuration, which you can use to launch a replacement instance in the event of a failure.

#### What security features does EC2 offer?
  EC2 offers Security Groups which serve as a firewall for instances. The rules of the security group filters the traffic that is allowed to access the instances. All the rules from all security groups that are attached to an instance are evaluated before traffic is allowed to pass through.

#### Can you automate EC2 scaling?
Yes. The Amazon Auto Scaling helps you maintain scale availability and lets you automatically add or remove EC2 instances according to conditions you define.

#### What are the steps to launch an EC2 instance?
  1. Instance Name and Tags
  2. Select Amazon Machine Image
  3. Select Instance Type
  4. Key Pair
  5. Network Settings
  6. Configure Storage
  7. Advanced Details
#### How do security groups protect your EC2 instances?
Security Groups are based on rules that you can configure, it blocks all access unless one allow rule is in place for that traffic. The rules can be modified at any time and the new rule updates are automatically applied to all instances associated with the security group immediately

#### Why is data sovereignty important in AWS Regions?
  You might have government compliance requirements that your financial information in Frankfurt cannot leave Germany. Any data stored in the Frankfurt Region never leaves the Frankfurt Region, or data in the London region never leaves London, or Sydney never leaves Sydney, unless you explicitly, with the right credentials and permissions, request the data be exported. 
Regional data sovereignty is part of the critical design of AWS Regions. With data being subject to the local laws and statutes of the country where the Region lives. So with that understanding, that your data, your application, lives and runs in a Region, one of the first decisions you get to make is which Region you pick.

#### What is the purpose of a VPC in Amazon EC2?
Imagine the millions of customers who use AWS services. Also, imagine the millions of resources that these customers have created, such as Amazon EC2 instances. Without boundaries around all of these resources, network traffic would be able to flow between them unrestricted. 
Amazon VPC enables you to provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define. Within a virtual private cloud (VPC), you can organize your resources into subnets. 

#### What are subnets and their role in EC2?
  A subnet is a section of a VPC in which you can group resources based on security or operational needs. Subnets can be public or private.
  Public subnets contain resources that need to be accessible by the public, such as an online store’s website.
  Private subnets contain resources that should be accessible only through your private network, such as a database that contains customers’ personal information and order histories.
  In a VPC, subnets can communicate with each other. For example, you might have an application that involves Amazon EC2 instances in a public subnet communicating with databases that are located in a private subnet.

#### What factors should you consider when choosing a region for your EC2 instance? What are the four main factors to consider when choosing an AWS Region? 
When determining the right Region for your services, data, and applications, consider the following four factors:
Compliance with data governance and legal requirements

Depending on your company and location, you might need to run your data out of specific areas. For example, if your company requires all of its data to reside within the boundaries of the UK, you would choose the London Region.
Not all companies have location-specific data regulations, so you might need to focus more on the other three factors.

Proximity to your customers

Selecting a Region that is close to your customers will help you to get content to them faster. For example, your company is based in Washington, DC, and many of your customers live in Singapore. You might consider running your infrastructure in the Northern Virginia Region to be close to company headquarters, and run your applications from the Singapore Region.

Available services within a Region

Sometimes, the closest Region might not have all the features that you want to offer to customers. AWS is frequently innovating by creating new services and expanding on features within existing services. However, making new services available around the world sometimes requires AWS to build out physical hardware one Region at a time. 
Suppose that your developers want to build an application that uses Amazon Braket (AWS quantum computing platform). As of this course, Amazon Braket is not yet available in every AWS Region around the world, so your developers would have to run it in one of the Regions that already offers it.

Pricing

Suppose that you are considering running applications in both the United States and Brazil. The way Brazil’s tax structure is set up, it might cost 50% more to run the same workload out of the São Paulo Region compared to the Oregon Region. You will learn in more detail that several factors determine pricing, but for now know that the cost of services can vary from Region to Region.

#### What is an AWS Region?
  A Region is a physical location around the world where AWS clusters data centers. It is where all of the pieces and parts of your application live.

#### What are the main architectural components of Amazon EC2?
  Regions
  VPC
  Subnets
  Security Groups

#### What security features does Amazon EC2 provide?
  Amazon EC2 provides with Security groups and IAM roles that enables you to manage access to AWS services and resources securely. IAM gives you the flexibility to configure access based on your company’s specific operational and security needs. You do this by using a combination of IAM features, which are explored in detail in this lesson:

IAM users, groups, and roles
IAM policies
Multi-factor authentication  

 #### What level of control do users have over EC2 instances?
  Depending on the IAM role an root user can launch servers when needed and terminate or stop instances when they are no longer needed. There is full control over the guest operating system. One can launch instances of any size into an Availability Zone anywhere in the world and can control traffic through Security Groups and Elastic Load Balancing.

#### How does EC2 demonstrate elasticity?
  One can use the Amazon EC2 to increase and decrease capacity within minutes, not hours or days. You can comission one, hundreds, or even thousands of server instances simultaneously. You can also use Amazon EC2 Auto Scaling to maintain availability of your Amazon EC2 fleet and automatically scale your fleet up and down depending on your needs to maximize performance and maximize cost.

#### How does EC2 integrate with other AWS services?
Amazon EC2 is integrated with most AWS services. These services could include Amazon S3, Amazon RDS, and Amazon VPC. This integration provides a complete, secure solution for computing, query processing, and cloud storage accross a wide range of applications. One can access and manage these integrations through the Control 

#### What are the benefits of using AWS Elastic Beanstalk?
  AWS Elastic Beanstalk gives you the convenience of not having to provision and manage all of these pieces separately, while still giving you the visibility and control of the underlying resources. You get to focus on your business application, not the infrastructure.
  With AWS Elastic Beanstalk, you provide code and configuration settings, and Elastic Beanstalk deploys the resources necessary to perform the following tasks:

Adjust capacity
Load balancing
Automatic scaling
Application health monitoring

#### What is serverless computing and its use cases?
  Serverless Computing gives you the ability to run code without provisioning or managing servers. Serverless computing features automatic scaling, built-in high availability, and a pay-for-use billing model to increase agility and optimize costs. Serverless computing also eliminates infrastructure management tasks like capacity provisioning and patching, so you can focus on writing code that serves clients. Serverless use cases include:
  .File Processing
  .Web Applications
  .Mobile Backends
  . Cron jobs(scheduling computer tasks)

#### What are containers and their advantages?
  Containers are a method of OS virtualization that you can use to run an application and its dependencies in resource-isolated processes. By using containers, you can package an application's code, configurations, and dependencies into simple building blocks that deliver environmental consistency, operationa efficiency, developer productivity, and version control. Containers are smaller than virtual machines and do not contain an entire operating system. Instea, containers share a virtualized OS and run as resource-isolated processes, which ensure quick, reliable, and consistent deployments. Containers hold everything that the software needs to run, such as libraries, system tools, code, and the runtime. Container use cases are:
  .Building Microservices architecture
  .Video rendering services
  .Quick development and deployment

#### What is the primary purpose of AWS Regions in the global infrastructure?
AWS Regions are physical locations around the world where AWS deploys its infrastructure. The primary purpose of AWS Regions is to provide geographic diversity and redundancy. They allow customers to deploy resources in multiple geographic areas to achieve lower latency, comply with data sovereignty requirements, and enhance fault tolerance and high availability.

#### Describe the function of Amazon CloudFront in AWS's architecture.
Amazon CloudFront is a content delivery network (CDN) service provided by AWS. Its main function is to deliver content (such as web pages, videos, applications) with low latency and high transfer speeds. CloudFront caches content at edge locations located around the world, reducing the load on origin servers and improving user experience by serving content from locations closer to the end-users.

#### Explain how Amazon Route 53 integrates with AWS Edge locations to enhance user experiences.
Amazon Route 53 is a scalable domain name system (DNS) web service. It integrates with AWS Edge locations by routing end-user requests to the closest available AWS Edge location, which can then serve the requested content through services like CloudFront. This integration enhances user experiences by reducing latency and improving responsiveness for global applications.

#### What are the advantages of using AWS Outposts for local data processing needs?
AWS Outposts bring native AWS services, infrastructure, and operating models to virtually any customer on-premises facility. Advantages include seamless integration with AWS services, low latency for local data processing, support for workloads that need to remain on-premises due to specific requirements, and consistent operational experience across cloud and on-premises environments.

#### How are AWS Lambda and AWS Outposts different in what they offer for cloud computing?
AWS Lambda is a serverless compute service that lets you run code without provisioning or managing servers. It automatically scales based on demand and charges you only for the compute time consumed. AWS Outposts, on the other hand, extends AWS infrastructure to on-premises locations, allowing you to run AWS services locally for applications that require low-latency data processing or need to meet specific compliance requirements.

#### What is high availability?
High availability refers to a system or service that is designed to be operational and accessible for a high percentage of the time, usually 99.99% or higher. It typically involves redundancy, fault tolerance, and rapid failover mechanisms to minimize downtime and ensure continuous operation.

#### What are the benefits of AWS having a global infrastructure with multiple regions?
The benefits include improved latency for end-users, compliance with data sovereignty requirements, enhanced fault tolerance and disaster recovery capabilities, and the ability to deploy applications closer to customers worldwide. It also provides flexibility to scale resources geographically as business needs evolve.

#### How do AWS Regions enhance disaster recovery capabilities?
AWS Regions allow you to deploy resources in geographically separate locations. This geographical diversity is crucial for disaster recovery because it ensures that if one region experiences a service disruption (e.g., due to a natural disaster or outage), applications and data can failover to resources in another region, maintaining continuity of operations.

#### What is the purpose of having multiple Availability Zones within an AWS Region?
Availability Zones (AZs) are distinct locations within a region that are engineered to be isolated from failures in other AZs. The purpose of having multiple AZs is to provide high availability and fault tolerance. By distributing resources across AZs, you can protect applications and data from localized failures and ensure that your services remain operational even if one AZ goes down.

#### How does AWS ensure low latency communication between Availability Zones?
AWS connects Availability Zones within a region through low-latency links in its global network infrastructure. This network design ensures fast and reliable communication between AZs, enabling synchronous replication for services like databases and allowing for rapid data transfer during failover scenarios.

#### Why is it important to run EC2 instances across multiple AZs?
Running EC2 instances across multiple AZs improves fault tolerance and high availability. If one AZ becomes unavailable, instances in other AZs can continue to operate without disruption. This setup also allows for load balancing and scaling across multiple availability zones to distribute traffic and optimize performance.

#### How do regional AWS services enhance high availability?
Regional AWS services are designed to operate across multiple Availability Zones within a region. They automatically replicate data and distribute resources across AZs, which enhances fault tolerance and ensures that services remain available even if there are failures in one AZ. This regional redundancy is key to achieving high availability in AWS deployments.

#### What is the purpose of Amazon CloudFront?
Amazon CloudFront is a content delivery network (CDN) service that accelerates the delivery of your websites, APIs, video content, and other web assets to users across the globe. It improves performance by caching content at edge locations closest to end-users, reducing latency and lowering the load on origin servers.

#### What are edge locations in AWS?
Edge locations are endpoints for AWS CloudFront and AWS Lambda Edge. They are located in major cities around the world and are used for caching content closer to end-users to improve latency and data transfer speeds. Edge locations are part of AWS's global network infrastructure.

#### What is AWS Outposts?
AWS Outposts is a fully managed service that extends AWS infrastructure, AWS services, APIs, and tools to virtually any customer on-premises facility. It allows you to run compute and storage locally, providing a consistent hybrid experience and seamless integration with AWS services in the cloud.

#### How do Availability Zones within AWS Regions contribute to disaster recovery and high availability?
Availability Zones within AWS Regions contribute to disaster recovery and high availability by providing physically separate locations with independent power, cooling, and networking. This isolation helps protect applications and data from failures and allows for redundant deployments that can automatically failover to another AZ in case of disruption.

#### How do AWS Edge locations and Amazon CloudFront improve content delivery?
AWS Edge locations host CloudFront caches, allowing content to be delivered with lower latency and higher transfer speeds to end-users. When users request content, CloudFront serves it from the nearest edge location rather than fetching it from the origin server, reducing latency and improving overall performance.

#### What is an API in the context of AWS?
In AWS, an API (Application Programming Interface) is a set of rules and protocols that allows one software application to communicate with another. AWS provides APIs for interacting with its services programmatically, enabling automation, integration, and orchestration of cloud resources.

#### What is the primary method of interacting with AWS services?
The primary method of interacting with AWS services is through the AWS Management Console, a web-based interface that allows you to access and manage AWS resources using a graphical user interface (GUI).

#### What are the main ways to interact with AWS services?
Besides the Management Console, you can interact with AWS services using:
    - Command Line Interface (CLI): AWS provides a CLI tool that allows you to manage services from the command line.
    - Software Development Kits (SDKs): SDKs are available for various programming languages, making it easier to integrate AWS services into applications.
    - APIs: Directly calling AWS service APIs enables programmatic control and automation of AWS resources.

#### Why is automation important in cloud deployment?
Automation in cloud deployment improves efficiency, consistency, and scalability. It reduces manual intervention, minimizes errors, and speeds up deployment processes. Automation also facilitates continuous integration and continuous deployment (CI/CD) pipelines, enabling faster delivery of applications and services.

#### What is the primary advantage of using AWS Elastic Beanstalk over manual methods like the AWS Management Console?
AWS Elastic Beanstalk automates the deployment and management of applications, handling capacity provisioning, load balancing, scaling, and application health monitoring. This automation simplifies the deployment process and reduces the operational overhead compared to manual configuration via the Management Console.

#### How does AWS CloudFormation help in managing AWS resources?
AWS CloudFormation is a service that allows you to define and provision AWS infrastructure as code (IaC). It uses templates to describe resources and their dependencies in JSON or YAML format. CloudFormation automates resource provisioning, simplifies updates and rollback procedures, and helps maintain consistency across environments.

#### What are the main components of AWS Global Infrastructure?
The main components include:
    - Regions: Geographical locations where AWS deploys its data centers.
    - Availability Zones (AZs): Isolated locations within regions for fault tolerance.
    - Edge Locations: Points of presence for CDN services like CloudFront.
    - Regional Edge Caches: Caches for CloudFront content within AWS regions.

#### Which AWS services automatically run across multiple Availability Zones?**
AWS services such as Amazon EC2, Amazon RDS (Relational Database Service), and Amazon S3 (Simple Storage Service) automatically replicate data and distribute workloads across multiple Availability Zones within a region for high availability and fault tolerance.

#### What is the recommended best practice for deploying infrastructure in AWS?**
 The recommended best practice is to use AWS Cloudformation or another infrastructure as code (IaC) tool to automate the deployment of infrastructure. This approach ensures consistency, scalability, and repeatability in deployments, and it facilitates version control and auditing of changes.

#### What are the four main purchasing options for EC2 instances, and what are their key characteristics?
The four purchasing options for EC2 instances are:
    - On-Demand Instances: Pay-as-you-go with no long-term commitments.
    - Reserved Instances: Reserved capacity for a 1- or 3-year term, offering significant cost savings.
    - Spot Instances: Bid for unused EC2 capacity, potentially saving up to 90% compared to On-D
  
--------
#### 1.2: Identify design principles of the AWS Cloud
#### Knowledge of: AWS Well-Architected Framework
#### Skills in:
- Understanding the pillars of the Well-Architected Framework (for example, operational excellence, security, reliability, performance efficiency, cost optimization, sustainability)
- Identifying differences between the pillars of the Well-Architected Framework

#### 1.3: Understand the benefits of and strategies for migration to the AWS Cloud
#### Knowledge of:
- Cloud adoption strategies
- Resources to support the cloud migration journey
#### Skills in:
- Understanding the benefits of the AWS Cloud Adoption Framework (AWS CAF) (for example, reduced business risk; improved environmental, social, and governance (ESG) performance; increased revenue; increased operational efficiency)
- Identifying appropriate migration strategies (for example, database replication, use of AWS Snowball)

#### 1.4: Understand concepts of cloud economics
#### Knowledge of:
- Aspects of cloud economics
- Cost savings of moving to the cloud
##### Skills in:
- Understanding the role of fixed costs compared with variable costs
- Understanding costs that are associated with on-premises environments
- Understanding the differences between licensing strategies (for example, Bring Your Own License [BYOL] model compared with included licenses)
- Understanding the concept of rightsizing
- Identifying benefits of automation (for example, provisioning and configuration management with AWS CloudFormation)
- Identifying managed AWS services (for example, Amazon RDS, Amazon Elastic Container Service [Amazon ECS], Amazon Elastic Kubernetes Service [Amazon EKS], Amazon DynamoDB)


#### Questions

- What are the four main purchasing options for EC2 instances, and what are their key characteristics?
- What are the different computing models available in AWS?
- What are some of the popular AWS computing services?
  AWS S3, AWS VPC, AWS Lambda, AWS Beanstalk
