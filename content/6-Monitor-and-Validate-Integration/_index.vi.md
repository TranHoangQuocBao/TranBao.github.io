---
title: "6. Giám sát và Xác minh Tích hợp"
date: 2025-08-11
weight: 6
chapter: false
prev: "4."
---

## Các bước thực hiện

### 1. Thiết lập công cụ giám sát
- **Amazon CloudWatch**: Theo dõi các chỉ số về tình trạng dịch vụ thư mục, trạng thái trust và quá trình replication.
- **AWS CloudTrail**: Ghi lại và xem xét các thay đổi đối với môi trường AD.
- **AWS Directory Service Console**: Kiểm tra trạng thái và nhật ký.

---

### 2. Xác minh Trust Relationship
- Sử dụng **Active Directory Domains and Trusts** để xác nhận trust đã được thiết lập và đang hoạt động.
- Chạy lệnh `nltest /sc_query:<TrustedDomain>` để kiểm tra trạng thái kênh bảo mật.

---

### 3. Kiểm tra hoạt động của Người dùng và Nhóm
- Thử đăng nhập người dùng từ cả hai môi trường.
- Xác nhận nhóm và quyền được đồng bộ.

---

## Thực hành tốt nhất
- Bật cảnh báo CloudWatch cho lỗi trust hoặc replication.
- Thiết lập kiểm tra tự động định kỳ.
- Lưu lại toàn bộ kết quả và điều chỉnh khi cần.
