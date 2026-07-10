---
title: "Nhật ký tuần 5 - Module 5: Cơ sở dữ liệu đám mây Amazon RDS"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Chủ đề tuần

Sử dụng dịch vụ Managed Database để loại bỏ gánh nặng vận hành OS, tập trung vào bảo mật tầng dữ liệu.

### Mục tiêu tuần

* Khởi tạo máy chủ Amazon RDS (MySQL/PostgreSQL) an toàn trong Private Subnet.
* Đảm bảo tính khả dụng (High Availability) bằng tùy chọn Multi-AZ.
* Cấu hình Security Group cho phép EC2 đọc/ghi vào Database.

### Lịch công việc

| Ngày | Thứ | Nội dung công việc | Lab / Dự án |
|---|---|---|---|
| 18/05/2026 | Thứ 2 | Khởi tạo Subnet Group bao gồm các Private Subnet trải đều trên nhiều vùng AZ khác nhau. | Cấu hình Network |
| 19/05/2026 | Thứ 3 | Tạo phiên bản Amazon RDS MySQL, cấu hình Master Password và vô hiệu hóa Public Access. | [Lab 000015 - Triển khai Amazon RDS](https://000015.awsstudygroup.com) |
| 20/05/2026 | Thứ 4 | Thiết lập Security Group RDS: Chỉ chấp nhận lưu lượng port 3306 đến từ Security Group của EC2 Web Server. | Network Security |
| 21/05/2026 | Thứ 5 | Đứng từ EC2, dùng MySQL Client kết nối thử vào Endpoint của RDS. Tạo Snapshot sao lưu nhanh và dọn dẹp. | [Lab 000015 - Triển khai Amazon RDS](https://000015.awsstudygroup.com) |

### Kết quả kỳ vọng

* Cơ sở dữ liệu được cách ly tuyệt đối, không thể truy cập trực tiếp từ Internet.
* Giao tiếp thành công tuyến đường nội bộ an toàn giữa tầng Compute và tầng Database.

### Tham chiếu tuần 5

* [Lab 000015 - Khởi tạo và thiết lập Cơ sở dữ liệu Amazon RDS](https://000015.awsstudygroup.com)