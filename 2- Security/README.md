# Prepare for the AWS Certified Cloud Practitioner (CLF-C01) Certification Exam

# 1- Security on the cloud

## AWS Security Domain Includes

- Security in the Cloud.
- Shared Responsibility Model
- Security **Pillar** of the Well-Architected Framework.
- Principle of least privilege.
- AWS Cloud Compliance.
[AWS Compliance Programs](https://aws.amazon.com/compliance/programs/)

## Reviewing AWS Security Services

- AWS Identity and Access Management (**IAM**).
- AWS Web Application Firewall (**WAF**).
- AWS **Shield**.
- Amazon Inspector.
- AWS Trusted Advisor.
- Amazon GuardDuty.

## IT Infrastructure: In The Past

- Server rooms secured with key cards.
- Off-site data centers.
- Lots of security devices and people.
- Difficult to access.

## IT Infrastructure: Present-Day AWS Cloud

- **Global** network of data centers built with security in mind.
- **Safeguards** to protect customer privacy.
- **Dozens** of compliance programs to help meet industry compliance requirements for data security.

## In AWS Cloud, IT Infrastructure Looks Like...

- **High-security** standard **without** need for your own **data centers**.
- Scale your business quickly.

## Shared Responsibility Model (Your responsibility vs. AWS's responsibility)

> Security of Cloud Computing infrastructure and data is a **Shared responsibility** between the **Customer** and **AWS**.


You/Customer | AWS |
:---------:|:----------:|
Security **in** the Cloud      | Security **of** the Cloud   |

![Shared_Responsibility_Model](/Images/2-%20Security/Shared_Responsibility_Model.jpg)

## Shared Responsibility by Service Type

![Shared-Responsibility-by-Service-Type](/Images/2-%20Security/Shared-Responsibility-by-Service-Type.png)

## AWS: Security of the Cloud

<br>

**AWS** is **responsible** for **protecting** the **infrastructure**, such as

- **Physical security** of _data centers_ hosting the AWS Cloud.
- Security of **hardware**, **software**, **networking**, and so on, that runs the cloud computing service.

> AWS is responsible for security of **the components** that make up the AWS Cloud.

## You: Security in the Cloud

<br>

You are responsible for **Varying levels of security functions**, depending on the AWS Cloud service used, such as

- Protecting customer **data and data encryption**.
- Identity and Access Management (**IAM**).
- **Paching** Operating Systems (**OS**) **of** Virtual Machines (**VMs**).
- **Configuring Firewalls**.

> The Customer is responsible for **security of things** _inside_ the AWS Cloud like **encryption and paching servers**.

## Security **pillar** in a Well-Architected IT Infrastructure / Framework (Secure from **internal** & **External** threats)

## Secutiry have **5** main parts

1. Identity and Access Management (**IAM**).
2. Detective Controls
3. Infrastructure Protection.
4. Data Protection.
5. Incident Response.

## 1- Identity and Access Management (**IAM**)

- Actively manage all-user access.
- Use strong identity foundation.
- Principle of **least privilege**.

## 2- Detective Controls

- Enable Traceability: "**Who did what, when?**".
- Actively monitor alerts.
- Audit actions and changes to environment in real time.

## 3- Infrastructure Protection

- Apply security on **all layers** of infrastructure.
- Not just the **outer layer** like the **Physical Data Centers**.
- **Virtual Servers**: secure **multiple layers** like **subnet**, **load balancer**, and **OS**.
- Security best practices should be **automated** to save **time** and **money** when **scaling**.

## Data sould be secured at both states [ At Rest - In Transit ]


At Rest | In Transit |
:---------:|:----------:|
Image saved in **S3 bucket**  | **Email** being **sent** from one **server** to **another** |
|

## 4- Data Protection

- Security **mechanisms** should be **adjusted** depending on **sensitivity** of **data**.
- Keep people **Away** from **Data**.

## 5- Incident Response
- **Intervene**, **Investigate**, and **deal** with all security events.
- Once issue is **resolved**, **update** incident **management** process.
- Continue to **learn** from past **mistakes** and **security events**.

## Principle of Least Privilege (Who can access What?)

<br>

> only give access to resources that a person needs to do his job, and no more.

> Every **role** has a **set of access permissions** necessary to effectively complete it's **job**, and the individual in the role should have **no more or no less** than the **optimal** level of **access**.

- Use Identity Access Management (**IAM**) to provide access.
- you can provide access to resources to both **users and other AWS services**.
- Start with the **Least** (**Minimum**) set of **permissions**, and grant **additional** only as **necessary**.
- **Determine** what user/service **needs** to be able to do and craft **policies** to perform only those **specific** tasks.

## Recommended Security Practices

1. Shared Responsibility Model.

> Security of data and resources in the cloud is shared responsibility between **the cloud service provider** and **the customer**.

You/Customer | AWS |
:---------:|:----------:|
Security **in** the Cloud      | Security **of** the Cloud   |

2. Security **Pillar** of the Well-Architected Framework.

3. Principle of least privilege.

## Question

1. **How can you best protect your AWS Cloud infrastructure from both _internal_ and _external_ threats?**

> you can do this by ( **Follow the 5 areas of security pillar of Well-Architected Framework** ).

2. **What resources should a certain user have access to?**

> By apply the Principle of Least Privilege.

- Only provide access to resources an **entity** requires to do it's job.

- permission should be **no more or no less** than the **optimal** level of **access**.

- Use Identity and Access Management (**IAM**) in the AWS Cloud.

- **Coincides** with the **Shared Responsibility Model**.

3. **Which statement best exemplifies the principle of least privilege?**

> Grant access to the optimal resources required for a job and no more.

4. **How does cloud security differ from security at private data centers?**

> Cloud security can be at least as comprehensive as security at private data centers.
>
> Cloud data centers provide all the options that you expect, but you do not have to manage them.

5. **In the shared responsibility model with AWS Cloud, who should manage identity and access?**

> **the customer**
>
> Only the customer will know which people should have access.

6. **In a well-architected framework, how should you implement infrastructure protection?**

> **on all layers**
>
> Best practices require automated security on all systems.

7. **You are engaged in educational record management and want to port your operations to AWS. How should you start examining security issues?**

> Peruse the site aws.amazon.com/compliance/programs/
>
> From there, you may examine the resources at aws.amazon.com/compliance/ferpa/

# 2- Security Services

## 1- Identity and Access Management (**IAM**).

List of Imprortant Things about IAM|
:------:|
Manage access to **services** and **resources** on the AWS Cloud|
Manage **Users** and **Groups**|
Can provide access to **users** or other **AWS service**|
**Permissions** are **global**: any access setting will be true across all regions|
Follow principle of Least Privilege|


## With IAM You have **3** **methods** of **Management**

1. Manage **Users**.
2. Manage **Roles**.
3. Manage **Federated Users**.

## Method 1: Manage **Users**

- Create users in IAM and assign them security credentials.
- Users can have very percise permissin sets.
- User can access AWS through AWS Management Console.
- You can provide programmatic access to data/resources.
- Programmatic access: **applications** directly **accessing** **resources** **instead** of **humans** doing the same activity.

## Method 2: Manage **Roles**

- Create **roles** to manage **permissions** and what those roles can do.
- An **entity** **assumes** a role to **obtain temporary security** credentials to make **API** **calls** to your **resources**.
- Used to p**rovide access** to a user from **another AWS account** to your AWS account.

## Manage **Federated Users** [ FBI OPEN UP! ]

- Enable identity federation: allow existing identities in your enterprise to **Access AWS without having to create IAM user** for each **identityIdeal**
for lists.
- Can **use** any **identity management solution** using **SAML 2.0** or one of **AWS's federation samples**.

## Benefits of Identity and Access Management (**IAM**)

1. Enhanced security.
2. Granular control.
3. Ability to provide temporary credentials [ **In Manage Roles** ]
4. Flexible **security credential management**.
5. Federated access.
6. **Seamless integration** across various AWS service.

## 2- Web Application Firewall (WAF)

- Protect web apps runnig on the AWS Cloud from common web exploits.
- Firewall service for web applications.
- Protect web apps against exploits that could compromise **security** or **availability**.
- Protect apps from exploits that could force your app to **consume excessive resources** (More Cost).

### Advantages of (WAF)

1. Improve web **traffic visibility**.
2. Provide **cost-effective** web app protection.
3. **Increased security** and protection against **web attacks**.
4. Easy to **deploy** and **maintain**.

## 3- AWS Shield (DDoS Protection).

> **What is DDoS Attack?**
>
> - An attempt to make a machine or network resource **unavailable**.
> - Most often my making **excessive repeated requests** to the website **using thousands of unique IP addresses**.

### Advantages of AWS Shield

- Provides **detection** and **automatic mitigations**.
- **Minimizes effects** of DDoS attack to your apps.
- Helps **Minimize** application **Down time and Latency** when an attack happens.

### Tires of AWS Shield

Standard Tier | Advanced Tier |
:---------:|:----------:|
 Automatically Enabled     |Continuous, **24/7** access to AWS DDoS response team |
 **Free**      | Near **real-time** visibility into **events** |
 Protects web apps against a **majority** of common DDoS attacks      | Integrates with **AWS WAF** |
 Get comprehensive availability protection against **all known infrastructure attacks** when used with **CloudFront** and **Route 53**   | Provides **high-level** protections, **network and transport layer** protections, and **automated** application traffic **monitoring** |

 ### Advantages of AWS Shield: **Advanced**

 - Financial protection against DDoS-related spikes in charges for **EC2**, **Elastic Load Balancers**, **CloudFront**, and **Route 53**.

 - Available **globally** on all **CloudFront** and **Route 53** Edge locations.

 - Your web application can be hosted **anywhere** in the world and still be **protected** by **AWS Shield**.


## 4- Amazon Inspector

> Inspects your applications to find security issues and bring them to your attention.

- **Automated** security assessment service for applications.
- **Automatically** assess for **exposure**, **vulnerability**, and **derivations** from best practices.
- **Generate** detailed **Reports** to help check for **vulnerabilities**.
- Security teams can **get reports** validating that **tests** were performed.

### Advantages of Amazon Inspector

- **Reduce risk** of introducing security **issues** during **deployment** and **development**.
- You can **define standards** and best practices.
- or you can use the **AWS constantly updated standard**.

## 5- AWS Trusted Advisor

> Makes sure AWS Cloud resources are aligned with **best practices** and **provide** customized **recommendations**.
>
> Secure your cloud **IT Infrastructure**.

- **Guides** provisioning of resources to follow **AWS best practices**.

- **Scans** your infrastructure and advises you on **how it is or it is not following AWS best practices**.

- Based of **FIVE** categories:

**5** categories |
:--------:
 Cost Optimization |
 Performance |
 Security |
 Fault Tolerance |
 Service Limit |

- Provides action **recommendations** to **meet best practices**.

### Seven (**7**) Core Trusted Advisor **Checks**

1. **S3** bucket permissions.
2. **Security groups** _ specific ports unrestricted.
3. **IAM** use.
4. **MFA** on **root** account.
5. **EBS** public **Snapshots**.
6. **RDS** public **Snapshots**.
7. Service **Limits**.

### **Additionally**

- **More** types of **checks** on **top** of **Core Checks**.
- **Notifications** through weekly updates.
- Set up **automated actions** in responce to akerts **using** **CloudWatch**.
- **Programmatic** access to scan results via **AWS Support API**.

## 6- Amazon GuardDuty

> Continuous, **24/7** _threat detection_ service.
>
> Amazon **GuardDuty** continuously monitors your **AWS Cloud Infrastructure**, Intelligently **detects threats** using **Machine Learning**, and **Helps** you to **Take Action** immediately if a threat is found.

- Provides **24/7** _threat detection_ service for the AWS Cloud.
- **Monitors** for **malicious** activity and **unauthorized** behavior.
- **Analyzes** events to send actionable **alerts** via **CloudWatch**.

### Note
> Amazon **GuardDuty** used **Machine Learning [ Anomaly Detection ]**, and **Integrated Threat Intelligence** to identify potential threats.
>
> **Easy** to deploy.

## Questions

1. **How does AWS GuardDuty deal with threats?**

> It constantly monitors activity and deploys machine learning techniques for analysis.
AWS GuardDuty is **continuously active**.

2. **What does AWS Inspector examine?**

> **application security**
>
> If you develop your own application, AWS Inspector can help you find any security flaws.

3. **What action does AWS Trusted Advisor take upon implementation?**

> It looks at your setup and suggests changes to meet best practices.
>
> Security is just one issue that Trusted Advisor examines.

4. **Why would you employ federated users?**

> **to integrate with external operations and across AWS systems**
>
> For example, you might integrate Microsoft Active Directory with AWS IAM.

5. **What is the purpose of a WAF?**

> **to protect applications from malicious activity**
>
> A WAF, or web application firewall, protects your applications from web exploits.

6. **Why would you need the advanced instead of the standard AWS Shield?**

> to get real-time tools for balancing loads
>
> The advanced AWS Shield provides more dynamic responses and financial protection.

## Review the Security and Compliance Domain

1. Shared responsibility model.
2. Security pillar of the Well-Architected Framework.
3. Principle of least privilege.
4. Security Services.

## 1- Shared responsibility model

> Security of Cloud Computing infrastructure and data is a **Shared responsibility** between the **Customer** and **AWS**.


You/Customer | AWS |
:---------:|:----------:|
Security **in** the Cloud | Security **of** the Cloud |


## 2- Security pillar of the Well-Architected Framework

### It has **5** main parts

1. Identity and Access Management (**IAM**).
2. Detective Controls
3. Infrastructure Protection.
4. Data Protection.
5. Incident Response.

## 3- Principle of least privilege

> Provide the **Least amount of access** necessary to any entity; **No More, No Less**.

## 4- Security Services

### AWS Security Services

1. IAM
2. WAF
3. Shild
4. Inspector
5. Trusted Advisor
6. GuardDuty
