# Prepare for the AWS Certified Cloud Practitioner (CLF-C01) Certification Exam

# AWS Cloud Core Services (Technologies)

# 1- Compute

1. EC2
2. Elastic Beanstalk
3. Elastic Load Balancing
4. Lambda
5. Lightsail
6. Deploying and Operating in AWS
7. AWS Global Infrastructure

## 1- EC2 (Amazon Elastic Compute Cloud)

- Virtual server runing on AWS.
- Configurable by number of **virtual** **CPUs**, GBs of **RAM**, Size/Type of **Storage**, and **network** speed.
- Pay-as-you-go (Only charged for what you use, when you use it).
- Deploy extremely **scalable** and **reliable** virtual **servers** within minutes.

## 2- Elastic Beanstalk

- Handles the deployment process including (**capacity provisioning**, **load balancing**, **auto scaling**, **health monitoring**).
- Accommodates services deployed using **Java**, **.Net**, **PHP**, **Node.js**, **Python**, **Ruby**, **Go**, and **Docker**.
- You retain **Control** over **Resources** at all time.
- **Free** to use.
- Pay **only** for other AWS **resources** consumed to **deploy**.

## Advantages

- Autoscaling
- Complete freedom to select AWS resources like EC2 instance you want to use.
- Allows **manual** **management** of infrastructure.
- Provisions and operates the infrastructure for you so you only focus on coding.

## 3- Elastic Load Balancing

> Performs automatic **distribution** of **incomig traffic** across multiple **replicated servers** so no single server is **overloaded**.
- **Fault-tolerant**.
- **Scalable** and **Secure**.
- Monitor **health** of **servers** so if one goes **down**, **standby** servers will **join** the **service**.

## 4- Lambda

- Runs code (Lambda function) in **response to event**.
- **Automatically** runs uploaded code and scales applications.
- Pay only for **the time** the code is **running** and each **event trigger**.
- No need to provision and maintain servers Lambda will do that and you only need to focus on code.

## 5- Lightsail

- **Preconfigured** and **ready-to-use**, Operating Systems (**OS**), **Web App**, and **Development Stack**.
- **Scalable** with your project **growth**.
- **Cost-effictive** monthly fees.
- **One-Click-to-launch** services
- **Easy** to quickly **deploy** **projects**.

## 6- Deploying and operating in AWS

> The following are the **AWS API's** that are made to help you to **deploy** and **manage** your **AWS Cloud Infrastructure**.

1. AWS Management **Console**.
2. AWS Command-Line Interface (**CLI**).
3. AWS Software Development Kits (**SDKs**).

## 1- AWS Management Console

- **Graphical interface** (**GUI**) that supports most AWS services.
- **User-friendly** and easy to **navigate**.
- Can access **billing statements**, **launch** new **services**, check out **health** of web apps, and so on.

## 2- AWS Command-Line Interface (**CLI**)

- Access AWS services via **Command Line**.
-Command Line: access and change resources via **Text-Based** command entry.
- Programming language agnostic.
- Create **scripts** to run on **AWS**.

## 3- AWS Software Development Kits (**SDKs**)

- Incorporate connectivity and functionality of wide range of AWS services into your code.

- Deploy AWS services and resources using a variety of popular programming languages like **Java**, **.Net**, **PHP**, **Node.js**, **Python**, **Ruby**.
- Use AWS resources in exsisting applications.

# Infrastructure as Code (IAC)

- Deploy resources into AWS Cloud using code!

- Some **examples** of AWS services that utilize Infrastructure as Code (IAC)

|Examples of services that supports (**IAC**)|
:------:
Elastic Beanstalk (**EB**)|
AWS Lambda|
AWS CloudFormation|

## 7- AWS Global Infrastructure

## AWS Availability Zones (**AZs**)

- AWS **data canters** aournd the world.
- Completely **Independant** of each other in **network and power source**.
- Currently almost **six dozen** AZs around the world.

## Regions

- Made up of two (**2**) or more **Availabiliy Zones** (**AZs**).

- Currently **two dozen** AWS Regions around the world.

## High Availability

Metric| Meaning
---------|----------|
 High Available | **resources** may have **duplicate copies** in **multiple AZs** or even **Regions**
 Resiliency | Ability to provide **uninterrupted performance**, even **during** natural **disasters**
 Redundancy | Having muliple **copies** of data in **different** **data centers** |
