---
title: "Worklog Tuần 4"
date: 2025-09-29
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu Tuần 4:
- Hiểu nền tảng và khái niệm lưu trữ của Amazon S3.
- Host website tĩnh bằng S3 Website Hosting.
- Tăng tốc phân phối nội dung bằng CloudFront CDN.
- Triển khai S3 Versioning và Lifecycle Management.
- Kích hoạt Cross-Region Replication (CRR) để đảm bảo tính bền vững.

### Công việc:

| Ngày | Công việc                                      | Ngày | Hoàn thành | Tham khảo |
| ---- | ---------------------------------------------- | ----- | ---------- | ---------- |
| 16   | Bắt đầu với Amazon S3                          | 09/29 | 09/29      | https://cloudjourney.awsstudygroup.com/ |
| 17   | Kích hoạt Static Website trên S3               | 09/30 | 09/30      | https://cloudjourney.awsstudygroup.com/ |
| 18   | Tăng tốc website tĩnh bằng CloudFront          | 10/01 | 10/01      | https://cloudjourney.awsstudygroup.com/ |
| 19   | Kích hoạt Versioning & Lifecycle Rules         | 10/02 | 10/02      | https://cloudjourney.awsstudygroup.com/ |
| 20   | Thiết lập Cross-Region Replication (CRR)       | 10/03 | 10/03      | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 4:

- **Nắm vững nền tảng Amazon S3**, gồm:
  - Buckets, Objects, Folders, Prefixes  
  - Mô hình lưu trữ “11 số 9” durability  
  - Storage Classes: Standard, IA, Glacier, Deep Archive  
  - Các khái niệm bảo mật:  
    - Bucket Policy  
    - ACL  
    - Block Public Access  
  - Nguồn lý thuyết: https://cloudjourney.awsstudygroup.com/

- **Tạo và cấu hình S3 Bucket**, gồm:
  - Quy tắc đặt tên bucket (global unique)
  - Chọn region phù hợp chi phí/độ trễ
  - Bật/tắt Public Access
  - Hiểu cấu trúc URL endpoint của S3 static website

- **Triển khai Static Website Hosting**, gồm:
  - Bật Static Hosting mode
  - Cấu hình `index.html` và `error.html`
  - Upload HTML/CSS/JS lên bucket
  - Viết Bucket Policy cho phép đọc public
  - Kiểm tra website bằng endpoint của S3

- **Tích hợp CloudFront cho website**, gồm:
  - Tạo CloudFront Distribution mới
  - Chọn S3 làm Origin
  - Tạo OAI để chặn truy cập trực tiếp S3
  - Cấu hình TTL, caching, invalidation
  - Quan sát sự phân phối toàn cầu của CDN

- **Bật Versioning**, cung cấp:
  - Theo dõi lịch sử đối tượng
  - Bảo vệ khi xóa nhầm
  - Lưu nhiều phiên bản object

- **Cấu hình Lifecycle Rules**, gồm:
  - Chuyển object sang IA/Glacier
  - Tự động xóa object cũ
  - Quản lý version dư thừa

- **Thiết lập Cross-Region Replication (CRR)**:
  - Tạo bucket ở region thứ hai
  - Bật versioning cho cả 2 bucket
  - Tạo IAM Role dành cho replication
  - Kiểm tra object tự động replicate

- **Thực hành CLI với S3**, gồm:
  - `aws s3 ls`
  - `aws s3 sync`
  - `aws s3 cp`
  - Xem bucket policy / versioning config

- **Nắm được cách triển khai – bảo mật – tối ưu – tự động hóa hệ thống lưu trữ bằng S3.**
