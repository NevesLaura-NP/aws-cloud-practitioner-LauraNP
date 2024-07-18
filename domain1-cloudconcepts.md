## Domain 1: Cloud Concepts (24% of scored content)

![AWS Cloud Practitioner Domains](https://github.com/emiliedionisio/aws-cloud-practitioner-C02/blob/main/1-cloudconcepts.png)

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
  Cloud-based resources are connected to on-premises infrastructure. You might want to use this approach in a number of situations. For example, you have legacy applications that are better maintained on premises, or government regulations require your business to keep certain records on premises.For example, suppose that a company wants to use cloud services that can automate batch data processing and analytics. However, the company has several legacy applications that are more suitable on premises and will not be migrated to the cloud. With a hybrid deployment, the company would be able to keep the legacy applications on premises while benefiting from the data and analytics services that run in the cloud.

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
–
General purpose instances provide a balance of compute, memory, and networking resources. You can use them for a variety of workloads, such as:

application servers
gaming servers
backend servers for enterprise applications
small and medium databases
Suppose that you have an application in which the resource needs for compute, memory, and networking are roughly equivalent. You might consider running it on a general purpose instance because the application does not require optimization in any single resource area.

Compute optimized instances
–
Compute optimized instances are ideal for compute-bound applications that benefit from high-performance processors. Like general purpose instances, you can use compute optimized instances for workloads such as web, application, and gaming servers.



However, the difference is compute optimized applications are ideal for high-performance web servers, compute-intensive applications servers, and dedicated gaming servers. You can also use compute optimized instances for batch processing workloads that require processing many transactions in a single group.


Memory optimized instances
–
Memory optimized instances are designed to deliver fast performance for workloads that process large datasets in memory. In computing, memory is a temporary storage area. It holds all the data and instructions that a central processing unit (CPU) needs to be able to complete actions. Before a computer program or application is able to run, it is loaded from storage into memory. This preloading process gives the CPU direct access to the computer program.



Suppose that you have a workload that requires large amounts of data to be preloaded before running an application. This scenario might be a high-performance database or a workload that involves performing real-time processing of a large amount of unstructured data. In these types of use cases, consider using a memory optimized instance. Memory optimized instances enable you to run workloads with high memory needs and receive great performance.


Accelerated computing instances
–
Accelerated computing instances use hardware accelerators, or coprocessors, to perform some functions more efficiently than is possible in software running on CPUs. Examples of these functions include floating-point number calculations, graphics processing, and data pattern matching.



In computing, a hardware accelerator is a component that can expedite data processing. Accelerated computing instances are ideal for workloads such as graphics applications, game streaming, and application streaming.

Storage optimized instances
–
Storage optimized instances are designed for workloads that require high, sequential read and write access to large datasets on local storage. Examples of workloads suitable for storage optimized instances include distributed file systems, data warehousing applications, and high-frequency online transaction processing (OLTP) systems.



In computing, the term input/output operations per second (IOPS) is a metric that measures the performance of a storage device. It indicates how many different input or output operations a device can perform in one second. Storage optimized instances are designed to deliver tens of thousands of low-latency, random IOPS to applications. 



You can think of input operations as data put into a system, such as records entered into a database. An output operation is data generated by a server. An example of output might be the analytics performed on the records in a database. If you have an application that has a high IOPS requirement, a storage optimized instance can provide better performance over other instance types not optimized for this kind of use case.

- What is a Load Balancer?
- Elastic Load Balancing is the AWS service that automatically distributes incoming application traffic across multiple resources, such as Amazon EC2 instances. 

A load balancer acts as a single point of contact for all incoming web traffic to your Auto Scaling group. This means that as you add or remove Amazon EC2 instances in response to the amount of incoming traffic, these requests route to the load balancer first. Then, the requests spread across multiple resources that will handle them. For example, if you have multiple Amazon EC2 instances, Elastic Load Balancing distributes the workload across the multiple instances so that no single instance has to carry the bulk of it. 

Although Elastic Load Balancing and Amazon EC2 Auto Scaling are separate services, they work together to help ensure that applications running in Amazon EC2 can provide high performance and availability. 






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

- What is the primary purpose of AWS Regions in the global infrastructure?
- Describe the function of Amazon CloudFront in AWS's architecture.
- How do AWS Edge locations enhance the performance of Amazon CloudFront?
- Explain how Amazon Route 53 integrates with AWS Edge locations to enhance user experiences.
- What are the advantages of using AWS Outposts for local data processing needs?
- How are AWS Lambda and AWS Outposts different in what they offer for cloud computing?
- What is high availability?
- What are the benefits of AWS having a global infrastructure with multiple regions?
- What is an AWS Region?
- Why is data sovereignty important in AWS Regions?
- How do AWS Regions enhance disaster recovery capabilities?
- What are the four main factors to consider when choosing an AWS Region? 1. The location of the user, 2.
- What is an AWS Availability Zone?
- What is the purpose of having multiple Availability Zones within an AWS Region?
- How does AWS ensure low latency communication between Availability Zones?
- Why is it important to run EC2 instances across multiple AZs?
- How do regional AWS services enhance high availability?
- What is the purpose of Amazon CloudFront?
- What are edge locations in AWS?
- What is AWS Outposts?
- How do Availability Zones within AWS Regions contribute to disaster recovery and high availability?
- How do AWS Edge locations and Amazon CloudFront improve content delivery?
- What is an API in the context of AWS?
- What is the primary method of interacting with AWS services?
- What are the main ways to interact with AWS services?
- Why is automation important in cloud deployment?
- What is the primary advantage of using AWS Elastic Beanstalk over manual methods like the AWS Management Console?
- What is AWS Elastic Beanstalk used for?
- How does AWS CloudFormation help in managing AWS resources?
- What are the main components of AWS Global Infrastructure?
- Which AWS services automatically run across multiple Availability Zones?
- What is the recommended best practice for deploying infrastructure in AWS?
- What is Amazon EC2?
- What is Amazon EC2 and its primary benefits?
- What is a Security Group in EC2?
- What are the four main purchasing options for EC2 instances, and what are their key characteristics?
- How does EC2 pricing work?
- What is an Amazon Machine Image (AMI)?
- How does EC2 integrate with other AWS services?
- What are the different computing models available in AWS?
- What is an instance and its use cases?
- What are containers and their advantages?
- What is serverless computing and its use cases? 
- When would you consider a hybrid deployment model?
- What are some of the popular AWS computing services?
- What is AWS Lambda?
- What is Amazon ECS?
- How does AWS Fargate differ from Amazon EC2?
- What are the benefits of using AWS Elastic Beanstalk?
- How does EC2 demonstrate elasticity?
- What level of control do users have over EC2 instances?
- How does EC2 integrate with other AWS services?
- What security features does Amazon EC2 provide?
- What are the main architectural components of Amazon EC2?
- What factors should you consider when choosing a region for your EC2 instance?
- What is the purpose of a VPC in Amazon EC2?
- What are subnets and their role in EC2?
- How do security groups protect your EC2 instances?
- What are the steps to launch an EC2 instance?
- What is the importance of tagging in EC2?
  
- Can you automate EC2 scaling? Yes. The auto scaling function of EC2 can only scale horizontally; it cannot scale vertically. This indicates that while the quantity of EC2 can be created and terminated automatically, the scaling of already-existing EC2 cannot be done so automatically; instead, the user must take action.
  
- What security features does EC2 offer?
- What are the benefits of using AMIs?
