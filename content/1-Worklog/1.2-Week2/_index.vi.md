---
title: "Nhật ký tuần 2 - Module 2: Điện toán đám mây Amazon EC2 & EBS"
date: 2026-04-24
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Chủ đề tuần

Triển khai, cấu hình máy chủ ảo Amazon EC2 và cấp phát lưu trữ EBS.

### Mục tiêu tuần

* Khởi tạo và kết nối SSH an toàn vào máy chủ EC2 Linux.
* Cấu hình Inbound/Outbound rules trong Security Group.
* Mở rộng không gian lưu trữ với ổ cứng Elastic Block Store (EBS).

### Lịch công việc

| Ngày | Thứ | Nội dung công việc | Lab / Dự án |
|---|---|---|---|
| 27/04/2026 | Thứ 2 | Khởi tạo máy chủ t2.micro đầu tiên. Thực hành kết nối SSH thông qua Key Pair (file .pem). | [Lab 000004 - Giới thiệu Amazon EC2](https://000004.awsstudygroup.com) |
| 28/04/2026 | Thứ 3 | Tìm hiểu Security Group. Mở port 22 (SSH) cho IP cá nhân và port 80 (HTTP) ra Internet. | [Lab 000004 - Giới thiệu Amazon EC2](https://000004.awsstudygroup.com) |
| 29/04/2026 | Thứ 4 | Viết kịch bản User Data tự động cài đặt Apache Web Server ngay lúc khởi động EC2. Kiểm thử truy cập web. | Scripting / User Data |
| 30/04/2026 | Thứ 5 | Tạo thêm một EBS Volume mới, attach vào EC2 đang chạy và thực hiện các lệnh Linux để mount phân vùng. | [Lab 000005 - Lưu trữ với Amazon EBS](https://000005.awsstudygroup.com) |

### Kết quả kỳ vọng

* Host thành công một trang web cơ bản trên EC2.
* Siết chặt được hàng rào bảo mật ở lớp network (Security Group).
* Thành thạo thao tác cấp phát và mount ổ cứng ảo EBS mà không làm hỏng OS.

### Tham chiếu tuần 2

* [Lab 000004 - Giới thiệu và cấu hình Amazon EC2](https://000004.awsstudygroup.com)
* [Lab 000005 - Quản lý không gian lưu trữ với Amazon EBS](https://000005.awsstudygroup.com)