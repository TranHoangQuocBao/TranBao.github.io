---
title: "3. Create AWS Managed Microsoft AD"
date: 2025-08-11
weight: 3
chapter: false
prev: "2."
---

## Steps to Perform

### 1. Open AWS Management Console
Open the **AWS Management Console** and navigate to **Directory Service**.  

---

### 2. Click "Set up directory"
Click **Set up directory**.  
![AWS Managed AD Step 2](/images/003/anh1.png)

---

### 3. Select AWS Managed Microsoft AD
Select **AWS Managed Microsoft AD** and click **Next**.  
![AWS Managed AD Step 3](/images/003/anh2.png)

---

### 4. Choose Edition
- **Standard Edition**: Supports up to 30,000 objects, suitable for small environments.  
- **Enterprise Edition**: Supports up to 500,000 objects, suitable for large organizations.  
![AWS Managed AD Step 4](/images/003/anh3.png)

---

### 5. Fill in Directory Information
Enter the directory DNS name, NetBIOS name, and the admin password.  
![AWS Managed AD Step 5](/images/003/anh4.png)

---

### 6. Configure VPC
Select the **VPC** and two subnets in different Availability Zones.  
![AWS Managed AD Step 6](/images/003/anh5.png)

---

### 7. Review and Create
Review all settings and click **Create directory**.  
![AWS Managed AD Step 7](/images/003/anh6.png)

---

### 8. Wait for Active Status
Wait until the status changes to **Active** (about 20–45 minutes).  
![AWS Managed AD Step 8](/images/003/anh7.png)

---

## Expected Result
An AWS Managed Microsoft AD is created, available in your VPC, and ready for further configuration.
