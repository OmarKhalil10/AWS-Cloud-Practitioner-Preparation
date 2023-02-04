# Prepare for the AWS Certified Cloud Practitioner (CLF-C01) Certification Exam

# 2- Security on the cloud

## Reviewing AWS Security Services

- AWS Identity and Access Management (**IAM**).
- AWS Web Application Firewall (**WAF**).
- AWS **Shield**.
- AWS Trusted Advisor.
- Amazon Inspector.
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

## Security in a Well-Architected IT Infrastructure (Secure from **internal** & **External** threats)

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

## 4- Data Protection

- Security **mechanisms** should be **adjusted** depending on **sensitivity** of **data**.
- Keep people **Away** from **Data**.

## 5- Incident Response
- **Intervene**, **Investigate**, and **deal** with all security events.
- Once issue is **resolved**, **update** incident **management** process.
- Continue to **learn** from past **mistakes** and **security events**.