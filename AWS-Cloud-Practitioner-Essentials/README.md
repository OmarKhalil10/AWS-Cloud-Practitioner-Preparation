# Prepare for the AWS Certified Cloud Practitioner (CLF-C01) Certification Exam

# AWS Certified Cloud Practitioner Track Modules

* Module 1: Introduction to Amazon web services
* Module 2: Compute in the cloud
* Module 3: Global infrastructure and reliability
* Module 4: Networking
* Module 5: Storage and databases
* Module 6: Security
* Module 7: Monitoring and analytics
* Module 8: Pricing and support
* Module 9: Introduction
* Module 10: The cloud journey
* Module 11: AWS certified cloud practitioner basics
* Final assessment

# Module 1: Introduction to Amazon web services

## 1- Introduction

1. Introduction
2. Cloud Computing
3. Quiz

## What is a client-server model?

In computing, a client can be a web browser or desktop application that a person interacts with to make requests to computer servers. A server can be services such as Amazon Elastic Compute Cloud (Amazon EC2), a type of virtual server.

![Client-Server-Arch](/Images/AWS-Cloud-Practitioner-Essentials/Client-Server-Arch.png)

> For example, suppose that a client makes a request for a news article, the score in an online game, or a funny video. The server evaluates the details of this request and fulfills it by returning the information to the client.

# Cloud Computing

## Deployment models for cloud computing

When selecting a cloud strategy, a company must consider factors such as required cloud application components, preferred resource management tools, and any legacy IT infrastructure requirements.

### The three cloud computing deployment models are:

1. cloud-based
2. on-premises
3. hybrid

**1- cloud-based**

- Run all parts of the application in the cloud.
- Migrate existing applications to the cloud.
- Design and build new applications in the cloud.

In a **cloud-based deployment model**, you can migrate existing applications to the cloud, or you can design and build new applications in the cloud. You can build those applications on low-level infrastructure that requires your IT staff to manage them. Alternatively, you can build them using higher-level services that reduce the management, architecting, and scaling requirements of the core infrastructure.


> For example, a company might create an application consisting of virtual servers, databases, and networking components that are fully based in the cloud.

**2- on-premises**

- Deploy resources by using virtualization and resource management tools.
- Increase resource utilization by using application management and virtualization technologies.

**On-premises deployment** is also known as a **private cloud deployment**. In this model, resources are deployed on premises by using virtualization and resource management tools.

> For example, you might have applications that run on technology that is fully kept in your on-premises data center. Though this model is much like legacy IT infrastructure, its incorporation of application management and virtualization technologies helps to increase resource utilization.

## 2- hybrid

- Connect cloud-based resources to on-premises infrastructure.
- Integrate cloud-based resources with legacy IT applications.

In a **hybrid deployment**, **cloud-based** resources are connected to **on-premises** infrastructure. You might want to use this approach in a number of situations.

> For example, you have legacy applications that are better maintained on premises, or government regulations require your business to keep certain records on premises.

> For example, suppose that a company wants to use cloud services that can automate batch data processing and analytics. However, the company has several legacy applications that are more suitable on premises and will not be migrated to the cloud. With a hybrid deployment, the company would be able to keep the legacy applications on premises while benefiting from the data and analytics services that run in the cloud.

## Benefits of cloud computing

Consider why a company might choose to take a particular cloud computing approach when addressing business needs.

![Benefits of cloud computing](/Images/AWS-Cloud-Practitioner-Essentials/Benefits%20of%20cloud%20computing.png)

### 1- Trade upfront expense for variable expense

Upfront expense refers to data centers, physical servers, and other resources that you would need to invest in before using them. Variable expense means you only pay for computing resources you consume instead of investing heavily in data centers and servers before you know how you’re going to use them.

By taking a cloud computing approach that offers the benefit of variable expense, companies can implement innovative solutions while saving on costs.

### 2- Stop spending money to run and maintain data centers

Computing in data centers often requires you to spend more money and time managing infrastructure and servers.

