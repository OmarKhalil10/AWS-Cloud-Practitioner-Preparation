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
|

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

1. Identity and Access Management (**IAM**).

List of Imprortant Things about IAM|
:------:|
Manage access to **services** and **resources** on the AWS Cloud|
Manage **Users** and **Groups**|
Can provide access to **users** or other **AWS service**|
**Permissions** are **global**: any access setting will be true across all regions|
Follow principle of Least Privilege|
|

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
