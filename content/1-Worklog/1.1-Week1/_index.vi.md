---
title: "Worklog Tuần 1"
date: 2025-09-09
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Mục tiêu Tuần 1:
- Xây dựng nền tảng kiến thức cơ bản về AWS Cloud.
- Tạo và cấu hình tài khoản AWS Free Tier.
- Thiết lập cấu hình bảo mật IAM cho tài khoản.
- Cài đặt và cấu hình Hugo để viết tài liệu.
- Làm quen và điều hướng AWS Management Console.
- Thiết lập AWS Budgets để theo dõi chi phí.
- Bắt đầu sử dụng AWS CLI cho các thao tác cơ bản.

### Công việc cần thực hiện trong tuần:

| Ngày | Công việc                                   | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| ---- | ------------------------------------------- | ------------- | ---------------- | -------------------- |
| 1    | Tạo tài khoản AWS đầu tiên                  | 09/09/2025    | 09/09/2025       | https://cloudjourney.awsstudygroup.com/ |
| 2    | Tạo Admin Group và Admin User               | 09/09/2025    | 09/09/2025       | https://cloudjourney.awsstudygroup.com/ |
| 3    | Cài đặt Hugo                                | 09/10/2025    | 09/10/2025       |  |
| 4    | Khám phá AWS Management Console             | 09/11/2025    | 09/11/2025       | https://cloudjourney.awsstudygroup.com/ |
| 5    | Tạo Budget bằng Template                    | 09/12/2025    | 09/12/2025       | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 1:

- **Hiểu các khái niệm cốt lõi của AWS Cloud**, bao gồm:
  - Hạ tầng toàn cầu (Regions, Availability Zones, Edge Locations)
  - Mô hình trách nhiệm chia sẻ của AWS (Shared Responsibility Model)
  - Các nhóm dịch vụ:  
    **Compute**, **Storage**, **Networking**, **Databases**, **Security**, **Developer Tools**, **Monitoring**
  - Kiến thức tham khảo từ:  
    ➝ https://cloudjourney.awsstudygroup.com/

- **Tạo và cấu hình thành công tài khoản AWS Free Tier**, bao gồm:
  - Xác minh email và thông tin thanh toán
  - Bật MFA cho tài khoản root
  - Áp dụng các biện pháp bảo mật cơ bản khuyến nghị

- **Thiết lập nền tảng IAM bảo mật**, bao gồm:
  - Tạo Admin Group với quyền AdministratorAccess
  - Tạo Admin User và gán vào nhóm
  - Đăng nhập bằng IAM User thay vì root
  - Thực hiện theo các best practice bảo mật của AWS

- **Làm quen với giao diện AWS Management Console**:
  - Hiểu cách nhóm các dịch vụ
  - Điều hướng dashboard, thanh tìm kiếm, menu tài nguyên
  - Truy cập các dịch vụ như EC2, S3, IAM, VPC

- **Cài đặt và cấu hình Hugo để viết tài liệu**:
  - Cài Hugo CLI
  - Tạo và khởi tạo cấu trúc site Hugo
  - Thêm file nội dung ban đầu và chạy thử bản build

- **Thiết lập AWS Budgets để theo dõi chi phí**:
  - Tạo cảnh báo chi phí Free Tier
  - Cấu hình thông báo qua email
  - Hiểu cách vận hành hệ thống billing của AWS

- **Cài đặt và cấu hình AWS CLI**, bao gồm:
  - Thiết lập Access Key + Secret Key
  - Chọn Region mặc định + Output format

- **Thực hiện các thao tác cơ bản bằng AWS CLI**, như:
  - `aws configure list`
  - `aws ec2 describe-regions`
  - `aws ec2 describe-instances`
  - `aws ec2 describe-key-pairs`
  - Kiểm tra danh tính bằng `sts get-caller-identity`

- **Nắm được khả năng thao tác AWS song song bằng Console và CLI.**
