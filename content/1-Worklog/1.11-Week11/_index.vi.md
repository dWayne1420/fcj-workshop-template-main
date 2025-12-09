---
title: "Worklog Tuần 11"
date: 2025-11-17
weight: 1
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu Tuần 11:
- Học nền tảng container Docker.
- Push image lên Amazon ECR.
- Deploy service bằng Amazon ECS (EC2/Fargate).
- Cấu hình ECS Networking & Auto Scaling.
- Hiểu workflow điều phối container.

### Công việc:

| Ngày | Công việc                      | Ngày  | Hoàn thành | Tham khảo |
| ---- | ------------------------------ | ------ | ---------- | ---------- |
| 51   | Học kiến thức Docker cơ bản    | 11/17  | 11/17      | https://cloudjourney.awsstudygroup.com/ |
| 52   | Tạo ECR Repository             | 11/18  | 11/18      | https://cloudjourney.awsstudygroup.com/ |
| 53   | Build & Push image lên ECR     | 11/19  | 11/19      | https://cloudjourney.awsstudygroup.com/ |
| 54   | Deploy ECS (EC2/Fargate)       | 11/20  | 11/20      | https://cloudjourney.awsstudygroup.com/ |
| 55   | ECS Networking & Auto Scaling  | 11/21  | 11/21      | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 11:

- **Học nền tảng Docker**, gồm:
  - Image vs Container
  - Dockerfile commands
  - Multi-stage builds
  - Tagging & versioning
  - Container networking

- **Build Docker Image**, gồm:
  - Tạo Dockerfile cho Node.js app
  - Tối ưu layer giảm kích thước image
  - Dùng `.dockerignore`
  - Test container local

- **Tạo Amazon ECR Repository**, gồm:
  - Tạo private registry  
  - Login bằng AWS CLI  
  - Tag & push image

- **Triển khai ứng dụng bằng ECS**, gồm:
  - Task Definition
  - CPU/memory config
  - Environment variables
  - ECS Service
  - Tích hợp ALB
  - Set số lượng replicas

- **Sử dụng AWS Fargate**, gồm:
  - Không cần EC2 host
  - Compute fully-managed
  - Auto-scaling

- **Cấu hình ECS Networking**, gồm:
  - Chọn subnet VPC
  - Deploy vào private/public
  - Security Group cho tasks
  - IAM Role cho ECS Tasks

- **Test Auto Scaling ECS**, gồm:
  - Scale khi CPU tăng
  - Giới hạn min/max task
  - Load test kích hoạt scaling

- **Đạt khả năng deploy workload container bằng ECS + ECR + Fargate.**
