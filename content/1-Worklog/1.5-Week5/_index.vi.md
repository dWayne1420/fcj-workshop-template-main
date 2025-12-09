---
title: "Worklog Tuần 5"
date: 2025-10-06
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu Tuần 5:
- Hiểu cơ sở dữ liệu quan hệ trên AWS qua Amazon RDS.
- Triển khai database được quản lý trên AWS Lightsail.
- Học triển khai container bằng Lightsail Containers.
- Tìm hiểu NoSQL thông qua DynamoDB.
- Bắt đầu làm việc với AWS bằng lập trình qua SDK.

### Công việc:

| Ngày | Công việc                                   | Ngày  | Hoàn thành | Tham khảo |
| ---- | ------------------------------------------- | ------ | ---------- | ---------- |
| 21   | Học Amazon RDS                              | 10/06  | 10/06      | https://cloudjourney.awsstudygroup.com/ |
| 22   | Triển khai Database trên Lightsail          | 10/07  | 10/07      | https://cloudjourney.awsstudygroup.com/ |
| 23   | Deploy Containers trên Lightsail            | 10/08  | 10/08      | https://cloudjourney.awsstudygroup.com/ |
| 24   | Làm việc với Amazon DynamoDB                | 10/09  | 10/09      | https://cloudjourney.awsstudygroup.com/ |
| 25   | Bắt đầu với AWS SDK                         | 10/10  | 10/10      | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 5:

- **Nắm vững các khái niệm của Amazon RDS**, gồm:
  - Các loại engine (MySQL, PostgreSQL, MariaDB)
  - Reserved Instance, Multi-AZ, Read Replica
  - Backup tự động, snapshot, maintenance window
  - Parameter Group & Security Group
  - Endpoint Public vs Private

- **Tạo một Amazon RDS Instance**, gồm:
  - Chọn phiên bản DB engine
  - Chọn Instance Class + storage
  - Cấu hình bảo mật (Public Access + SG port 3306)
  - Tạo database khởi tạo và kết nối bằng MySQL Workbench

- **Triển khai Lightsail Managed Database**, gồm:
  - So sánh ưu/nhược với RDS
  - Tạo Private Static IP
  - Kết nối app ↔ DB Lightsail
  - Cấu hình backup & failover

- **Triển khai ứng dụng bằng Lightsail Containers**, gồm:
  - Build Docker image
  - Push image lên Lightsail Container Registry
  - Tạo deployment + scale
  - Config environment variables

- **Học DynamoDB**, gồm:
  - Partition key / Sort key
  - Provisioned vs On-Demand
  - DynamoDB Streams
  - GSI & LSI
  - NoSQL design best practices

- **Thực hành DynamoDB**, gồm:
  - Tạo bảng
  - Thêm item
  - Query + Scan bằng Console và CLI

- **Bắt đầu với AWS SDK**, gồm:
  - Cài AWS SDK (JavaScript hoặc Python)
  - Viết script:
    - Upload file lên S3
    - Query DynamoDB
    - List EC2 Instances
  - Làm việc với temporary credentials qua IAM Role

- **Tích lũy kinh nghiệm thực tế với database quan hệ, NoSQL và container.**
