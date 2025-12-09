---
title: "Worklog Tuần 9"
date: 2025-11-03
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu Tuần 9:
- Hiểu kiến trúc serverless và mô hình event-driven.
- Xây dựng compute functions bằng AWS Lambda.
- Deploy REST API bằng API Gateway (HTTP/REST).
- Tích hợp Lambda với DynamoDB, S3, SNS, EventBridge.
- Học IAM roles & permissions cho serverless.

### Công việc:

| Ngày | Công việc                           | Ngày  | Hoàn thành | Tham khảo |
| ---- | ----------------------------------- | ------ | ---------- | ---------- |
| 41   | Học AWS Lambda                      | 11/03  | 11/03      | https://cloudjourney.awsstudygroup.com/ |
| 42   | Xây dựng & test Lambda Functions    | 11/04  | 11/04      | https://cloudjourney.awsstudygroup.com/ |
| 43   | Tạo REST API bằng API Gateway       | 11/05  | 11/05      | https://cloudjourney.awsstudygroup.com/ |
| 44   | Tích hợp Lambda với DB & S3         | 11/06  | 11/06      | https://cloudjourney.awsstudygroup.com/ |
| 45   | IAM Roles cho hệ serverless         | 11/07  | 11/07      | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 9:

- **Nắm vững nền tảng AWS Lambda**, gồm:
  - Mô hình thực thi (ephemeral runtime)
  - Cold start vs warm start
  - Memory/Timeout
  - Concurrency  
  - Lambda Layers & Extensions

- **Xây dựng Lambda Function**, gồm:
  - Handler Node.js/Python
  - Log event và context
  - Tạo test event
  - Trả JSON đúng chuẩn

- **Tích hợp Lambda với AWS Services**, gồm:
  - DynamoDB (PutItem / GetItem)
  - S3 (upload / read / delete)
  - SNS (notify)
  - EventBridge (cron jobs)

- **Tạo REST API bằng API Gateway**, gồm:
  - Resources & methods
  - Kết nối API → Lambda
  - Cấu hình CORS
  - Mapping request/response
  - Deploy stage dev/prod
  - Test bằng Postman + curl

- **IAM Role cho serverless**, gồm:
  - Execution role
  - AWSLambdaBasicExecutionRole
  - Least Privilege

- **Tạo workflow serverless hoàn chỉnh**, gồm:
  - API Gateway → Lambda → DynamoDB
  - S3 Upload → Lambda Trigger
  - CRON → Lambda Scheduler

- **Kỹ năng CLI**, gồm:
  - `aws lambda create-function`
  - `aws lambda invoke`
  - `aws apigateway get-rest-apis`

- **Đạt hiểu biết mức production về kiến trúc serverless.**
