---
title: "Nhật ký tuần 7 - Module 7: Giám sát CloudWatch & Phân tích Log"
date: 2026-05-29
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Chủ đề tuần

Sử dụng bộ công cụ giám sát (Monitoring) để theo dõi sức khỏe hệ thống và thiết lập các kịch bản cảnh báo sự cố tự động.

### Mục tiêu tuần

* Theo dõi biểu đồ tài nguyên bằng CloudWatch Metrics.
* Tích hợp Simple Notification Service (SNS) để nhận Email Alert.
* Thu thập VPC Flow Logs hỗ trợ truy vết các hành vi mạng nghi vấn.

### Lịch công việc

| Ngày | Thứ | Nội dung công việc | Lab / Dự án |
|---|---|---|---|
| 01/06/2026 | Thứ 2 | Truy cập CloudWatch Metrics, tạo Dashboard giám sát thông số CPU, Network In/Out của cụm máy chủ EC2. | CloudWatch Basics |
| 02/06/2026 | Thứ 3 | Tạo Topic trên Amazon SNS và đăng ký email cá nhân. Liên kết SNS với Billing Alarm báo động cước phí. | [Lab 000027 - Tích hợp SNS & Alarms](https://000027.awsstudygroup.com) |
| 03/06/2026 | Thứ 4 | Tạo CloudWatch Alarm cảnh báo khi ứng dụng gặp tải bất thường và tự động bắn mail thông báo sự cố. | [Lab 000027 - Tích hợp SNS & Alarms](https://000027.awsstudygroup.com) |
| 04/06/2026 | Thứ 5 | Bật tính năng VPC Flow Logs. Phân tích nhật ký mạng để lọc các địa chỉ IP bị Security Group từ chối truy cập. | [Lab 000028 - Phân tích VPC Flow Logs](https://000028.awsstudygroup.com) |

### Kết quả kỳ vọng

* Nắm trong tay quyền kiểm soát trạng thái hệ thống, tự động hóa Email Alert khi có biến động bất thường.
* Biết cách dùng logs mạng để phân tích, điều tra sơ bộ rủi ro an toàn thông tin (như quét port, tấn công dò quét).

### Tham chiếu tuần 7

* [Lab 000027 - Thiết lập cảnh báo tự động với Amazon CloudWatch & SNS](https://000027.awsstudygroup.com)
* [Lab 000028 - Thu thập và phân tích luồng mạng với VPC Flow Logs](https://000028.awsstudygroup.com)