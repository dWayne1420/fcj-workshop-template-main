---
title: "Worklog Tuần 10"
date: 2025-11-10
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu Tuần 10:
- Học hệ thống DevOps trên AWS cho tự động hóa CI/CD.
- Tạo repository bằng CodeCommit.
- Build ứng dụng bằng CodeBuild.
- Deploy tự động bằng CodeDeploy.
- Xây dựng CI/CD Pipeline với CodePipeline.

### Công việc:

| Ngày | Công việc                    | Ngày  | Hoàn thành | Tham khảo |
| ---- | ---------------------------- | ------ | ---------- | ---------- |
| 46   | Tìm hiểu AWS DevOps Tools    | 11/10  | 11/10      | https://cloudjourney.awsstudygroup.com/ |
| 47   | Tạo repo CodeCommit          | 11/11  | 11/11      | https://cloudjourney.awsstudygroup.com/ |
| 48   | Build app bằng CodeBuild     | 11/12  | 11/12      | https://cloudjourney.awsstudygroup.com/ |
| 49   | Deploy qua CodeDeploy        | 11/13  | 11/13      | https://cloudjourney.awsstudygroup.com/ |
| 50   | Tạo CI/CD Pipeline hoàn chỉnh| 11/14  | 11/14      | https://cloudjourney.awsstudygroup.com/ |

### Thành tựu Tuần 10:

- **Hiểu hệ sinh thái AWS DevOps**, gồm:
  - CodeCommit (Git)
  - CodeBuild (tự động build)
  - CodeDeploy (triển khai ứng dụng)
  - CodePipeline (orchestration CI/CD)
  - Artifact S3
  - IAM cho DevOps pipeline

- **Tạo repo CodeCommit**, gồm:
  - Git credentials IAM
  - Clone/push source code
  - Version control

- **Cấu hình CodeBuild**, gồm:
  - File `buildspec.yml`
  - Cài dependency
  - Unit test chạy trong pipeline
  - Artifact lên S3
  - Theo dõi build logs

- **Triển khai ứng dụng bằng CodeDeploy**, gồm:
  - Deployment groups
  - `appspec.yml`
  - Lifecycle hooks trên EC2
  - Auto rollback khi fail

- **Tạo CI/CD Pipeline đầy đủ**, gồm:
  - CodeCommit → CodeBuild → CodeDeploy → EC2
  - Trigger khi push Git
  - Auto deploy mỗi commit
  - Stage approval cho production

- **Kiểm thử pipeline end-to-end**, gồm:
  - Commit code
  - Build tự động
  - Deploy tự động
  - Theo dõi log build/deploy

- **Đạt kỹ năng DevOps thực chiến trên AWS.**