A benefit of cloud computing is the ability to focus less on these tasks and more on your applications and customers.

### 3- Stop guessing capacity

With cloud computing, you don’t have to predict how much infrastructure capacity you will need before deploying an application.

> For example, you can launch Amazon EC2 instances when needed, and pay only for the compute time you use. Instead of paying for unused resources or having to deal with limited capacity, you can access only the capacity that you need. You can also scale in or scale out in response to demand.

### 4- Benefit from massive economies of scale

By using cloud computing, you can achieve a lower variable cost than you can get on your own.

Because usage from hundreds of thousands of customers can aggregate in the cloud, providers, such as AWS, can achieve higher economies of scale. The economy of scale translates into lower pay-as-you-go prices.

### 5- Increase speed and agility

The flexibility of cloud computing makes it easier for you to develop and deploy applications.

This flexibility provides you with more time to experiment and innovate. When computing in data centers, it may take weeks to obtain new resources that you need. By comparison, cloud computing enables you to access new resources within minutes.

### 6- Go global in minutes

The global footprint of the AWS Cloud enables you to deploy applications to customers around the world quickly, while providing them with low latency. This means that even if you are located in a different part of the world than your customers, customers are able to access your applications with minimal delays.

Later in this course, you will explore the AWS global infrastructure in greater detail. You will examine some of the services that you can use to deliver content to customers around the world.

## Quiz

What is cloud computing?

- [x] On-demand delivery of IT resources and applications through the internet with pay-as-you-go pricing

What is another name for on-premises deployment?

- [x] Private cloud deployment

# Module 2: Compute in the Cloud

1. Introduction
2. Amazon EC2 instance types
3. Amazon EC2 pricing
4. Scaling Amazon EC2
5. Directing traffic with Elastic Load Balancing
6. Messaging and Queuing
7. Additional compute services
8. Summary
9. Quiz
## Learning objectives

In this module, you will learn how to:

* Describe the benefits of Amazon EC2 at a basic level.
* Identify the different Amazon EC2 instance types.
* Differentiate between the various billing options for Amazon EC2.
* Summarize the benefits of Amazon EC2 Auto Scaling.
* Summarize the benefits of Elastic Load Balancing.
* Give an example of the uses for Elastic Load Balancing.
* Summarize the differences between Amazon Simple Notification Service (Amazon SNS) and Amazon Simple Queue Service (Amazon SQS).
* Summarize additional AWS compute options.

## Introduction
### Amazon Elastic Compute Cloud (Amazon EC2)

Amazon Elastic Compute Cloud (Amazon EC2) provides secure, resizable compute capacity in the cloud as Amazon EC2 instances.

Imagine you are responsible for the architecture of your company's resources and need to support new websites. With traditional on-premises resources, you have to do the following:

* Spend money upfront to purchase hardware.
* Wait for the servers to be delivered to you.
* Install the servers in your physical data center.
* Make all the necessary configurations.

By comparison, with an Amazon EC2 instance you can use a virtual server to run applications in the AWS Cloud.

* You can provision and launch an Amazon EC2 instance within minutes.
* You can stop using it when you have finished running a workload.
* You pay only for the compute time you use when an instance is running, not when it is stopped or terminated.
* You can save costs by paying only for server capacity that you need or want.

### How Amazon EC2 works

![How Amazon EC2 works](/Images/AWS-Cloud-Practitioner-Essentials/How%20Amazon%20EC2%20works.png)

### 1- Launch

First, you launch an instance. Begin by selecting a template with basic configurations for your instance. These configurations include the operating system, application server, or applications. You also select the instance type, which is the specific hardware configuration of your instance.

As you are preparing to launch an instance, you specify security settings to control the network traffic that can flow into and out of your instance. Later in this course, we will explore Amazon EC2 security features in greater detail.

### 2- Connect

Next, connect to the instance. You can connect to the instance in several ways. Your programs and applications have multiple different methods to connect directly to the instance and exchange data. Users can also connect to the instance by logging in and accessing the computer desktop

### 3- Use

