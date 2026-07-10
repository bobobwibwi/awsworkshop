---
title: "Nhật ký tuần 9 - Ôn tập chặng 2: Lưu trữ, Co giãn & Giám sát"
date: 2026-06-12
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Chủ đề tuần

Hoàn thiện việc ôn tập các kỹ thuật nâng cao về Database, chịu tải (Scaling) và giám sát luồng dữ liệu mạng.

### Mục tiêu tuần

* Ôn tập các luồng kết nối an toàn cho S3 và RDS.
* Thực hành lại cơ chế Load Balancer và Auto Scaling Group.
* Áp dụng CloudWatch và VPC Flow Logs vào kịch bản thực tế.

### Lịch công việc

| Ngày | Thứ | Nội dung công việc | Lab / Dự án |
|---|---|---|---|
| 15/06/2026 | Thứ 2 | Ôn tập S3 & RDS: Thiết lập Static Website và cấu hình RDS Multi-AZ kết nối với EC2 qua lớp mạng Private. | Ôn tập Lab 5 |
| 16/06/2026 | Thứ 3 | Cấu hình lại luồng ALB kết hợp Auto Scaling Group. Dùng công cụ stress test để kiểm tra khả năng scale-out tự động. | Ôn tập Lab 6 |
| 17/06/2026 | Thứ 4 | Phân tích VPC Flow Logs: Truy xuất và đọc hiểu các log traffic bị REJECT để nhận diện các IP có hành vi quét port. | Ôn tập Lab 7 |
| 18/06/2026 | Thứ 5 | Thiết lập CloudWatch Alarm và tích hợp SNS để tự động bắn email khi server vượt mức 80% CPU. | Hệ thống Cảnh báo |
| 19/06/2026 | Thứ 6 | Dọn dẹp sạch sẽ (Clean up) toàn bộ môi trường Lab ôn tập của 2 tuần qua để cắt giảm chi phí. | Clean up |

### Kết quả kỳ vọng

* Nắm vững cách thiết kế một hệ thống High Availability (HA) hoàn chỉnh, từ Frontend phân tải đến Backend cơ sở dữ liệu.
* Làm chủ được bộ công cụ giám sát, sẵn sàng ứng dụng vào Đồ án.

### Tham chiếu tuần 9

* Tài liệu hướng dẫn Auto Scaling & AWS CloudWatch.