# Prepare for the AWS Certified Cloud Practitioner (CLF-C01) Certification Exam


# 1. Prepare Your App

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


## AWS Free Tier


