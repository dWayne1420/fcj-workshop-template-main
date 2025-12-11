---
title: "Worklog Tuần 12"
date: 2025-11-24
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu Tuần 12:
- Deploy đầy đủ dự án theo kiến trúc đã thiết kế.
- Tích hợp monitoring, CI/CD, serverless, container.
- Tối ưu hiệu năng, chi phí, bảo mật.
- Kiểm thử toàn hệ thống & sửa lỗi.
- Viết tài liệu hoàn chỉnh cho dự án cuối kỳ.

### Công việc tuần này:

| Ngày | Công việc                           | Ngày  | Hoàn thành |
| ---- | ----------------------------------- | ------ | ---------- |
| 56   | Deploy toàn bộ dự án hoàn chỉnh    | 11/24  | 11/24      |
| 57   | Tối ưu chi phí & bảo mật           | 11/25  | 11/25      |
| 58   | Kiểm thử hiệu năng & tải            | 11/26  | 11/26      |
| 59   | Fix bug & cải thiện độ ổn định      | 11/27  | 11/27      |

### Thành tựu Tuần 12:

- **Deploy thành công kiến trúc toàn hệ thống**, gồm:
  - VPC (public/private subnet)
  - Compute layer: EC2 hoặc Lambda
  - S3 + CloudFront hosting
  - Database layer: RDS/DynamoDB
  - API Gateway
  - CloudWatch Dashboards
  - CI/CD Pipeline
  - ECS containers

- **Tích hợp monitoring đầy đủ**:
  - CloudWatch Alarms (CPU, memory, custom)
  - Logs tập trung CloudWatch Logs
  - Thông báo SNS
  - Dashboard giám sát tập trung

- **Tối ưu chi phí**, gồm:
  - Rightsizing EC2
  - S3 Lifecycle
  - Glacier Archive
  - DynamoDB On-Demand
  - Kiểm tra chi phí trên Cost Explorer

- **Kiểm thử hiệu năng**, gồm:
  - Load test API
  - Stress test EC2 Auto Scaling
  - Kiểm tra ECS scale-out
  - Kiểm tra tốc độ CloudFront toàn cầu

- **Cải thiện độ ổn định**, gồm:
  - Sửa lỗi latency
  - Fix IAM permission
  - Khắc phục Target Group unhealthy
  - Tối ưu hóa indexing DB

- **Hoàn thiện tài liệu dự án**, gồm:
  - Sơ đồ kiến trúc cuối cùng
  - Tài liệu API
  - Hướng dẫn triển khai
  - Quy trình bảo mật
  - Logging & alerting SOP
  - Báo cáo chi phí & tối ưu

- **Đạt mức sẵn sàng triển khai production thực tế trên AWS.**