After you have connected to the instance, you can begin using it. You can run commands to install software, add storage, copy and organize files, and more.

## Amazon EC2 instance types

[Amazon EC2 instance types](https://aws.amazon.com/ec2/instance-types/) are optimized for different tasks. When selecting an instance type, consider the specific needs of your workloads and applications. This might include requirements for compute, memory, or storage capabilities.

### What we will learn

![Amazon EC2 instance types](/Images/AWS-Cloud-Practitioner-Essentials/Amazon%20EC2%20instance%20types.png)

### 1- General purpose instances

General purpose instances provide a balance of compute, memory, and networking resources. You can use them for a variety of workloads, such as:

* application servers
* gaming servers
* backend servers for enterprise applications
* small and medium databases

> Suppose that you have an application in which the resource needs for compute, memory, and networking are roughly equivalent. You might consider running it on a general purpose instance because the application does not require optimization in any single resource area.

### 2- Compute optimized instances

Compute optimized instances are ideal for compute-bound applications that benefit from high-performance processors. Like general purpose instances, you can use compute optimized instances for workloads such as web, application, and gaming servers.

> However, the difference is compute optimized applications are ideal for high-performance web servers, compute-intensive applications servers, and dedicated gaming servers. You can also use compute optimized instances for batch processing workloads that require processing many transactions in a single group.

### 3- Memory optimized instances

Memory optimized instances are designed to deliver fast performance for workloads that process large datasets in memory. In computing, memory is a temporary storage area. It holds all the data and instructions that a central processing unit (CPU) needs to be able to complete actions. Before a computer program or application is able to run, it is loaded from storage into memory. This preloading process gives the CPU direct access to the computer program.



> Suppose that you have a workload that requires large amounts of data to be preloaded before running an application. This scenario might be a high-performance database or a workload that involves performing real-time processing of a large amount of unstructured data. In these types of use cases, consider using a memory optimized instance. Memory optimized instances enable you to run workloads with high memory needs and receive great performance.


### 4- Accelerated computing instances

Accelerated computing instances use hardware accelerators, or coprocessors, to perform some functions more efficiently than is possible in software running on CPUs. Examples of these functions include floating-point number calculations, graphics processing, and data pattern matching.

> In computing, a hardware accelerator is a component that can expedite data processing. Accelerated computing instances are ideal for workloads such as graphics applications, game streaming, and application streaming.


### 5- Storage optimized instances

Storage optimized instances are designed for workloads that require high, sequential read and write access to large datasets on local storage. Examples of workloads suitable for storage optimized instances include distributed file systems, data warehousing applications, and high-frequency online transaction processing (OLTP) systems.



In computing, the term input/output operations per second (IOPS) is a metric that measures the performance of a storage device. It indicates how many different input or output operations a device can perform in one second. Storage optimized instances are designed to deliver tens of thousands of low-latency, random IOPS to applications.

> You can think of input operations as data put into a system, such as records entered into a database. An output operation is data generated by a server. An example of output might be the analytics performed on the records in a database. If you have an application that has a high IOPS requirement, a storage optimized instance can provide better performance over other instance types not optimized for this kind of use case.

### Quiz

Match each description to an Amazon EC2 instance type.

![Quiz Amazon EC2 instance types](/Images/AWS-Cloud-Practitioner-Essentials/match-quiz%20Amazon%20EC2%20instance%20types.png)

## Amazon EC2 pricing

With Amazon EC2, you pay only for the compute time that you use. Amazon EC2 offers a variety of pricing options for different use cases. For example, if your use case can withstand interruptions, you can save with Spot Instances. You can also save by committing early and locking in a minimum level of use with Reserved Instances.

### 1- On-Demand

On-Demand Instances are ideal for short-term, irregular workloads that cannot be interrupted. No upfront costs or minimum contracts apply. The instances run continuously until you stop them, and you pay for only the compute time you use.

Sample use cases for On-Demand Instances include developing and testing applications and running applications that have unpredictable usage patterns. On-Demand Instances are not recommended for workloads that last a year or longer because these workloads can experience greater cost savings using Reserved Instances.

### 2- Amazon EC2 Savings Plans

AWS offers Savings Plans for several compute services, including Amazon EC2. Amazon EC2 Savings Plans enable you to reduce your compute costs by committing to a consistent amount of compute usage for a 1-year or 3-year term. This term commitment results in savings of up to 72% over On-Demand costs.

Any usage up to the commitment is charged at the discounted Savings Plan rate (for example, $10 an hour). Any usage beyond the commitment is charged at regular On-Demand rates.

### 3- Reserved Instances

Reserved Instances are a billing discount applied to the use of On-Demand Instances in your account. You can purchase Standard Reserved and Convertible Reserved Instances for a 1-year or 3-year term, and Scheduled Reserved Instances for a 1-year term. You realize greater cost savings with the 3-year option.

At the end of a Reserved Instance term, you can continue using the Amazon EC2 instance without interruption. However, you are charged On-Demand rates until you do one of the following:

Terminate the instance.
Purchase a new Reserved Instance that matches the instance attributes (instance type, Region, tenancy, and platform).

### 4- Spot Instances

Spot Instances are ideal for workloads with flexible start and end times, or that can withstand interruptions. Spot Instances use unused Amazon EC2 computing capacity and offer you cost savings at up to 90% off of On-Demand prices.

Suppose that you have a background processing job that can start and stop as needed (such as the data processing job for a customer survey). You want to start and stop the processing job without affecting the overall operations of your business. If you make a Spot request and Amazon EC2 capacity is available, your Spot Instance launches. However, if you make a Spot request and Amazon EC2 capacity is unavailable, the request is not successful until capacity becomes available. The unavailable capacity might delay the launch of your background processing job.

After you have launched a Spot Instance, if capacity is no longer available or demand for Spot Instances increases, your instance may be interrupted. This might not pose any issues for your background processing job. However, in the earlier example of developing and testing applications, you would most likely want to avoid unexpected interruptions. Therefore, choose a different EC2 instance type that is ideal for those tasks.

### 5- Dedicated Hosts

Dedicated Hosts are physical servers with Amazon EC2 instance capacity that is fully dedicated to your use.

You can use your existing per-socket, per-core, or per-VM software licenses to help maintain license compliance. You can purchase On-Demand Dedicated Hosts and Dedicated Hosts Reservations. Of all the Amazon EC2 options that were covered, Dedicated Hosts are the most expensive.

## Scaling Amazon EC2

### Scalability

Scalability involves beginning with only the resources you need and designing your architecture to automatically respond to changing demand by scaling out or in. As a result, you pay for only the resources you use. You don’t have to worry about a lack of computing capacity to meet your customers’ needs.

If you wanted the scaling process to happen automatically, which AWS service would you use? The AWS service that provides this functionality for Amazon EC2 instances is **Amazon EC2 Auto Scaling**.

### Amazon EC2 Auto Scaling

If you’ve tried to access a website that wouldn’t load and frequently timed out, the website might have received more requests than it was able to handle. This situation is similar to waiting in a long line at a coffee shop, when there is only one barista present to take orders from customers.

**Amazon EC2 Auto Scaling** enables you to **automatically add or remove Amazon EC2 instances** in response to changing application demand. By automatically scaling your instances **in and out** as needed, you are able to maintain a greater sense of application availability.

Within Amazon EC2 Auto Scaling, you can use two approaches:

1. dynamic scaling
2. predictive scaling

**Dynamic scaling**: responds to changing demand.

**Predictive scaling**: automatically schedules the right number of Amazon EC2 instances based on predicted demand.

> When you create an Auto Scaling group, you can set the minimum number of Amazon EC2 instances. **The minimum capacity** is the number of Amazon EC2 instances that launch immediately after you have created the Auto Scaling group. In this example, the **Auto Scaling group** has a minimum capacity of one Amazon EC2 instance.

### NOTE
> If you do not specify the desired number of Amazon EC2 instances in an Auto Scaling group, the desired capacity defaults to your minimum capacity.

### maximum capacity

Example, you might configure the Auto Scaling group to scale out in response to increased demand, but only to a maximum of four Amazon EC2 instances.

## Directing traffic with Elastic Load Balancing

**Elastic Load Balancing** is the AWS service that automatically distributes incoming application traffic across multiple resources, such as Amazon EC2 instances.

A load balancer acts as a single point of contact for all incoming web traffic to your Auto Scaling group. This means that as you add or remove Amazon EC2 instances in response to the amount of incoming traffic, these requests route to the load balancer first. Then, the requests spread across multiple resources that will handle them. For example, if you have multiple Amazon EC2 instances, Elastic Load Balancing distributes the workload across the multiple instances so that no single instance has to carry the bulk of it.

> Although Elastic Load Balancing and Amazon EC2 Auto Scaling are separate services, they work together to help ensure that applications running in Amazon EC2 can provide high performance and availability.

## Messaging and queuing

### Monolithic applications and microservices


**monolithic application**:

In this approach to application architecture, if a single component fails, other components fail, and possibly the entire application fails.

> To help maintain application availability when a single component fails, you can design your application through a microservices approach.

In a microservices approach, application components are **loosely coupled**. In this case, if a single component fails, the other components continue to work because they are communicating with each other. **The loose coupling prevents the entire application from failing**.

When designing applications on AWS, you can take a microservices approach with services and components that fulfill different functions.

**Two services facilitate application integration**:

* Amazon Simple Notification Service (**Amazon SNS**)
* Amazon Simple Queue Service (**Amazon SQS**)

### 1- Amazon Simple Notification Service (Amazon SNS)

It is a **publish/subscribe** service. Using Amazon SNS topics, a **publisher publishes messages to subscribers**.

In Amazon SNS, subscribers can be:

* web servers
* email addresses
* AWS Lambda functions
* other options

### 2- Amazon Simple Queue Service (Amazon SQS)

Amazon Simple Queue Service (Amazon SQS) is a **message queuing service**.

Using Amazon SQS, you can send, store, and receive messages between software components, without losing messages or requiring other services to be available. In Amazon SQS, an application sends messages into a queue. A **user or service retrieves a message from the queue, processes it, and then deletes it from the queue**.

**How it deals with messages**:

1. Retrieve
2. Process
3. Delete

## Additional compute services

### 1- Serverless computing [Focus on Code]

As mentioned earlier If you have applications that you want to run in Amazon EC2, you
must do the following:

1. Provision instances (virtual servers)
2. Upload your code
3. Continue to manage the instances while your application is running

The term **“serverless”** means that your code runs on servers, but **you do not need to provision or manage these servers**. With serverless computing, you can focus more on innovating new products and features instead of maintaining servers.

> An AWS service for **serverless** computing is **AWS Lambda**.

### AWS Lambda

AWS Lambda is a service that **lets you run code without needing to provision or manage servers**.

While using AWS Lambda, you **pay only for the compute time that you consume**. Charges apply only when your code is running. You can also run code for virtually any type of application or backend service, all with **zero administration**.

> For example, a simple Lambda function might involve automatically resizing uploaded images to the AWS Cloud. In this case, the function triggers when uploading a new image.

### How AWS Lambda works

1. You upload your code to Lambda

2. You set your code to trigger from an event source, such as AWS services, mobile applications, or HTTP endpoints

3. Lambda runs your code only when triggered

4. You pay only for the compute time that you use

NOTE:

> In AWS, you can also build and run containerized applications.

### Containers

Containers provide you with a standard way to **package your application's code and dependencies into a single object**

You can also use containers for processes and workflows in which there are **essential requirements for security, reliability, and scalability**

### Amazon Elastic Container Service (**Amazon ECS**)

Amazon Elastic Container Service (Amazon ECS) is a highly scalable, high-performance container management system that enables you to run and scale containerized applications on AWS.

Amazon ECS **supports Docker containers**.

### Docker

It is a software platform that **enables you to build, test, and deploy applications** quickly. AWS supports the use of the following:

1. source Docker **Community** Edition
2. **subscription-based** Docker Enterprise Edition

> With Amazon ECS, you can use API calls to launch and stop Docker-enabled applications.

### Amazon Elastic Kubernetes Service (**Amazon EKS**)

Amazon Elastic Kubernetes Service (Amazon EKS) is a fully managed service that you can **use to run Kubernetes on AWS**.

### Kubernetes

It is open-source software that **enables you to deploy and manage containerized applications at scale**. A large community of volunteers maintains Kubernetes, and AWS actively works together with the Kubernetes community. As new features and functionalities release for Kubernetes applications, you can **easily apply these updates to your applications managed by Amazon EKS**.

### AWS Fargate [Serverless Compute Engine]

AWS Fargate is a **serverless compute engine for containers**

It works with both **Amazon ECS and Amazon EKS**.

When using AWS Fargate, you **do not need to provision or manage servers**. AWS Fargate manages your server infrastructure for you. You can focus more on innovating and developing your applications, and you pay only for the resources that are required to run your containers.

## Summary

In Module 2, you learned about the following concepts:

* Amazon EC2 instance types and pricing options
* Amazon EC2 Auto Scaling
* Elastic Load Balancing
* AWS services for messaging, containers, and serverless computing
## Quiz

1. You want to use an Amazon EC2 instance for a batch processing workload. What would be the best Amazon EC2 instance type to use?

- [x] Compute optimized

2. What are the contract length options for Amazon EC2 Reserved Instances? (Select TWO.)


- [x] 1 year

- [x] 3 years

> Reserved Instances require a commitment of either 1 year or 3 years. The 3-year option offers a larger discount.


3. ou have a workload that will run for a total of 6 months and can withstand interruptions. What would be the most cost-efficient Amazon EC2 purchasing option?

- [x] Spot Instance

4. Which process is an example of Elastic Load Balancing?

- [x]
Ensuring that no single Amazon EC2 instance has to carry the full workload on its own

5. You want to deploy and manage containerized applications. Which service should you use?

- [x] Amazon Elastic Kubernetes Service (Amazon EKS)
# Module 3: Global infrastructure and reliability
## Learning objectives

In this module, you will learn how to:

* Summarize the benefits of the AWS Global Infrastructure.
* Describe the basic concept of Availability Zones.
* Describe the benefits of Amazon CloudFront and edge locations.
* Compare different methods for provisioning AWS services.

## Building a global footprint

To understand the AWS global infrastructure, consider the coffee shop. If an event such as a parade, flood, or power outage impacts one location, customers can still get their coffee by visiting a different location only a few blocks away.

> This is similar to how the AWS global infrastructure works.
## AWS global infrastructure

## Selecting a Region

When determining the right Region for your services, data, and applications, consider the following four business factors.

![Region Selection Factors](/Images/AWS-Cloud-Practitioner-Essentials/Region%20Selection%20Factors.png)

### 1- Compliance with data governance and legal requirements

Depending on your company and location, you might need to run your data out of specific areas. For example, if your company requires all of its data to reside within the boundaries of the UK, you would choose the London Region.

Not all companies have location-specific data regulations, so you might need to focus more on the other three factors.

### 2- Proximity to your customers

Selecting a Region that is close to your customers will help you to get content to them faster. For example, your company is based in Washington, DC, and many of your customers live in Singapore. You might consider running your infrastructure in the Northern Virginia Region to be close to company headquarters, and run your applications from the Singapore Region.

### 3- Available services within a Region

Sometimes, the closest Region might not have all the features that you want to offer to customers. AWS is frequently innovating by creating new services and expanding on features within existing services. However, making new services available around the world sometimes requires AWS to build out physical hardware one Region at a time.

Suppose that your developers want to build an application that uses **Amazon Braket (AWS quantum computing platform)**. As of this course, Amazon Braket is not yet available in every AWS Region around the world, so your developers would have to run it in one of the Regions that already offers it.

### 4- Pricing

Suppose that you are considering running applications in both the United States and Brazil. The way Brazil’s tax structure is set up, it might cost 50% more to run the same workload out of the São Paulo Region compared to the Oregon Region. You will learn in more detail that several factors determine pricing, but for now know that the cost of services can vary from Region to Region.
## Availability Zones

An Availability Zone is a **single data center or a group of data centers within a Region**. Availability Zones are located tens of miles apart from each other. This is close enough to have low latency (the time between when content requested and received) between Availability Zones. However, if a disaster occurs in one part of the Region, they are distant enough to reduce the chance that multiple Availability Zones are affected.

### Quiz

Which statement best describes an Availability Zone?

- [x] A single data center or group of data centers within a Region

## Edge locations

An **edge location** is a **site** that Amazon CloudFront uses to **store cached copies of your content closer to your customers** for **faster delivery**.

### How to provision AWS resources

### Ways to interact with AWS services

1. AWS Management Console
2. AWS Command Line Interface (**CLI**)
3. AWS Software Development Kits (**SDKs**)



Interaction Way | Description |
---------|----------|
**AWS Management Console** | The AWS Management Console is a web-based interface for accessing and managing AWS services. You can quickly access recently used services and search for other services by name, keyword, or acronym. The console includes wizards and automated workflows that can simplify the process of completing tasks. You can also use the AWS Console mobile application to perform tasks such as monitoring resources, viewing alarms, and accessing billing information. Multiple identities can stay logged into the AWS Console mobile app at the same time. |
**AWS Command Line Interface (CLI)** | To save time when making API requests, you can use the AWS Command Line Interface (AWS CLI). AWS CLI enables you to control multiple AWS services directly from the command line within one tool. AWS CLI is available for users on Windows, macOS, and Linux. By using AWS CLI, you can automate the actions that your services and applications perform through scripts. For example, you can use commands to launch an Amazon EC2 instance, connect an Amazon EC2 instance to a specific Auto Scaling group, and more. |
**AWS Software Development Kits (SDKs)** | Another option for accessing and managing AWS services is the software development kits (SDKs). SDKs make it easier for you to use AWS services through an API designed for your programming language or platform. SDKs enable you to use AWS services with your existing applications or create entirely new applications that will run on AWS. To help you get started with using SDKs, AWS provides documentation and sample code for each supported programming language. Supported programming languages include C++, Java, .NET, and more. |


## AWS Elastic Beanstalk

With AWS Elastic Beanstalk, you provide code and configuration settings, and Elastic Beanstalk deploys the resources necessary to perform the following tasks:

* Adjust capacity
* Load balancing
* Automatic scaling
* Application health monitoring

## AWS CloudFormation

With AWS CloudFormation, you can treat your **infrastructure as code**. This means that you can build an environment by writing lines of code instead of using the AWS Management Console to individually provision resources.

AWS CloudFormation **provisions your resources in a safe, repeatable manner**, enabling you to frequently build your infrastructure and applications **without having to perform manual actions**. It determines the right operations to perform when **managing your stack and rolls back changes** automatically **if it detects errors**.

## Summary

In Module 3, you learned about the following concepts:

* AWS Regions and Availability Zones
* Edge locations and Amazon CloudFront
* The AWS Management Console, AWS CLI, and SDKs
* AWS Elastic Beanstalk
* AWS CloudFormation

## Quiz

1. Which statement is TRUE for the AWS global infrastructure?

- [x] A Region consists of two or more Availability Zones.

2. Which factors should be considered when selecting a Region? (Select TWO.)

- [x] Compliance with data governance and legal requirements

- [x] Proximity to your customers

3. Which statement best describes Amazon CloudFront?

- [x] A global content delivery service

**Notes**:

### AWS Outposts
It is a service that enables you to run **infrastructure in a hybrid cloud** approach.

4. Which site does Amazon CloudFront use to cache copies of content for faster delivery to users at any location?

- [x] Edge location

































































