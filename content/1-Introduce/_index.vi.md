---
title: "Giới thiệu"
date: 2025-08-12T00:00:00+07:00
weight: 1
chapter: false
pre: "<b>1. </b>"
---

# Giới thiệu về Tích hợp Active Directory với AWS Managed Microsoft AD

## Tổng quan
AWS Managed Microsoft AD là dịch vụ thư mục được quản lý bởi AWS, cho phép tổ chức vận hành Microsoft Active Directory trên nền tảng đám mây AWS mà không cần quản lý thủ công các Domain Controller.  
Giải pháp này hỗ trợ tích hợp liền mạch với môi trường Active Directory tại chỗ, cho phép thiết lập mối quan hệ tin cậy, đồng bộ người dùng và xác thực tập trung cho cả ứng dụng đám mây và tại chỗ.

## Lợi ích chính

### 1. Quản lý tập trung
- Đồng bộ người dùng và nhóm giữa AD tại chỗ và AWS.
- Quản lý quyền và chính sách truy cập tại một nơi duy nhất.
- Giảm bớt các tác vụ lặp lại khi tạo và cấu hình tài khoản.

### 2. Nâng cao bảo mật
- Tích hợp Xác thực đa yếu tố (MFA) và Đăng nhập một lần (SSO).
- Thực thi chính sách bảo mật thông qua Group Policy Objects (GPOs).
- Mã hóa dữ liệu khi truyền và khi lưu trữ.

### 3. Khả năng mở rộng linh hoạt
- Dễ dàng mở rộng dung lượng người dùng và nhóm mà không cần mua thêm phần cứng.
- Triển khai Multi-AZ để đảm bảo tính sẵn sàng cao và khả năng chịu lỗi.
- Tích hợp với các dịch vụ AWS như Amazon EC2, RDS và WorkSpaces.

### 4. Giảm gánh nặng vận hành
- Loại bỏ nhu cầu duy trì máy chủ AD vật lý.
- Tự động cập nhật bản vá và phần mềm.
- Tối ưu chi phí với mô hình trả phí theo mức sử dụng.

## Thành phần chính
1. **AWS Managed Microsoft AD** – Dịch vụ chính cung cấp hạ tầng Active Directory được quản lý toàn diện trên AWS.
2. **Quan hệ tin cậy (Trust Relationships)** – Cho phép xác thực chéo miền và tích hợp với AD hiện có.
3. **AWS IAM Identity Center / SSO** – Đăng nhập một lần t
