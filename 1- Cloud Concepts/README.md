# Prepare for the AWS Certified Cloud Practitioner (CLF-C01) Certification Exam

# 1- Introduction to Cloud Computing

## The Internet

**How data transfered from browser to server and back?**
- Browser--Request-->ISP--Request-->Server---->Webhost--Packet-->Browser

## Cloud = Internet
Made up of copper wires and global network of billions of devices.

## AWS Cloud Computing
- It is the **on-demand** delivery of compute, database storage, application, and other IT resources.
- Utilize a **pay-as-you-go** model [pay only for what you use, when you use them].
- Inastantaneous Access.
- Access resources where and when you want.
- More flexible and affordable than **legacy IT infrastructre**.
- Affordable for organizations and individuals with **smaller budgets**.

## History of Cloud Computing
- 1950s **Mainframe Computing** [Central computers and Dump terminals].
- 1970s **Virtual Machines** [Hypervisors].

## Examples of Cloud Computing services aroud us
- Email
- Youtube
- Office 365
- Google Drive [with different tiers subscription]

## Questions
**Which technology provides oversight for the cloud?**

_hypervising_ Together with connectivity, hypervising is the enabling technology.

**What marks the origin of cloud computing, and when did it occur?**

_the development of mainframe computing in the 1950s_

Electronic computing begins here, and the idea of having multiple, dumb terminals started the idea of the cloud.

# 2- Cloud Computing Concepts

## Why to choose Cloud Computing for work?
 - No need for physical servers on cabling.
 - No need for server room setup or maintenance.
 - No hardware replacement or procurements.
 - Pay only when and what you consume [**Pay-as-you-go**].
 - **Scalability** Scale up or down instantaneously and only pay for waht you use.
 - Benefit from **Economy of scale**.

## Main 6 Advantages of Cloud Computing according to [AWS] _IMPORTANT_

1. Trade capital expense for variable expense.
2. Benefit from massive economies of scale.
3. Stop guessing capacity.
4. Increase speed and agility.
5. Stop spending money runnig and maintaining data centers.
6. Go global in minutes.

## Three-3 Main Cloud Computing Models
- SaaS [**Software**].
- PaaS [**Platform**].
- IaaS [**Infrastructure**].

**Infrastructure as a Service (IaaS)**
- Basic building blocks.
- Most flexibility and management control.
- Closest to having traditional **on-premises** data center.

**Platform as a Service (PaaS)**
- Deploy and manage applications without worry. [Ex: Microsoft Azure web hosting - Google App Engine - Heroku].
- Execute programming languages to host applications.
- Less flexibility than IaaS, as **packages are _Preconstructed_**.

**Software as a Service (SaaS)**
- **"Completed Products"** managed by the service provider [Ex: Gmail - Outlook].
- Easy to use as **End-User**.
- Less flexibility.

## Complexity level
1. High [**IaaS**].
2. Mid [**PaaS**].
3. Low [**SaaS**].

## Cloud Deployment Models
- **Public** Cloud Delployment.
- **On-Premises / Private** Deployment.
- **Hybrid** Deployment.

1. **Cloud Deployment**
- **100%** of IT infrastructure on the cloud.
- All applications migrated to or created in the cloud.
- Rmoves **roadblock** of costly and **time-consuming** procurement processes.

2. **On-Premises/Private Cloud Deployment**
- Use **Virtualization** to deploy resources in their **on-premises** data centers.
- Often looks like **Traditional** IT infrastructure.
- Does not provide a lot of benefits of cloud computing.
- Resources **Cannot** be accessed using the **internet** [this provide a very quick data access].
- Procide dedicated resources [no resource sharing with other companies].
- High Security.

3. **Hybrid Deployment**
- Connect **on-premises** technology with **cloud-based** resources.
- Great for established companies that are in the process of **migrating** over the cloud.
- Data **Partially** on the cloud, and **Partially** in the on-premises data centers.
- Use the **Cloud** as **Backup** and **disaster recovery solution**.

## We choose the best deployment model based on this features

1. **Cloud Deployment**
- Utilize **Flexibility** and **Affordability** of cloud computing.

2. **On-Premises/Private Cloud Deployment**
- High Security on-premises.
- High **Data Retrieval** speed.
- Virtualization of legacy resources.

3. **Hybrid Deployment**
- **Partially** on the cloud, and **Partially** in the on-premises data centers.

## Well-Architected Framework

[**Build the most secure, durable, efficient, and high-performing IT infrastructure possible**].

**_BEST PRACTICES_**

1. **Avoid Unnecessary Costs**
- Use only what you need.
- Reserve resources in advance.
- Continue to monitor for optimization.

2. **Reliability**
- Test disaster recovery settings.
- Incorporate redundancy.
- Have duplicate copies of resources.

3. **Efficiency**
- The **efficient use** of computing **resources** to **adjust** to system **requirements**.

4. **Security** [Information - System - Assests]
- Best practice should be **automated**.
- **Data** should be always **protected**.
- Enable **Traceability**.
- **Manage access**.

5. **Operational Excellence**
- Document everything.
- Refine operational procedures.
- Anticipate failure.
- Update processes.
- Learn from failures.

 6. **Sustainability**
 - Maximum performance from available resources.
 - Minimize required total resources.
 - Minimize **environmental** impact.
 - Have **lower footprints** and **more energy efficient** than typical **on-premises environments**


