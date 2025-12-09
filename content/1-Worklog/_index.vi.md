# Giới thiệu Worklog

## Tổng quan
Bản Worklog này ghi lại toàn bộ hành trình học và thực hành AWS của tôi trong **12 tuần liên tiếp**. Mục tiêu là kết hợp **lý thuyết** từ khóa học (tham khảo: https://cloudjourney.awsstudygroup.com/) với **thực hành trực tiếp** trên tài khoản AWS (Free Tier khi có thể) để xây dựng năng lực triển khai, vận hành và tối ưu hệ thống cloud theo tiêu chuẩn production.

## Cách tôi hoàn thành
- **Phương pháp học:** cứ mỗi tuần tôi chọn một nhóm chủ đề (ví dụ: IAM & VPC, EC2 & LAMP, S3 & CloudFront, ...), đọc tài liệu tham khảo, sau đó thực hành trực tiếp trên AWS bằng cả **Console** và **AWS CLI**.  
- **Thực hành có cấu trúc:** mỗi tuần gồm một bảng task rõ ràng (Day / Task / Start / Completion / Ref) – hoàn thành task bằng cách thực hiện các bước cài đặt, cấu hình, kiểm thử và ghi chú kết quả.  
- **Ghi chép & báo cáo:** mọi thao tác, lệnh CLI, cấu hình quan trọng và kết quả kiểm thử được ghi lại trong Worklog tuần tương ứng để dễ tra cứu và lặp lại.  
- **Kiểm thử & tối ưu:** sau khi triển khai, tôi chạy các kiểm thử (kết nối, load test cơ bản, health check), theo dõi metrics bằng CloudWatch và điều chỉnh cấu hình (SG, sizing, lifecycle rules...) để tối ưu hiệu năng và chi phí.

## Thời gian hoàn thành
- **Tổng thời gian:** 12 tuần (tuần 1 bắt đầu 09/09/2025 theo Worklog).  
- **Tần suất:** mỗi tuần có các nhiệm vụ cụ thể (thường 5 ngày công việc/tuần theo bảng Tasks) — tổng hợp lý thuyết + thực hành, mỗi ngày hoàn thành 1–2 task tuỳ độ phức tạp.

## Nội dung đã thực hiện theo tuần (tóm tắt)
- **Tuần 1 — AWS Foundations:** tạo tài khoản Free Tier, thiết lập IAM cơ bản, cài Hugo, làm quen Console, cấu hình AWS Budgets và AWS CLI.  
- **Tuần 2 — IAM & VPC:** quản lý IAM (users/groups/roles/policies), xây dựng VPC (public/private subnet), cấu hình Security Groups & NACL, triển khai EC2 và khảo sát VPN site-to-site.  
- **Tuần 3 — EC2 nâng cao & LAMP/Node.js:** tìm hiểu instance types, EBS, AMI; cài LAMP stack; deploy Node.js; áp dụng IAM governance cho chi phí.  
- **Tuần 4 — S3 & CloudFront:** quản lý bucket, host static website, tích hợp CloudFront, bật versioning, lifecycle rules, và cross-region replication.  
- **Tuần 5 — RDS / Lightsail / DynamoDB / SDK:** triển khai RDS, thử Lightsail DB và Containers, học DynamoDB, viết script với AWS SDK.  
- **Tuần 6 — Thiết kế kiến trúc & Database:** nghiên cứu dịch vụ phù hợp, vẽ kiến trúc hệ thống, thiết kế ERD/schema, hoàn thiện tài liệu kỹ thuật.  
- **Tuần 7 — CloudWatch / SNS / SQS:** cấu hình logs, metrics, dashboards, alarms; tích hợp SNS cho alert; thiết kế workflows với SQS.  
- **Tuần 8 — Elastic Beanstalk & Auto Scaling:** deploy ứng dụng đa tầng bằng EB, cấu hình ALB và Auto Scaling, quản lý lifecycle (deploy/rollback).  
- **Tuần 9 — Serverless (Lambda & API Gateway):** viết Lambda, tạo REST API với API Gateway, tích hợp Lambda với S3/DynamoDB/SNS/EventBridge và quản lý IAM cho serverless.  
- **Tuần 10 — CI/CD (CodeCommit/CodeBuild/CodeDeploy/CodePipeline):** xây pipeline tự động từ code → build → deploy, viết `buildspec.yml` & `appspec.yml`, kiểm thử flow end-to-end.  
- **Tuần 11 — Containers (Docker, ECR, ECS, Fargate):** viết Dockerfile, push image lên ECR, deploy trên ECS (EC2 & Fargate), cấu hình networking và auto-scaling cho services.  
- **Tuần 12 — Final Deployment & Optimization:** triển khai toàn bộ dự án theo kiến trúc đã thiết kế, tích hợp monitoring & CI/CD, tối ưu chi phí/hiệu năng/bảo mật, kiểm thử tải, hoàn tất tài liệu dự án.

## Kết quả đạt được
- Có thể triển khai và vận hành một hệ thống ứng dụng cloud end-to-end trên AWS (compute, storage, database, networking, monitoring).  
- Nắm vững thao tác quản trị bằng **Console** và **AWS CLI**, biết kết hợp chúng để tự động hoá.  
- Xây được CI/CD pipeline cơ bản, triển khai serverless và containerized workloads.  
- Có bộ tài liệu kiến trúc, thiết kế cơ sở dữ liệu và hướng dẫn deploy reproducible cho dự án.

## Link tham khảo chính
- Tài liệu lý thuyết & hướng dẫn thực hành: https://cloudjourney.awsstudygroup.com/

