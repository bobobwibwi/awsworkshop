---
title: "Nhật ký tuần 6 - Module 6: Cân bằng tải ELB & Auto Scaling"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Chủ đề tuần

Giải quyết bài toán thắt cổ chai hiệu suất: Tự động chia tải và co giãn số lượng máy chủ dựa trên lưu lượng thực tế.

### Mục tiêu tuần

* Cấu hình Application Load Balancer (ALB) điều phối traffic.
* Đóng gói AMI và tạo Launch Template chuẩn.
* Xây dựng Auto Scaling Group (ASG) hỗ trợ Scale Out/Scale In tự động.

### Lịch công việc

| Ngày | Thứ | Nội dung công việc | Lab / Dự án |
|---|---|---|---|
| 25/05/2026 | Thứ 2 | Tạo Amazon Machine Image (AMI) từ một con EC2 đã cài cắm sẵn source code web ổn định. | [Lab 000019 - Đóng gói AMI](https://000019.awsstudygroup.com) |
| 26/05/2026 | Thứ 3 | Tạo Launch Template dựa trên AMI vừa sinh ra, định hình instance type, key pair và security group dùng chung. | [Lab 000021 - Tạo Launch Templates](https://000021.awsstudygroup.com) |
| 27/05/2026 | Thứ 4 | Thiết lập Application Load Balancer (ALB). Cấu hình Target Group và Health Check để nhận diện các máy chủ. | [Lab 000020 - Cân bằng tải với ELB](https://000020.awsstudygroup.com) |
| 28/05/2026 | Thứ 5 | Khởi tạo Auto Scaling Group (ASG) gắn vào ALB. Viết Scaling Policy tự tăng server nếu CPU vượt ngưỡng 70%. | [Lab 000022 - Thiết lập Auto Scaling](https://000022.awsstudygroup.com) |
| 29/05/2026 | Thứ 6 | Dùng Apache Benchmark chạy stress test để đẩy tải server lên cao, theo dõi log xem ASG sinh thêm EC2. | Stress Testing |

### Kết quả kỳ vọng

* Đảm bảo hệ thống duy trì được tính High Availability ngay cả khi một máy chủ bị sập đột ngột.
* Năng lực hệ thống tự phình to khi có bão traffic và tự thu hẹp lại khi vắng khách để tối ưu hóa chi phí.

### Tham chiếu tuần 6

* [Lab 000020 - Phân phối lưu lượng truy cập với Elastic Load Balancing](https://000020.awsstudygroup.com)
* [Lab 000022 - Tự động hóa mở rộng với Auto Scaling Group](https://000022.awsstudygroup.com)