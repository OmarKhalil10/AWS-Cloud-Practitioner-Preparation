# Prepare for the AWS Certified Cloud Practitioner (CLF-C01) Certification Exam


# 1. Prepare Your App

1. Billing concepts
2. Types of charges
3. Consolidated billing
4. Cost calculators
5. AWS Free Tier
6. Study Break: Billing and Pricing domain

## Billing and Cost Management Dashboard

- **Estimated** and **plan** your AWS costs.
- **Consolidated billing**: simple accounting for multiole AWS accounts within your organization.
- **Alerts** when you are nearing usage **thresholds**, which could mean additional costs.
- Use **Cost Explorer** to view costs as **graph**.

> **Uderstanding AWS Billig**
>
> Helping you stay on top of your costs and services being consuned by your otganization.


## Pay-As-You-Go Model of Cloud Computing

- No huge upfront costs.
- Billig only for the resources consumed.
- Easily Scale resources UP or DOWN to suit business needs.

## Fundamental Drivers of Cost

- Compute like (EC2).
- Storage like (S3).
- Outbound Data Transfer.

### 1- Compute

- Pay **hourly** from the time **launched** to **termination**.

- EC2 (**Virtual Server**): Pay for the length of time the server is **UP and RUNNING**.

### 2- Storage

- Pay per **GB** of storage used.
- S3 (**Storage Service**): Upload photos into an app and pay for the storage used.

### 3- Outbound Data Transfer (No Charge for Data Transfer Between AWS Resources **Within The Same Region**)

- Pay to transfer the data (**OUT of AWS**).
- Usually no charge for data **INTO** AWS or data transfer between other AWS services (**in other words, between S3 and EC2 within the same region**).

## Pricing Model Example: Storage Types (S3)


Storage Type | Price (in US East Region) |
---------|----------|
 Standard Storage (**Most Expensive**) | $0.023 |
 Glacier Storage | $0.004 per GB |
 Glacier Deep Archive Storage | $0.00099 per GB |

## Pricing Model Example: Data Input/Output (**Aurora**)


Input/Output | Price (in US East Region) |
---------|----------|
 Data In/Data Out | $0.20 per 1 million requests |

## Consolidated Billing (Is FREE)

> Create a payer AWS account to view and pay combined billing charges for all linked accounts in an organization

- Independent acconut, **but can't use any other services.**.
- **Cannot deploy service** into the linked accounts.
- All resources usage becomes **Consolidated** as usage from one large **entity-Organization** may be eligable for **volume discounts**.

## Cost Calculators

## 1- (**TCO** Calculator: **T**otal **C**ost of **O**wnership)

### Usage of Total Cost of Ownership (TOC) Claculator

