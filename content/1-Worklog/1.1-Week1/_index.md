---
title: "Week 1 Worklog"
date: 2025-09-09
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Week 1 Objectives:
- Build foundational understanding of AWS Cloud concepts.
- Create and configure an AWS Free Tier account.
- Establish IAM security baseline for account access.
- Install and configure Hugo for documentation.
- Learn and navigate the AWS Management Console.
- Set up AWS Budgets for cost monitoring.
- Begin using AWS CLI for basic operations.

### Tasks to be carried out this week:

| Day | Task                                         | Start Date | Completion Date | Reference Material |
| --- | -------------------------------------------- | ---------- | --------------- | ------------------ |
| 1   | Creating my first AWS account                | 09/09/2025 | 09/09/2025      | https://cloudjourney.awsstudygroup.com/ |
| 2   | Create Admin Group and Admin User            | 09/09/2025 | 09/09/2025      | https://cloudjourney.awsstudygroup.com/ |
| 3   | Setting Hugo                                 | 09/10/2025 | 09/10/2025      |  |
| 4   | Explore AWS Management Console               | 09/11/2025 | 09/11/2025      | https://cloudjourney.awsstudygroup.com/ |
| 5   | Create Budget by Template                    | 09/12/2025 | 09/12/2025      | https://cloudjourney.awsstudygroup.com/ |

### Week 1 Achievements:

- **Understood core AWS Cloud concepts**, including:
  - Global Infrastructure (Regions, AZs, Edge Locations)
  - AWS Shared Responsibility Model
  - Service categories:  
    **Compute**, **Storage**, **Networking**, **Databases**, **Security**, **Developer Tools**, **Monitoring**
  - Practical understanding sourced from  
    ➝ https://cloudjourney.awsstudygroup.com/

- **Successfully created and configured an AWS Free Tier account**, including:
  - Email + billing verification
  - MFA setup for root account
  - Initial security best practices for new accounts

- **Built a secure IAM foundation**, including:
  - Created Admin Group (AdministratorAccess)
  - Created Admin User and assigned permissions
  - Logged in using IAM user instead of root
  - Secured the account following AWS-recommended guidelines

- **Mastered basic AWS Management Console operations**:
  - Learned how services are grouped
  - Navigated dashboards, search bar, and resource menus
  - Found and opened services such as EC2, S3, IAM, VPC

- **Installed and configured Hugo for documentation**:
  - Installed Hugo CLI
  - Created and initialized Hugo site folder structure
  - Added initial content and tested local build

- **Set up AWS Budgets for cost monitoring**:
  - Created Free Tier cost alerts
  - Configured email notifications
  - Understood core concepts of AWS billing

- **Installed and configured AWS CLI**, including:
  - Added Access Key + Secret Key
  - Configured default region + output format

- **Performed essential AWS CLI operations**, such as:
  - `aws configure list`
  - `aws ec2 describe-regions`
  - `aws ec2 describe-instances`
  - `aws ec2 describe-key-pairs`
  - Checked identity via `sts get-caller-identity`

- **Gained the ability to work with AWS via both Console and CLI**, managing services in parallel.
