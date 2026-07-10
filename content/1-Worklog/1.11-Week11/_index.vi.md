---
title: "Nhật ký tuần 11 - Triển khai Đồ án thực tập (Final Project)"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Chủ đề tuần

Bắt tay vào thực thi: Triển khai hạ tầng và cấu hình hệ thống thực tế trên AWS dựa trên Proposal đã được duyệt.

### Mục tiêu tuần

* Triển khai kiến trúc mạng lõi an toàn (VPC, Subnets, Security Groups).
* Xây dựng tầng Compute và Database đảm bảo High Availability.
* Tích hợp các cơ chế bảo vệ và giám sát an toàn thông tin cho hệ thống.

### Lịch công việc

| Ngày | Thứ | Nội dung công việc | Lab / Dự án |
|---|---|---|---|
| 29/06/2026 | Thứ 2 | Khởi tạo Custom VPC cho đồ án. Phân hoạch IP chặt chẽ, cấu hình Internet Gateway và NAT Gateway. | Thực thi Đồ án |
| 30/06/2026 | Thứ 3 | Cấu hình tầng Database (RDS) hoàn toàn cách ly trong Private Subnet, thiết lập Security Group chỉ cho phép IP nội bộ. | Thực thi Đồ án |
| 01/07/2026 | Thứ 4 | Đóng gói AMI hệ điều hành, tạo Launch Template và thiết lập Auto Scaling Group kết nối với ALB. | Thực thi Đồ án |
| 02/07/2026 | Thứ 5 | Tích hợp giám sát: Bật CloudWatch, cấu hình SNS gửi email cảnh báo khi hệ thống có dấu hiệu quá tải. | Thực thi Đồ án |
| 03/07/2026 | Thứ 6 | Kiểm thử toàn diện (Testing): Giả lập lỗi sập server để test khả năng tự phục hồi của Auto Scaling Group. | Kiểm thử hệ thống |

### Kết quả kỳ vọng

* Hạ tầng đồ án được dựng thành công, chạy trơn tru theo đúng bản vẽ kiến trúc.
* Hệ thống được thiết kế theo tư duy "kín kẽ", đáp ứng tốt các yêu cầu về bảo mật mạng và tính sẵn sàng cao.

### Tham chiếu tuần 11

* Bản thiết kế kiến trúc Đồ án cá nhân (Proposal).
* Tài liệu thực hành AWS Well-Architected Framework.