---
title: "1 - Tài khoản AWS quyền Quản trị"
date: 2025-08-11
weight: 2
chapter: false
prev: "1."
---

## Các bước thực hiện

### 1. Đăng nhập AWS Management Console
Truy cập [https://aws.amazon.com/](https://aws.amazon.com/) và đăng nhập bằng tài khoản root AWS của bạn.  
![AWS Admin Access](/images/001/1.png)

### 2. Mở IAM Console
Trong AWS Console, tìm kiếm **IAM** và mở dịch vụ **Identity and Access Management**.  
![AWS Admin Access](/images/001/2.png)

### 3. Tạo người dùng mới
Chọn **Users** → **Add users**.  
![AWS Admin Access](/images/001/3.png)  
Nhập tên người dùng (ví dụ: `admin-user`).  
Chọn hình thức xác thực **Password** hoặc **Access key** tùy nhu cầu.  
![AWS Admin Access](/images/001/4.png)

### 4. Gán quyền
Chọn **Attach existing policies directly**.  
Tích chọn chính sách **AdministratorAccess**.  
![AWS Admin Access](/images/001/5.png)

### 5. Hoàn tất và lưu thông tin đăng nhập
Nhấn **Create user**.  
Tải xuống hoặc lưu trữ an toàn thông tin đăng nhập (credentials).  

## Kết quả
![AWS Admin Access](/images/001/6.png)  
![AWS Admin Access](/images/001/7.png)  
![AWS Admin Access](/images/001/8.png)  

Bạn đã có một IAM user với toàn quyền quản trị trên AWS.