Well-Architected| Protect against **Downtimes** caused by **natural disasters** or **power outage**|

## Questions

1. **An hour after Teixeira Gifts posts a 50% off holiday sale, its server goes down from the amount of traffic to the website. How would using elastic load balancing have prevented this issue?**

> **by automatically distributing traffic across multiple servers**
>
>This keeps any one server from being overwhelmed by traffic.

2. **You are just starting out with AWS but do not have technical know-how. What AWS service can you use to create websites and run your business's software?**

> **AWS Lightsail**
>
> You can also deploy simple web applications and spin up test environments.

3. **If you want to deploy AWS services by using a variety of popular programming languages, what service would you use?**

> AWS Software Development Kits
>
> These let you deploy AWS services and resources using a variety of popular programming languages.

4. **When would you find it most beneficial to use Elastic Beanstalk?**

> **when you are spending more time configuring than coding**
>
> Elastic Beanstalk handles the deployment process, leaving you time for the more important coding.

5. **As a general rule, what region should you select to host your AWS cloud infrastructure?**

> **the closest region to you geographically**
>
> Doing this reduces network latency for your end users.

6. **Why is Amazon Elastic Compute Cloud (EC2) one of the most widely used services in AWS?**

> **It lets you launch applications and servers without upfront financial commitments.**
>
> This capability eliminates the time and expense of purchasing any physical servers that can be obsolete before they are even installed.

# 2- Storage

1. S3 (**Simple Storage Service**)
2. Elastic Block Store (**EBS**)
3. Snowball
4. Storage Gateway

## 1- S3 (**Simple Storage Service**)

- **Object storage service**: storing each file as **separate entity** (_Object_).
- High **Availability**, **Security**, and **performance**.
- Scalable.
- Charged only for (what you use) - **Pay-as-you-go**.
- 99.999999999% **Durable**. (which means there is almost no chance of the data become **corrupted**).
- Upload files (objects) of all sizes (**0 byte ~ 5 terabytes**).
- Variety of uses: Use uploaded files for **websites**, **mobile apps**, **backup** and **archiving**, **enterprise application**, **IOT** devices, **big data analytics**.
- **Easy-to-use** management features to **fine-tune** access control.

### S3 Storage Classes

1. Standard
2. Intelligent-Tiering
3. Standard-Infrequent Access
4. One Zone-infrequent Access
5. Glacier
6. Glacier Deep Archive

> You can **setup S3 lifecycle policies** which will **automatically** **transfer** files form one storage class **to cheaper one** after certain number of days.

## 2- Elastic Block Store (**EBS**)

- Raw, unformatted block device attached to an EC2 instance.
- Can add multiple EBS volumes to one EC2 instance.
- Use as **file system** or **hard drive**.
- Dynamically change **configurations** to attached volumes via **Management Console**.
- Automatically **replicated** within it's **availability zone**.
- It's high available and durable.
- Different types of EBS storage for your needs and budgets.
- Presistent block storage volumes: **do not disappear** when EC2 instances are rebooted.
- Can be encrypted.
- Exist independently of EC2 instances so can be moved to other instances.

> You can think of EBS volumes as **external hard drives for your virtual servers**.

## 3- Snowball

- Data migration tool.
- **Hardware Solution**: AWS will physically ship you a **Snowball** to move your data onto and ship back.
- You can move **50 terabytes** with a **regular Snowball** up to **100 petabytes** with a **Snowmobile** (45-foot-long shipping container).

> **Usage Fee**
>
> Free for **10 days** of onsite usage; extra usage fees for every extra day you keep it.
>
> Storage fee: free for date trasnsferred to S3 (but you will pay after data transfer for data storage in S3).
>
> Snowmobile: **Expensive!**.
>
> Service fee per job starting at **$200** for **50 terabytes** of data to **$320** for **80 terabytes** of data.

## 4- Storage Gateway (Hybrid Storage Solution)

<br>

> It connects you **on-premises** storage with **AWS Cloud Storage**, providing a **Hybrid Storage Solution**.

### Common challenges between on-premises environments and the AWS Cloud

<br>

