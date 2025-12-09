---
title: "Worklog Tuần 3"
date: 2025-09-22
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu Tuần 3:
- Khám phá các tính năng nâng cao của Amazon EC2.
- Cài đặt và cấu hình LAMP stack trên EC2.
- Triển khai ứng dụng Node.js trên EC2.
- Thiết lập IAM governance để kiểm soát chi phí.
- Học cách ứng dụng truy cập AWS một cách bảo mật.

### Công việc:

| Ngày | Công việc                                 | Bắt đầu | Kết thúc | Tham khảo |
| ---- | ----------------------------------------- | ------- | -------- | ---------- |
| 11   | Khám phá EC2 nâng cao                     | 09/22   | 09/22    | https://cloudjourney.awsstudygroup.com/ |
| 12   | Cài đặt LAMP Web Server                   | 09/23   | 09/23    | https://cloudjourney.awsstudygroup.com/ |
| 13   | Deploy ứng dụng Node.js                   | 09/24   | 09/24    | https://cloudjourney.awsstudygroup.com/ |
| 14   | Implement Cost Governance bằng IAM        | 09/25   | 09/25    | https://cloudjourney.awsstudygroup.com/ |
| 15   | Application Access to AWS Services        | 09/26   | 09/26    | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 3:

- **Khám phá chi tiết EC2**, bao gồm:
  - Các họ instance (General, Compute, Memory Optimized)
  - Các trạng thái và vòng đời instance
  - EBS (gp3, io2, thông lượng)
  - ENI, IP Public/Private, Elastic IP
  - Security Groups & network integration
  - AMI & Snapshot
  - User Data script để tự động hóa

- **Cài đặt đầy đủ LAMP stack (Linux + Apache + MySQL + PHP)**:
  - Cài Apache
  - Cấu hình Virtual Host
  - Cài PHP và Extensions
  - Tích hợp PHP + Apache
  - Cài và cấu hình MySQL
  - Deploy website PHP test
  - Bảo mật tài khoản root MySQL

- **Triển khai ứng dụng Node.js**, gồm:
  - Cài Node.js + NPM
  - Cài PM2 để chạy app nền
  - Tạo systemd service cho PM2
  - Cấu hình firewall + SG
  - Reverse proxy bằng NGINX
  - Deploy + kiểm thử Node app

- **Triển khai IAM Cost Governance**, gồm:
  - Quyền billing chỉ đọc
  - Budget và cost alerts
  - Cost Explorer
  - Policy giới hạn tài nguyên tốn phí cao

- **Học cách ứng dụng truy cập AWS một cách bảo mật**:
  - IAM Role cho EC2
  - Instance metadata IMDSv2
  - Truy cập S3 bằng SDK
  - Sử dụng temporary credentials

- **Thực hành CLI EC2**:
  - `describe-instances`
  - start/stop EC2
  - tạo snapshot EBS
  - lấy CloudWatch metrics bằng CLI

- **Nắm được cách triển khai ứng dụng Fullstack trên EC2.**
