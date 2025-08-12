---
title: "5. Di chuyển Người dùng và Nhóm"
date: 2025-08-11
weight: 5
chapter: false
prev: "5."
---

## Các bước thực hiện

### 1. Cài đặt và cấu hình ADMT
Triển khai ADMT trên một máy chủ Windows Server là thành viên của miền AWS Managed AD đích.  
Đảm bảo máy chủ ADMT có thể kết nối tới cả hai miền.  
Nếu cần di chuyển mật khẩu, cài đặt **Password Export Server (PES)** trên bộ điều khiển miền của miền nguồn và cấu hình khóa mã hóa.

---

### 2. Lập kế hoạch di chuyển
Xác định các Đơn vị Tổ chức (OU) cần di chuyển.  
Tạo kế hoạch di chuyển theo từng đợt:  
- Tài khoản quan trọng trước (quản trị viên, tài khoản dịch vụ)  
- Người dùng thông thường  
- Nhóm bảo mật và nhóm phân phối

---

### 3. Di chuyển tài khoản người dùng
Sử dụng ADMT **User Account Migration Wizard** để:  
- Chọn miền nguồn và miền đích  
- Chọn các tài khoản cần di chuyển  
- Bật tùy chọn “Di chuyển các nhóm người dùng liên quan”  
- Tùy chọn di chuyển mật khẩu (yêu cầu PES)  
Kiểm tra nhật ký di chuyển để đảm bảo không có lỗi.

---

### 4. Di chuyển nhóm
Sử dụng ADMT **Group Migration Wizard** để:  
- Giữ nguyên phạm vi nhóm (Global, Universal, Domain Local)  
- Duy trì tính toàn vẹn của thành viên nhóm

---

### 5. Xác minh sau di chuyển
Đăng nhập bằng các tài khoản đã di chuyển để xác nhận khả năng xác thực trên AWS AD.  
Xác minh rằng quyền và thành viên nhóm vẫn giữ nguyên.  
Cập nhật các ứng dụng hoặc dịch vụ sử dụng AWS Managed Microsoft AD.

---

## Thực tiễn tốt nhất
- Thực hiện **di chuyển thử nghiệm** trước khi di chuyển toàn bộ trong môi trường sản xuất.  
- Sao lưu cả hai môi trường AD trước khi bắt đầu.  
- Lên lịch di chuyển vào thời gian ít người dùng.  
- Ghi chép lại mọi đối tượng đã di chuyển để phục vụ kiểm tra và khôi phục khi cần.