![Common challenges between on-premises environments and the AWS Cloud](/Images/3-%20Core%20Services/common-challenges-between-on-premises-environments-and-the-AWS-Cloud.png)

### High-level architecture of Storage Gateway

<br>

![High-level architecture of Storage Gateway](/Images/3-%20Core%20Services/High-level-architecture-of-storage-gateway.png)


### Three common use cases of Storage Gateway, which can be deployed across various stages of the cloud adoption journey

<br>

![Common use cases of Storage Gateway](/Images/3-%20Core%20Services/aws-storage-gateway-hybrid-cloud-storage-use-cases-blog-1024x489.png)


### Storage Gateway is made up of three gateway types

<br>

![Three gateway types](/Images/3-%20Core%20Services/SGW-family.png)


## AWS Storage Gateway: 1- File Gateway

- **Asynchronously** updates objects to S3 as local files are updated.
- Local **Cache** to provide **low-latency** access to recently accessed files.

## AWS Storage Gateway: 2- Volume Gateway

- Upload files in **blocks** (like virual hard drives).
- Asynchronously **backed up** as **Point-in-time** snapshots and stored as **EBS** Snapshot (Elastic Block Store Snapshot).

### Types of **Volume Gateway**

> We have 2 types of Volume Gateway

Types | Description |
:-------:|:-------:|
**Stored Volume** | Complete copy **on-premises**; sends snapshots to AWS |
**Cached Volume**| Keeps most **recently accessed data** on-premises; **complete copy on AWS** |

## AWS Storage Gateway: 3- Tape Gateway

- Uses **existing tape-based backup infrastructure** to back up to **virtual tapes** on **S3**.

- Data **stored locally** then **asynchronously** uploaded to **S3**.

- Data can be **archived** using Amazon **Glacier**.

## AWS Storage Gateway Pricing

- You will pay for storage and to access the stored data.

- The quicker you can access the data, the more expensive the solution is.

### Example

- Data stored via **tape gateway** is much **Cheaper** saved to **S3 Glacier Deep Archive** than **S3 Glacier**.

**Why?**

> Because data retrieval take loger time.

## Questions

1. **Which AWS Storage Gateway functions like virtual hard drives that upload files in blocks?**

> **Volume Gateway**
>
> Files are uploaded as blocks, not as individual files.

2. **What does it mean that Amazon Simple Storage Service (S3) is scalable?**

> **It provides the ability to scale your usage up or down and only pay for what you use.**
>
> Scalability is one of the ways to keep your costs down with AWS.

3. **What allows Elastic Block Stores (EBS) to be moved between E2 instances?**

> **They exist independently of virtual servers.**
>
> In this way, they can be thought of as virtual external hard drives that can be moved from device to device.

4. **IT manager Carlos receives approval to upload all his company's backup data to the AWS cloud. There are 35 terabytes of data. How should he perform the upload?**

> **Use the AWS Snowball.**
>
> Carlos uploads the data to the hardware "Snowball" that AWS mails to him, he mails it back, and then AWS uploads the hardware data to S3.

# 3- Database

1. DynamoDB
2. Relational Database Service (**RDS**)
3. Aurora
4. Redshift

## 1- DynamoDB

- Secure, Scalable (Automatically), fast, and **flexible**, **NoSQL database**.
- Virtually unlimited **throughput** and **storage**.
- **Serverless**: _NO NEED_ to **provision**, **manage**, or **update** your own servers.
- **pay for specific workload** or **pay-as-you-go**.


## 2- Relational Database Service (**RDS**)

- Relational Database.
- Only pay for what you use (Pay-as-you-go) or reserve at on-demand pricing (Cheaper).
- AWS takes care of **provisioning**, **monitoring**, and **maintaining** the database.
- Compatible with **Amazon Aurora**, **PostgreSQL**, **MySQL**, **MariaSQL**, **Oracle Database**, **Microsoft SQL Server**.
- Existing database can be migrated using **AWS Database Migration Service**.

## 3- Aurora (One of The Six Available **Relational Database** Engines)

