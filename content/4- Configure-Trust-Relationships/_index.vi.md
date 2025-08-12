---
title: "4. Cấu hình Trust Relationships"
date: 2025-08-11
weight: 4
chapter: false
prev: "4."
---

## Các bước thực hiện

### 1. Truy cập AWS Directory Service
Đăng nhập AWS Management Console, vào **Directory Service** và chọn AWS Managed Microsoft AD của bạn.  
![Cấu hình Trust Relationships](/images/004/01.png)

---

### 2. Mở mục Trust Relationships
Trong trang chi tiết của Directory, chọn **Networking & security** → **Trust relationships**.  
![Cấu hình Trust Relationships](/images/004/02.png)

---

### 3. Thêm Trust mới
Nhấn **Add trust**.  
![Cấu hình Trust Relationships](/images/004/03.png)

---

### 4. Chọn hướng Trust
Chọn hướng trust:  
- **One-way incoming** – AD on-premises tin tưởng AWS Managed AD  
- **One-way outgoing** – AWS Managed AD tin tưởng AD on-premises  
- **Two-way** – Cả hai tin tưởng lẫn nhau  

Chọn **Forest trust** để hỗ trợ xác thực cross-domain.  
![Cấu hình Trust Relationships](/images/0041/04.png)

---

### 5. Cấu hình thông tin Trust
Nhập **FQDN** của domain cần trust, đặt mật khẩu trust (giống nhau ở cả hai phía), và chọn:  
- **Selective authentication** – kiểm soát truy cập chặt chẽ hơn  
- **Forest-wide authentication** – cho phép truy cập rộng hơn  
![Cấu hình Trust Relationships](/images/004/04.png)

---

### 6. Xác nhận và kiểm tra Trust
Nhấn **Create** và chờ quá trình thiết lập hoàn tất.  
Từ AD on-premises, tạo trust tương ứng bằng công cụ **Active Directory Domains and Trusts**.  
Kiểm tra trust từ cả hai phía để đảm bảo kết nối thành công.  
![Cấu hình Trust Relationships](/images/004/05.png)

---

## Kết quả
AWS Managed Microsoft AD và AD on-premises đã được kết nối qua trust relationships, cho phép xác thực và truy cập tài nguyên giữa hai môi trường.
