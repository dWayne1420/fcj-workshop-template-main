---
title: "Worklog Tuần 8"
date: 2025-10-27
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu Tuần 8:
- Hiểu kiến trúc và thành phần của Elastic Beanstalk.
- Triển khai ứng dụng đa tầng bằng EB.
- Nắm Load Balancers và các môi trường EB.
- Cấu hình Auto Scaling và các trigger.
- Quản lý vòng đời ứng dụng trên EB.

### Công việc:

| Ngày | Công việc                          | Ngày  | Hoàn thành | Tham khảo |
| ---- | ---------------------------------- | ------ | ---------- | ---------- |
| 36   | Giới thiệu Elastic Beanstalk       | 10/27  | 10/27      | https://cloudjourney.awsstudygroup.com/ |
| 37   | Deploy ứng dụng lên EB             | 10/28  | 10/28      | https://cloudjourney.awsstudygroup.com/ |
| 38   | Cấu hình Load Balancer             | 10/29  | 10/29      | https://cloudjourney.awsstudygroup.com/ |
| 39   | Cấu hình Auto Scaling              | 10/30  | 10/30      | https://cloudjourney.awsstudygroup.com/ |
| 40   | Update & Redeploy ứng dụng         | 10/31  | 10/31      | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 8:

- **Nắm vững khái niệm Elastic Beanstalk**, gồm:
  - Môi trường EB (Web Server vs Worker)
  - Phiên bản Platform (Node.js, Python, PHP…)
  - ASG & Load Balancer tự tạo
  - Chiến lược triển khai: Rolling, Immutable, Blue/Green

- **Triển khai ứng dụng hoàn chỉnh lên EB**:
  - Tạo Application & Environment
  - Upload bản code dạng ZIP
  - EB tự tạo:
    - EC2
    - Security Groups
    - Auto Scaling Group
    - Load Balancer
  - Kiểm tra health + logs

- **Cấu hình ALB (Application Load Balancer)**:
  - Path-based routing
  - Health Check chuẩn
  - Listener Rules
  - Kiểm tra sticky session

- **Cấu hình Auto Scaling**:
  - Target Tracking (CPU > 50%)
  - Step Scaling (CPU > 70% → scale out)
  - Min/Max instance
  - Test bằng simulated load

- **Thực hiện các tác vụ vòng đời ứng dụng**:
  - Deploy version mới
  - Rollback
  - Tùy chỉnh qua `.ebextensions`
  - Lấy log bằng tail logs

- **Sử dụng EB CLI**:
  - `eb init`, `eb create`, `eb deploy`, `eb status`
  - Quản lý version dễ dàng

- **Đạt khả năng deploy & auto-scale workload sản xuất bằng Elastic Beanstalk.**
