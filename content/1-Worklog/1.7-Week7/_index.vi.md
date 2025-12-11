---
title: "Worklog Tuần 7"
date: 2025-10-20
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu Tuần 7:
- Học hệ thống giám sát AWS CloudWatch.
- Cấu hình CloudWatch Logs, Metrics và Dashboards.
- Thiết lập CloudWatch Alarms với thông báo SNS.
- Hiểu mô hình hàng đợi SQS và xử lý message.
- Tích hợp logging & monitoring vào ứng dụng.

### Công việc:

| Ngày | Công việc                              | Ngày  | Hoàn thành | Tham khảo |
| ---- | -------------------------------------- | ------ | ---------- | ---------- |
| 31   | Tìm hiểu CloudWatch Monitoring         | 10/20  | 10/20      | https://cloudjourney.awsstudygroup.com/ |
| 32   | Thiết lập CloudWatch Logs & Metrics    | 10/21  | 10/21      | https://cloudjourney.awsstudygroup.com/ |
| 33   | Cấu hình SNS Notifications             | 10/22  | 10/22      | https://cloudjourney.awsstudygroup.com/ |
| 34   | Học Amazon SQS Queues                  | 10/23  | 10/23      | https://cloudjourney.awsstudygroup.com/ |
| 35   | Tích hợp Monitoring vào ứng dụng       | 10/24  | 10/24      | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 7:

- **Nắm vững nền tảng AWS CloudWatch**, gồm:
  - Metrics (hệ thống, metrics của AWS services, custom metrics)
  - Log Groups & Log Streams
  - Cài CloudWatch Agent
  - Tích hợp EC2, Lambda, API Gateway
  - Tạo Dashboard và biểu đồ trực quan
  - Kiến thức tham khảo: https://cloudjourney.awsstudygroup.com/

- **Cấu hình CloudWatch Logs**, gồm:
  - Cài đặt CloudWatch Agent trên EC2
  - Cấu hình file `amazon-cloudwatch-agent.json`
  - Gửi log NGINX/Apache lên Log Group
  - Kiểm tra ingest log & timestamp

- **Làm việc với CloudWatch Metrics**, gồm:
  - CPUUtilization  
  - NetworkIn / NetworkOut  
  - DiskReadOps / DiskWriteOps  
  - Custom metrics tạo từ ứng dụng

- **Tạo CloudWatch Alarms**, ví dụ:
  - CPU > 70% trong 5 phút → gửi SNS
  - StatusCheckFailed > 0 → gửi email
  - Billing Alarm theo ngưỡng USD

- **Cấu hình SNS Topics**, gồm:
  - Tạo SNS Topic
  - Đăng ký email và verify subscription
  - Kết nối Alarm → SNS → Email
  - Kiểm tra trigger bằng cách tạo tải cao

- **Học hệ thống hàng đợi Amazon SQS**, gồm:
  - Hai loại queue: **Standard** và **FIFO**
  - Visibility Timeout
  - Dead-Letter Queue (DLQ)
  - Long polling vs Short polling
  - Use case: microservices, tách rời ứng dụng

- **Thực hành SQS**, gồm:
  - Tạo queue
  - Gửi/nhận message bằng Console & CLI
  - Xử lý message dạng batch
  - Purge queue

- **Tích hợp log ứng dụng vào CloudWatch**, đạt được:
  - Xem log real-time
  - Tạo metric từ log
  - Tạo pipeline cảnh báo hoàn chỉnh

- **Nắm năng lực giám sát – cảnh báo – tách rời ứng dụng bằng CloudWatch + SNS + SQS.**
