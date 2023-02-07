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

## Questions

# 3- Database

1. DynamoDB
2. Relational Database Service (**RDS**)
3. Aurora
4. Redshift

## 1- DynamoDB
## 2- Relational Database Service (**RDS**)
## 3- Aurora
## 4- Redshift

## Questions

# 4- Network and Content Delivery

1. VPC
2. CloudFront
3. Route 53

## 1- VPC
## 2- CloudFront
## 3- Route 53

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