---
title: "Week 5 Worklog"
date: 2025-10-06
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:
- Understand relational databases on AWS using Amazon RDS.
- Deploy a managed database instance on AWS Lightsail.
- Learn container-based deployment with Lightsail Containers.
- Explore NoSQL concepts through DynamoDB.
- Begin interacting with AWS programmatically via SDK.

### Tasks:

| Day | Task                                     | Date | Completed | Ref |
| --- | ---------------------------------------- | ------ | -------- | ---- |
| 21  | Learn Amazon RDS                         | 10/06  | 10/06    | https://cloudjourney.awsstudygroup.com/ |
| 22  | Deploy a Database on Lightsail           | 10/07  | 10/07    | https://cloudjourney.awsstudygroup.com/ |
| 23  | Deploy a Containers on Lightsail         | 10/08  | 10/08    | https://cloudjourney.awsstudygroup.com/ |
| 24  | Work with Amazon DynamoDB                | 10/09  | 10/09    | https://cloudjourney.awsstudygroup.com/ |
| 25  | Begin with AWS SDK                       | 10/10  | 10/10    | https://cloudjourney.awsstudygroup.com/ |

### Week 5 Achievements:

- **Learned foundational concepts of Amazon RDS**, including:
  - Database Engines (MySQL, PostgreSQL, MariaDB)
  - Reserved instances, Multi-AZ, Read Replicas
  - Automated backups, snapshots, maintenance windows
  - Parameter groups & security groups
  - Private vs Public RDS endpoints

- **Created an Amazon RDS instance**, including:
  - Selected DB engine version
  - Chose instance class & allocated storage
  - Configured security:
    - Public accessibility
    - SG allowing DB port 3306
  - Created initial DB & tested connection via MySQL Workbench

- **Deployed a Lightsail Managed Database**, including:
  - Compared with RDS features
  - Set up static private IP
  - Interconnected app ↔ Lightsail DB
  - Configured automatic backups + failover options

- **Deployed an Application Using Lightsail Containers**:
  - Built container image
  - Pushed to Lightsail Container Registry
  - Created deployment + scale settings
  - Configured environment variables

- **Learned Amazon DynamoDB**, including:
  - Partition key, sort key
  - Provisioned vs On-Demand capacity
  - DynamoDB Streams
  - Global & Local Secondary Indexes
  - Best practices for NoSQL data modeling

- **Performed DynamoDB operations**, including:
  - Created table
  - Inserted items
  - Query & Scan operations via Console + CLI

- **Started working with AWS SDK**, including:
  - Installed AWS SDK for JavaScript / Python
  - Wrote scripts to:
    - Upload files to S3
    - Query DynamoDB
    - List EC2 instances
  - Used temporary security credentials via IAM Roles

- **Gained practical experience in relational, NoSQL, and containerized application hosting.**
