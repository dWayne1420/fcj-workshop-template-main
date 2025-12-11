---
title: "Week 3 Worklog"
date: 2025-09-22
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:
- Explore advanced Amazon EC2 operations.
- Install and configure LAMP stack on EC2.
- Deploy Node.js application on EC2.
- Implement IAM governance for cost control.
- Learn how applications access AWS services securely.

### Tasks:

| Day | Task                                   | Start | End | Ref |
| --- | -------------------------------------- | ----- | --- | ----|
| 11  | Explore EC2 advanced features          | 09/22 | 09/22 | https://cloudjourney.awsstudygroup.com/ |
| 12  | Install LAMP Web Server                | 09/23 | 09/23 | https://cloudjourney.awsstudygroup.com/ |
| 13  | Deploy Node.js Applications            | 09/24 | 09/24 | https://cloudjourney.awsstudygroup.com/ |
| 14  | Implement Cost Governance using IAM    | 09/25 | 09/25 | https://cloudjourney.awsstudygroup.com/ |
| 15  | Application Access to AWS Services     | 09/26 | 09/26 | https://cloudjourney.awsstudygroup.com/ |

### Week 3 Achievements:

- **Explored EC2 deeply**, including:
  - Instance families (General, Compute, Memory optimized)
  - Instance lifecycle & states
  - EBS volumes (gp3, io2, throughput settings)
  - ENI, public/private IP, Elastic IP
  - Security Groups & Network Integration
  - AMIs & Snapshots
  - User Data automation scripts

- **Installed full LAMP stack (Linux + Apache + MySQL + PHP)**:
  - Installed Apache web server
  - Configured Virtual Hosts
  - Installed PHP & essential extensions
  - Connected Apache + PHP
  - Installed & configured MySQL
  - Deployed test PHP website
  - Secured MySQL root account

- **Deployed Node.js application**, including:
  - Installed Node.js + NPM
  - Installed PM2 process manager
  - Created systemd startup for PM2
  - Configured firewall + Security Groups
  - Reverse proxy using NGINX
  - Deployed and tested Node.js app

- **Implemented IAM cost governance**:
  - Read-only billing roles
  - Budget alerts
  - Cost explorer permissions
  - IAM policies to restrict expensive resources

- **Learned secure application access to AWS**:
  - IAM Roles for EC2
  - Instance metadata v2 (IMDSv2)
  - Accessing S3 programmatically
  - Using AWS SDK with temporary credentials

- **CLI operations practiced**:
  - `describe-instances`
  - Starting/stopping EC2
  - Creating EBS snapshots
  - Viewing CPU metrics via CloudWatch CLI

- **Acquired ability to deploy full-stack apps using EC2, LAMP, Node.js.**
