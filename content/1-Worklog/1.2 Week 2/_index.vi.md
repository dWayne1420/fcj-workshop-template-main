---
title: "Worklog Tuần 2"
date: 2025-09-15
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu Tuần 2:
- Thành thạo quản lý truy cập IAM, policies và identity.
- Xây dựng nền tảng VPC cho môi trường Public/Private.
- Hiểu và áp dụng firewall mạng (Security Group + NACL).
- Triển khai EC2 trong VPC tùy chỉnh.
- Thiết lập kết nối hybrid network bằng VPN.

### Công việc:

| Ngày | Công việc                                | Bắt đầu | Hoàn thành | Tham khảo |
| ---- | ---------------------------------------- | -------- | ----------- | ---------- |
| 6    | IAM Access Control                       | 09/15    | 09/15       | https://cloudjourney.awsstudygroup.com/ |
| 7    | Học và xây dựng Amazon VPC               | 09/16    | 09/16       | https://cloudjourney.awsstudygroup.com/ |
| 8    | Firewall VPC (SG + NACL)                 | 09/17    | 09/17       | https://cloudjourney.awsstudygroup.com/ |
| 9    | Deploy EC2 trong custom VPC              | 09/18    | 09/18       | https://cloudjourney.awsstudygroup.com/ |
| 10   | Thiết lập Site-to-Site VPN               | 09/19    | 09/19       | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 2:

- **Nắm vững truy cập IAM**, bao gồm:
  - Users, Groups, Roles, Policies
  - Inline Policy vs Managed Policy
  - Permission Boundary
  - Nguyên tắc Least Privilege
  - Best practice từ: https://cloudjourney.awsstudygroup.com/

- **Thực hành tạo và kiểm tra policy**, bao gồm:
  - Tạo IAM Policy JSON tùy chỉnh
  - Gán và gỡ policy
  - Kiểm tra rủi ro permission bằng IAM Access Analyzer

- **Xây dựng một Amazon VPC hoàn chỉnh từ đầu**, bao gồm:
  - CIDR Block (10.0.0.0/16)
  - Public Subnet + Private Subnet
  - Internet Gateway (IGW)
  - NAT Gateway
  - Route Tables
  - Gán subnet đúng route table

- **Cấu hình Firewall mạng**, gồm:
  - **Security Group (SG)**:
    - Cho phép HTTP/HTTPS/SSH
    - Kiểm soát ở cấp độ instance
  - **Network ACL (NACL)**:
    - Quy tắc stateless
    - Tạo inbound/outbound rule tùy chỉnh

- **Triển khai EC2 trong VPC tùy chỉnh**:
  - Chạy EC2 trong Public Subnet
  - Gán SG + Key Pair
  - SSH thành công
  - Cài NGINX để kiểm tra kết nối
  - Kiểm tra định tuyến và NAT

- **Hiểu cách thiết lập VPN**, bao gồm:
  - Customer Gateway (CGW)
  - Virtual Private Gateway (VGW)
  - Đường hầm VPN IPSec
  - Cách hoạt động của VPN routing

- **Thực hành CLI VPC**, ví dụ:
  - `describe-vpcs`
  - `describe-security-groups`
  - `describe-route-tables`
  - `describe-subnets`

- **Xây nền tảng mạng vững chắc cho các tuần tiếp theo.**
