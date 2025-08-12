---
title: "4. Configure Trust Relationships"
date: 2025-08-11
weight: 4
chapter: false
prev: "4."
---

## Step-by-Step

### 1. Access AWS Directory Service
Sign in to the AWS Management Console, navigate to **Directory Service**, and select your AWS Managed Microsoft AD.  
![Configure Trust Relationships](/images/004/01.png)

---

### 2. Open Trust Relationships
In the directory details page, choose **Networking & security** → **Trust relationships**.  
![Configure Trust Relationships](/images/004/02.png)

---

### 3. Add a New Trust
Click **Add trust**.  
![Configure Trust Relationships](/images/004/03.png)

---

### 4. Select Trust Direction
Choose the trust direction:  
- **One-way incoming** – On-prem AD trusts AWS Managed AD.  
- **One-way outgoing** – AWS Managed AD trusts on-prem AD.  
- **Two-way** – Both directories trust each other.  

Select **Forest trust** for cross-domain authentication.  
![Configure Trust Relationships](/images/004/04.png)

---

### 5. Configure Trust Settings
Enter the **FQDN** of the trusted domain, set the trust password (must match on both sides), and choose:  
- **Selective authentication** for tighter control  
- **Forest-wide authentication** for broader access  
![Configure Trust Relationships](/images/004/04.png)

---

### 6. Confirm and Validate Trust
Click **Create** and wait for the trust to be established.  
From your on-prem AD, create the corresponding trust using **Active Directory Domains and Trusts**.  
Validate the trust from both sides to confirm connectivity.  
![Configure Trust Relationships](/images/004/05.png)

---

## Outcome
AWS Managed Microsoft AD and your on-premises AD are now connected via trust relationships, enabling authenticated access to resources across environments.
