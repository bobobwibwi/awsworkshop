---
title: "Nhật ký tuần 3 - Module 3: Kiến trúc mạng chuyên sâu Amazon VPC"
date: 2026-05-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Chủ đề tuần

Xây dựng kiến trúc mạng ảo chuyên biệt, kiểm soát luồng định tuyến và cho phép Private Subnet giao tiếp Internet an toàn.

### Mục tiêu tuần

* Xây dựng Custom VPC với việc chia chẻ các dải IP (CIDR block).
* Phân bổ Route Tables cho Public và Private Subnet.
* Triển khai NAT Gateway để kéo gói cập nhật hệ thống một cách bảo mật.

### Lịch công việc

| Ngày | Thứ | Nội dung công việc | Lab / Dự án |
|---|---|---|---|
| 04/05/2026 | Thứ 2 | Phân hoạch dải IP. Khởi tạo một Custom VPC chứa cả lớp Public Subnet và Private Subnet. | [Lab 000006 - Xây dựng Advanced VPC](https://000006.awsstudygroup.com) |
| 05/05/2026 | Thứ 3 | Cấu hình Internet Gateway (IGW). Chỉnh sửa Route Table cho Public Subnet trỏ đường truyền ra IGW. | [Lab 000006 - Xây dựng Advanced VPC](https://000006.awsstudygroup.com) |
| 06/05/2026 | Thứ 4 | Tạo các EC2 instance đóng vai trò Frontend (Public) và Backend (Private) để test phân lớp mạng. | Cloud Lab Environment |
| 07/05/2026 | Thứ 5 | Xin cấp Elastic IP. Tạo NAT Gateway tại Public Subnet và trỏ Route Table của Private Subnet ra NAT. | [Lab 000007 - NAT Gateway & Routing](https://000007.awsstudygroup.com) |
| 08/05/2026 | Thứ 6 | Troubleshooting sự cố: Chạy ping test từ máy Backend ra Internet qua NAT Gateway, trace route luồng traffic. | Troubleshooting |

### Kết quả kỳ vọng

* Hoàn thiện lab hạ tầng mạng cô lập với độ bảo mật cao.
* Đảm bảo server nội bộ ẩn mình hoàn toàn trước Internet nhưng vẫn kéo được các bản vá lỗi (patching).

### Tham chiếu tuần 3

* [Lab 000006 - Thiết kế mạng ảo nâng cao Amazon VPC](https://000006.awsstudygroup.com)
* [Lab 000007 - Thiết lập định tuyến an toàn với NAT Gateway](https://000007.awsstudygroup.com)