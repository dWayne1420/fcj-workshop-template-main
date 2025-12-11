---
title: "Worklog Tuần 6"
date: 2025-10-13
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu Tuần 6:
- Nghiên cứu và đánh giá dịch vụ AWS cho kiến trúc dự án.
- Thiết kế sơ đồ kiến trúc hệ thống hoàn chỉnh.
- Xây dựng thiết kế database chi tiết.
- Viết tài liệu kiến trúc kỹ thuật.
- Ghi lại quá trình học và tham gia cộng đồng.

### Công việc:

| Ngày | Công việc                                | Ngày  | Hoàn thành | Tham khảo |
| ---- | ---------------------------------------- | ------ | ---------- | ---------- |
| 26   | Tìm hiểu dịch vụ cho dự án               | 10/13  | 10/13      | https://cloudjourney.awsstudygroup.com/ |
| 27   | Vẽ sơ đồ kiến trúc hệ thống              | 10/14  | 10/14      | https://cloudjourney.awsstudygroup.com/ |
| 28   | Thiết kế cơ sở dữ liệu                   | 10/15  | 10/15      | https://cloudjourney.awsstudygroup.com/ |
| 29   | Chỉnh sửa sơ đồ + viết tài liệu kỹ thuật | 10/16  | 10/16      | https://cloudjourney.awsstudygroup.com/ |
| 30   | Ghi lại các sự kiện đã tham gia          | 10/17  | 10/17      | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 6:

- **Nghiên cứu chi tiết dịch vụ AWS**, gồm:
  - Compute: EC2, Lambda, Lightsail, Fargate
  - Storage: S3, EFS, RDS, DynamoDB
  - Networking: VPC, CloudFront, API Gateway, Route 53
  - Monitoring & DevOps
  - So sánh chi phí, hiệu năng, độ phức tạp

- **Thiết kế sơ đồ kiến trúc hoàn chỉnh**:
  - VPC với Public/Private Subnet
  - Internet Gateway + NAT Gateway
  - Compute Flow: EC2 hoặc Lambda
  - RDS/DynamoDB làm data layer
  - CloudFront làm CDN
  - S3 cho file/static content
  - IAM Roles theo từng service
  - CloudWatch cho giám sát
  - Sử dụng AWS Icons chuẩn

- **Thiết kế database**, gồm:
  - Sơ đồ ERD
  - Cấu trúc bảng
  - Primary Key + Foreign Key
  - Normalization vs Optimization
  - Indexing plan
  - Migration plan

- **Viết tài liệu kỹ thuật**, gồm:
  - High-level overview
  - Mô tả thành phần hệ thống
  - Sơ đồ luồng dữ liệu
  - Thiết kế API
  - Deployment plan
  - IAM Role mapping
  - Monitoring & logging plan

- **Chỉnh sửa sơ đồ theo feedback**, cải thiện:
  - Bảo mật (giảm rule SG)
  - Chi phí (NAT Gateway → NAT Instance)
  - Hiệu năng (đưa static lên CloudFront)

- **Hoàn thành phần Events Participated**, ghi lại:
  - Các buổi workshop đã tham gia
  - Bài học rút ra
  - Hoạt động cộng đồng

- **Hình thành khả năng lập kế hoạch – thiết kế – tài liệu hóa kiến trúc AWS Production-ready.**