- One of the six available **Relational Databases** supported by Amazon **RDS**.
- Fully managed by **RDS**; No **administration** or **provisioning** necessary so you can only focus on coding.
- Monitor performance through **AWS Monitoring and Alerting Services**.
- MySQL and PostgreSQL **compatible**, but **5 times faster** than Standard **MySQL** and **3 times faster** than **PostgreSQL** and also **Cheaper**.
- Databases up to **64 TP** per instance.
- Hosted on **distributed**, **fault-tolerant**, **self-healing** storage systems with **low latency**.
- Can **migrate** existing MySQL or PostgreSQL **databases** using **AWS Database Migration Service**.

## 4- Redshift
- Fully managed, **petabyte-scale** data **warehouse** servive.
- Super fast, Super cheap.
- You pay for what you use (**Pay-as-you-go**).
- Fully integrated with your data lakes.
- Deploy new data warehouse in **minutes**.
- Secure.
- Data encryption compliant with many common requirements like **HIPAA**.

## Questions

1. **What advantage does Amazon Aurora provide when it comes to creating relational databases?**


> **It is five times faster than MySQL.**
>
> Not only is Aurora faster, but it is also less expensive than using MySQL.

2. **Erie Insurance needs a large data warehouse that is compliant with the Health Insurance Portability and Accountability Act (HIPAA). What AWS service would the company use?**

> **Redshift**
>
> Redshift is a petabyte-scale data warehouse service using encryption that is fully compatible with legal requirements such as HIPAA data.

3. **ABC Corp's new app results in far more being sent back and forth than its database solution can handle. How can DynamoDB help ABC Corp?**

> **by providing a secure, scalable, and flexible noSQL database**
>
> DynamoDB adapts to needs in order to keep speed and stability high, regardless of how large or small the need is.

4. **How is the Amazon Relational Database Service (RDS) especially useful for an experienced database user?**

> **Database engines, such as MySQL and Microsoft SQL Server, can be used.**
>
> This lets an experienced user dive right into creating a database.

# 4- Network and Content Delivery

1. VPC
2. CloudFront
3. Route 53

## 1- VPC

> It helps you to decide what comes in, what goes out, and what lives inside.

![VPC](/Images/3-%20Core%20Services/VPC.png)

- **Logically isolated section** in the cloud to provision resources.

- Flexible and Secure, allowing you to **control** almost every aspect of your **virtual network**.

- VPC automatically provisioned at AWS account signup with (**subnets**, **IP ranges**, **route tables** and **security groups**).

## 2- CloudFront: Content Delivery Network (CDN)

> Faster, Faster and Faster!

- It is a **Global** Content delivery Network (**CDN**).
- Integrates with many AWS services to provide optimal performance and security.
- Makes loading websites/apps for end users faster using **edge locations** to cache files and resources.
- It delivers content to user based on **2 factors**:
1. Location of the user.
2. Location of the Content Delivery Server.

![CloudFront Example](/Images/3-%20Core%20Services/cloudfront-functions-where.png)

### AWS CloudFront Advantages
- Scalable
- No minimum commitment or fixed term contract.
- Only pay for content delivered using the service (**Pay-as-you-go**).

## 3- Route 53: Domain Name System (**DNS**)

<br>

> Amazon Route 53 is a highly available and scalable Domain Name System (DNS) web service. Route 53 connects user requests to internet applications running on AWS or on-premises.

![Amazon Route 53](/Images/3-%20Core%20Services/product-page-diagram_Amazon-Route-53_HIW%402x.4c2af00405a0825f83fca113352b480b19d9210e.png)

- High **scalable** cloud Domain Name System (**DNS**).
- **Reliably and cost-effectively** rpute end users to your internet applications.
- **Connect user requests** to **infrastructure** running on **AWS** like **EC2 instance** or **S3 bucket**.
- Route users to infrastructure outside of AWS as DNS Service.
- Integrates with other AWS services like EC2 or S3.
- **Simple** to setup, **fast**, **secure** and **cost-effective**.
- You're charged only for what you use (**Pay-as-you-go**), without any upfront fees or minimum usage commitments.
- Automatically **scales** to handle **large query volumes**.

### Route 53 Basic Functions

Basic Functions|
:-------:|
 Domain Registration |
 Domain Name System (**DNS**) |
 Health check of web apps accessibility |
 Auto Naming for service discovery |

## Questions



# 5- Management Tools

1. CloudFormation
2. CloudTrail
3. CloudWatch

## 1- CloudFormation
## 2- CloudTrail
## 3- CloudWatch

## Questions

## Conclusion