- Get **reports** on **estimated savings** form moving **on-premises** IT infrastructure onto **AWS cloud**.
- Total Cost of Ownership (**TCO**) includes **upfront** hardware/**infrastructure** costs and **maintenance** costs.
- **TCO** can be reduced by moving to the cloud because **no upfront infrastructure purchases**.
- Rather, you will e Utilizing a **Pay-As-You-Go** model which will help you to (**pay only when your business uses the resources**).


## 2- AWS Pricing Calculator ([link](https://calculator.aws))

### How it works

![Pricing Calculator](/Images/4-%20Billing%20and%20Pricing/pricing%20calculator.png)

### Benefits and features


Benefits & Features | Description |
---------|----------|
 **Transparent pricing** | See the math behind the price for your service configurations. View prices per service or per group of services to analyze your architecture costs. |
 **Share your estimates** | Save each estimate's unique link to share or revisit directly through your browser. Estimates are saved to AWS public servers. |
 **Hierarchical estimates** | See and analyze service costs grouped by different parts of your architecture. |
 **Estimate exports** | Export your estimate to a .csv file to quickly share and analyze your proposed architecture spend. |

## Cost Explorer

> It is a part of Cost Management Console Dashboard

### Usage

- View and analyze your AWS cloud costs and usage
- Forecast how much you're likely to spend in upcoming month
- Get recommendations for what reserved instance to purchase to minimize cost

## AWS Free Tier
> It allows a free usage for AWS Cloud Service for free to test the service before you can use it

## Study Break: Billing and Pricing

## 1- AWS Billing and Cost Management Console

- Plan your AWS spending
- Simplify accounting through **Consolidated Billing**
- Recieve alerts for service usage **Thresholds**
- **Cost Explorer:** Generate billing **Reports** of AWS cost and usage
- **Other Resources:**
1. AWS Pricing Claculator
2. AWS Total Cost of Ownership Claculator (**TCO**)

## 2- Types of AWS Charges
1. Fundamental Charger:
- Compute
- Storage
- **Outbound** Data Transfer

> Note: Inbound Data Transfer is free [Between AWS Resources]

2. Different service charge differently

3. **The more** you do something (Compute, Storage, Transfer Data) **the cheaper** per unit the action becomes

## 3- Consolidated Billing (To Save More Money)

- It is a way to **Save Money** if you have alot of resources running in **Many AWS Accounts** in your organization
- Create a billing-only payer account that views and pays combined billing charges for **All** linked AWS accounts

- All resources used within the **linked AWS accounts** considered part of **One Large** organization; organization as a whole may be eligible for **Volume Discounts**

# 2- Support Plans

1. Basic
2. Developer
3. Business
4. Enterprise
5. Which one's best for you?
6. Study break: Reviewing AWS support plans

## 1- Basic Support Plan (FREE)

> It is used for new users who want to test out their services before use it, and it is available for 12-months

- No tech support; customers service limited to account and billing questions
- Provide access for AWS community forums
- Only **7-Core Trusted Advisor Checks For Free**
- AWS Personal Health Dashboard

## 2- Developer Support Plan

> It starts with **$29** per month and increases based on usage

- [AWS support plan](https://aws.amazon.com/premiumsupport/plans/)
- **One Primary Contact** to submit tech support requests [only one person can contact with them elected by the prganization]
- Unlimited number of cases
- Technicians will respond during **business hours via email**
- Service-level-agreement (**SLA**) for response: **12-hours** for **impaired system** and **24-hours** for **general guidance**

### Who used the **Developer** support plan?

> It is not even [**near-immediate**] plan and **not for production** as failure can have a huge impact

- Trying out features, deploying prototypes
- Assessing the viability of AWS within their IT infrastructure--need tech support
- Not fully committed to AWS yet, so don't want to pay full support price

## 3- Business Support Plan

> Ideal plan for those who use AWS in **PRODUCTION**

- [AWS support plan](https://aws.amazon.com/premiumsupport/plans/)
- It begins with **$100/month** OR **3-10%** of monthly AWS usage bill (whichever is higher)
- **Unlimited** number of **contacts** can open **unlimited** number of support cases
- Access AWS support API for support case automation
- Retrieve detailed information about support operations and data types in **JSON Format**
- **Full access** to AWS [Trusted Advisor checks](https://aws.amazon.com/premiumsupport/technology/trusted-advisor/)
- Can retrieve **Trusted Advisor** check data through **AWS Support API** like (Checks - Check Results - Check status)
- [**Extra Fees**] to access **infrastructure Event Management**
- Third-party application integration support
- SLA: **24/7 support** via (Phone - Email - Chat)
- **One-Hour** response time for **urgent** support cases when **production system is down**

## 4- Enterprise On-Ramp Support Plan (**NEW**)

- Cost **$5,500 per month** or **10% of monthly AWS usage** bill (whichever is higher)
- Conssultative application architecture guidance on how AWS resources can meet unique use case
- [**Once-A-Year**] Short-term engagement with AWS support for **architectural** and **scaling** guidance for **Infrastructure Event Management**

- Access to **POOL** of Technical Account Managers (**TAMs**) and **Concierge** Support Team
- Access to management business reviews
- SLA: **24/7** support via (Phone - Email - Chat)
- **30 minutes** response time for **business-critical system down**

## 5- Enterprise

- Greater of **$15,000 per month** or **3-10% of monthly AWS usage** costs
- **24/7** tech support with **SLA** of **15-minutes** for emergencies
- Technical Account Manager (**TAM**) and **Support Concierge** including [**proactive programs** - **well-architected reviews** - **trainings**]
- For **huge organization** with **huge budgets** and **mission-critical** resources on AWS Cloud
## Which one's best for you?

1. Basic
2. Developer
3. Business
4. Enterprise On-Ramp
5. Enterprise

Basic | Developer | Business | Enterprise On-Ramp | Enterprise
---------|----------|---------|---------|----------
Basic Support offers support for account and billing questions and service quota increases | Recommended if you are experimenting or testing in AWS | Minimum recommended tier if you have production workloads in AWS | Recommended if you have production and/or business critical workloads in AWS | Recommended if you have business and/or mission critical workloads in AWS

## Conclusion

1. Exam tips and resources
2. Netx steps

## 1- Exam tips and resources

**1. Compare and Contrast Pricing Models**
- Different ways AWS charges for resource usage
- Main ways: (Compute - Storage - Data Transfer Out)
- The **more you do an action** (store more data, etc) the **cheaper per unit of action**

**2. Account Structures for Billing and Pricing**
- **Consolidated billing**: Link all AWS accounts in an organization to simplify accounting and potentially recieve volume discounts for resource use
- Compare and contrast support plans and identify the most suitable support plan for a situation


Basic | Developer | Business | Enterprise On-Ramp | Enterprise
---------|----------|---------|----------|---------
 **Free** | Starting at **$29** per month | Starting at **$100** per month | Starting at **$5,500** per month | Starting at **$15,000** per month

> Support plans fees **doesn't** include AWS resource usage fees

## Resources for Billing Support

- AWS website: **White papers**, **Knowledge bases**, etc
- Contact AWS Billing Support
- Utilize Calculators: A**WS Cost Explorer**, AWS Total Cost of Ownership Calculator (**TCO**), AWS **Simple Monthly Calculator**

Links:
- [AWS Simple Monthly Calculator](https://calculator.s3.amazonaws.com/index.html)
- [AWS TCO Tools](https://calculator.aws/)

## 2- Netx steps

