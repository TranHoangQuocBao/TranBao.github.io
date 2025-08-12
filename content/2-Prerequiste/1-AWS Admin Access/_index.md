---
title: "1 - AWS Admin Access"
date: 2025-08-11
weight: 2
chapter: false
prev: "1."
---

## Step-by-Step

### 1. Sign in to AWS Management Console
Go to [https://aws.amazon.com/](https://aws.amazon.com/) and log in using your AWS root account.  
![AWS Admin Access](/images/001/1.png)

### 2. Open IAM Console
In the AWS Console, search for **IAM** and open the Identity and Access Management service.  
![AWS Admin Access](/images/001/2.png)

### 3. Create a New User
Click **Users** → **Add users**.  
![AWS Admin Access](/images/001/3.png)  
Enter a username (e.g., `admin-user`).  
Select **Password** or **Access key** authentication depending on your needs.  
![AWS Admin Access](/images/001/4.png)

### 4. Assign Permissions
Choose **Attach existing policies directly**.  
Select **AdministratorAccess** policy.  
![AWS Admin Access](/images/001/5.png)

### 5. Complete and Save Credentials
Click **Create user**.  
Download or securely store the access credentials.  

## Result
![AWS Admin Access](/images/001/6.png)  
![AWS Admin Access](/images/001/7.png)  
![AWS Admin Access](/images/001/8.png)  

You now have an IAM user with full administrative access.
