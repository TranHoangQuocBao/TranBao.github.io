---
title: "3. Tạo AWS Managed Microsoft AD"
date: 2025-08-11
weight: 3
chapter: false
prev: "2."
---

## Các bước thực hiện

### 1. Mở AWS Management Console
Mở **AWS Management Console** và điều hướng tới **Directory Service**.  

---

### 2. Nhấn "Set up directory"
Nhấn **Set up directory**.  
![AWS Managed AD Step 2](/images/003/anh1.png)

---

### 3. Chọn AWS Managed Microsoft AD
Chọn **AWS Managed Microsoft AD** và nhấn **Next**.  
![AWS Managed AD Step 3](/images/003/anh2.png)

---

### 4. Chọn phiên bản
- **Standard Edition**: Tối đa 30,000 object, phù hợp với môi trường nhỏ.  
- **Enterprise Edition**: Tối đa 500,000 object, phù hợp với tổ chức lớn.  
![AWS Managed AD Step 4](/images/003/anh3.png)

---

### 5. Điền thông tin Directory
Nhập tên DNS của directory, tên NetBIOS và mật khẩu admin.  
![AWS Managed AD Step 5](/images/003/anh4.png)

---

### 6. Cấu hình VPC
Chọn **VPC** và 2 subnet ở 2 Availability Zone khác nhau.  
![AWS Managed AD Step 6](/images/003/anh5.png)

---

### 7. Kiểm tra và tạo
Kiểm tra lại tất cả cài đặt và nhấn **Create directory**.  
![AWS Managed AD Step 7](/images/003/anh6.png)

---

### 8. Chờ trạng thái Active
Chờ trạng thái chuyển sang **Active** (khoảng 20–45 phút).  
![AWS Managed AD Step 8](/images/003/anh7.png)

---

## Kết quả mong đợi
Một AWS Managed Microsoft AD được tạo, khả dụng trong VPC của bạn và sẵn sàng cho cấu hình tiếp theo.
