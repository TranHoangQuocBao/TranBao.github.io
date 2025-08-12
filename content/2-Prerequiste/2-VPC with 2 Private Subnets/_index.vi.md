---
title: "2 - VPC với 2 Private Subnets"
date: 2025-08-11
weight: 2
chapter: false
prev: "2.2"
---

## Các bước thực hiện

### 1. Mở bảng điều khiển VPC
- Đăng nhập vào **AWS Management Console**.
- Truy cập dịch vụ **VPC**.
![VPC với 2 Private Subnets](/images/002/1.png)

### 2. Tạo VPC mới
- Nhấn **Create VPC**.
- Tên: `ProjectVPC` (ví dụ).
- IPv4 CIDR block: ví dụ `10.0.0.0/16`.
- Tenancy: **Default**.
- Nhấn **Create VPC**.
![VPC với 2 Private Subnets](/images/002/2.png)

### 3. Tạo Private Subnets
- Vào **Subnets** → **Create subnet**.
- Chọn VPC vừa tạo.
- Tạo **Private Subnet 1** ở Availability Zone 1 với CIDR (ví dụ `10.0.1.0/24`).
- Tạo **Private Subnet 2** ở Availability Zone 2 với CIDR (ví dụ `10.0.2.0/24`).
![VPC với 2 Private Subnets](/images/002/3.png)

### 4. Cấu hình Route Table
- Đảm bảo cả hai subnet đều liên kết với route table private (không kết nối trực tiếp tới internet gateway).
![VPC với 2 Private Subnets](/images/002/done.png)

### 5. Kiểm tra
- Xác nhận VPC có ít nhất **hai private subnet** nằm ở **hai Availability Zones khác nhau**.
![VPC với 2 Private Subnets](/images/002/5.png)

## Kết quả
Bạn đã có một VPC hoàn chỉnh với hai private subnet ở hai AZ khác nhau.
