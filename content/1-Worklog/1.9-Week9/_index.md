---
title: "Week 9 Worklog"
date: 2025-11-03
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:
- Understand serverless architecture and event-driven compute.
- Build compute functions with AWS Lambda.
- Deploy REST APIs using API Gateway (HTTP/REST).
- Integrate Lambda with DynamoDB, S3, SNS, EventBridge.
- Learn IAM roles & permissions for serverless systems.

### Tasks:

| Day | Task                                 | Date | Completed | Ref |
| --- | ------------------------------------ | ------ | -------- | ---- |
| 41  | Learn AWS Lambda                     | 11/03  | 11/03    | https://cloudjourney.awsstudygroup.com/ |
| 42  | Build and Test Lambda Functions      | 11/04  | 11/04    | https://cloudjourney.awsstudygroup.com/ |
| 43  | Create REST API with API Gateway     | 11/05  | 11/05    | https://cloudjourney.awsstudygroup.com/ |
| 44  | Integrate Lambda with DB & S3        | 11/06  | 11/06    | https://cloudjourney.awsstudygroup.com/ |
| 45  | IAM Roles for Serverless             | 11/07  | 11/07    | https://cloudjourney.awsstudygroup.com/ |

### Week 9 Achievements:

- **Mastered AWS Lambda foundations**, such as:
  - Execution model (ephemeral compute)
  - Cold start vs warm start
  - Memory & timeout settings
  - Concurrency model
  - Layers & extensions

- **Built Lambda Functions**:
  - Created handlers in Node.js/Python
  - Logged events & context
  - Used test events
  - Returned API responses with correct JSON structure

- **Integrated Lambda with AWS Services**:
  - DynamoDB (PutItem, GetItem)
  - S3 (upload, read, delete)
  - SNS (notifications)
  - EventBridge (scheduled events / cron jobs)

- **Created REST API using API Gateway**:
  - Created API resources & methods
  - Connected API → Lambda integration
  - Configured CORS
  - Set request/response mappings
  - Deployed stages (dev, prod)
  - Tested using Postman + curl

- **Implemented IAM Roles for serverless**:
  - Execution role for Lambda
  - Inline vs managed AWSLambdaBasicExecutionRole
  - Principle of Least Privilege applied to Lambda IAM

- **Created end-to-end serverless workflow**, including:
  - API Gateway → Lambda → DynamoDB
  - S3 Upload → Lambda Trigger
  - CRON schedule → Lambda automation

- **CLI Experience**:
  - `aws lambda create-function`
  - `aws lambda invoke`
  - `aws apigateway get-rest-apis`

- **Gained production-level understanding of serverless systems and event-driven architecture.**
