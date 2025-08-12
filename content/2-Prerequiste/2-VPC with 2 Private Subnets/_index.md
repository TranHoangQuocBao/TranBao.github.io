---
title: "2 - VPC with 2 Private Subnets"
date: 2025-08-11
weight: 2
chapter: false
prev: "2.2"
---

## Step-by-Step

### 1. Open the VPC Console
Sign in to AWS Management Console and navigate to **VPC** service.  
![VPC with 2 Private Subnets](/images/002/1.png)

### 2. Create a New VPC
Click **Create VPC**.  
- Name: `ProjectVPC` (example).  
- IPv4 CIDR block: e.g., `10.0.0.0/16`.  
- Tenancy: **Default**.  
- Click **Create VPC**.  
![VPC with 2 Private Subnets](/images/002/2.png)

### 3. Create Private Subnets
Go to **Subnets** → **Create subnet**.  
- Select your VPC.  
- Create **Private Subnet 1** in Availability Zone 1 with CIDR (e.g., `10.0.1.0/24`).  
- Create **Private Subnet 2** in Availability Zone 2 with CIDR (e.g., `10.0.2.0/24`).  
![VPC with 2 Private Subnets](/images/002/3.png)

### 4. Configure Route Tables
Ensure both subnets are associated with a private route table (no direct internet gateway).  
![VPC with 2 Private Subnets](/images/002/done.png)

### 5. Verify
Confirm that the VPC has at least **two private subnets in different Availability Zones**.  
![VPC with 2 Private Subnets](/images/002/5.png)

## Result
You now have a VPC ready with two private subnets in separate AZs.