# 3- Introduction to AWS

## Amazon Web Services (AWS)

- Provide **IT infrastructure** (IaaS) service to organizations as web services.
- Resources are accessed using internet.
- Utilize the **Pay-as-you-go** model to help organizations save money, time and human resources.

## 24 AWS Services by Groups

| Column 1 (8) | Column 2 (8) | Column 3 (8) |
| :-------------: | :-------------: | :-------------: |
| Analytics | Database  | Migration and Transfer  |
| Application Integration  | Developer Tools | Mobile  |
| AR and VR  | End-User Computing  | Networking and Content Delivery  |
| AWS Cost Management  | Game Tech  | Quantum Technologies  |
| Blockchain  | Internet of Things (IOT)  | Robotics  |
| Business Applications  | Machine learning  | Satellite  |
| Compute  | Management and Governance  | Security, Identity and Compliance  |
| Customer Engagement  | Media Services | Storage  |

## Big Companies using AWS
1. Airbnb
2. General Electric
3. Dow Jones
4. Kellogg's
5. Atlassian
6. Netflix
7. Citrix
8. Squate Enix
9. Spotify
10. USDA
11. UK Ministry of Justice

## Questions
**Q1. Why did Amazon originally venture into cloud computing?**

*to serve third-party vendors*

> AWS made life easier for small, external vendors on Amazon.

**Why do many large organizations use cloud computing?**

> for scalability, rapid deployment, and efficiency

# 4- Diving into AWS

## popular services offered in aws

1. **Compute Service**

- Provide **virtual server hosting**, **Container Management**, and **Serverless Computing**.

- Instead of hosting servers themselves, organizations can **"RENT"** server compute space and capacities for cheap from AWS.

- No longer have to **prochase** physical server or **maintain** data centers **on-premises**.

2. **Storage Services**

- Provide storage for both **in-use** and **archival** files.

**Examples**
> * (Elstic File System - **EFS**) to create shared folders in the cloud.
> * (simple storage - **S3**) to upload files like images, text, etc.
> * (**S3 Glacier**) to archive file and store large amount of data for cheap.
> * (**Storage Gateway**) to take daily **backups** of your company's on-premises data.

- Different **Cost** associated with **Frequency** and **Durability** of data access.

- Storage type for almost every level of need with ver granilar costs mmet budget requirements.

3. **Database Services**

- **Fully Managed** _Relational_ and _NoSQL_ databases.

**Examples**

> * (**RDS**) is the most **Cost-Efficient** database.
> * (**DynamoDB**)is a **Relational** and **highly scalable** _NoSQL_ database.

- Also offers **Fully Managed** Data **Warehouse** service.

**Examples**
> * (**Redshift**)

- Highly **scalable** and **cost-efficient**: crunch data at fraction of cost of on-ste database servers.

**Examples**
> * (**ElastiCache**) it chaches necessary data on the cloud.

# Practical Part!

## Create an AWS account

1. go to aws
2. create a personal account.
3. add your visa card number and confirm the security check.
4. confirm with message sent to your phone for verfication.
5. personalize your experience.
6. check your account and login.

## Exploring the AWS dashboard

> No limits - No Instructions :)

## Use case: AWS Free Tier

**Build A Personal Bolg Using AWS**

Service A | Service B |
:---------:|:----------:|
 Route 53      | EC2 AMI |
 Domain registration     | WordPress |
 Ex: **myblog.com**     | template on a virtual server |

## Questions

1. How can you find general documentation and help on the AWS dashboard?

> **from the Support drop-down menu**,
> You can find detailed documentation and create help tickets.

2. How should you use AWS Free Tier?

> **as a way to explore**, The service provides an introduction to AWS, and lets you try various capabilities.

3. How can you make the URL for your weblog simpler than the long AWS string?

> _by using the paid AWS domain registrar_, **This service is called Route 53.**

4. Your team has some extensive calculations to conduct for an engineering design. Which type of service would be most helpful?

> **Compute**, Compute services are core to many scientific and engineering operations.

5. What information is necessary for AWS account creation?

> **telephone number** and **credit card credentials**, The telephone number can be mobile or other.

## Conclusion

Topics to Review |
:---------:|
 What is AWS? |
 What are the six (6) advantages of Cloud Computing?|
 What are the three (3) Cloud Computing Models? [ **SIP** ]|
 What are the three (3) Cloud Computing Deployments? [ **PHO** ]|
 What are the Five (5) pillars of a Well-Architected Framework?|

* For the 3 **Cloud Models** and 3 **Cloud Deployments** remember this word [ **SIP PHO** ]
> Silly Memorizing Method
>
> SIP PHO
>
> SaaS, IaaS, Pass
>
> Public, Hybrid, On-Premises / Private

* For the **SIX 6** "_Pillars_" of a **Well-Architected Framework** remember this word [ **CROPSS** ]

1. [ **C** ] --> **C**ost Optimization.
2. [ **R** ] --> **R**eliability.
3. [ **O** ] --> **O**perational Excellence.
4. [ **P** ] --> **P**erformance Efficiency.
5. [ **S** ] --> **S**ecurity.
6. [ **S** ] --> **S**ustainability.