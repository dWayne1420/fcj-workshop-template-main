---
title: "Week 7 Worklog"
date: 2025-10-20
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:
- Learn AWS CloudWatch monitoring system.
- Configure CloudWatch Logs, Metrics, and Dashboards.
- Set up CloudWatch Alarms with SNS notifications.
- Understand SQS queue models and message processing.
- Integrate application logging and monitoring workflows.

### Tasks:

| Day | Task                                 | Date | Completed | Ref |
| --- | ------------------------------------ | ------ | -------- | ---- |
| 31  | Learn CloudWatch Monitoring           | 10/20  | 10/20    | https://cloudjourney.awsstudygroup.com/ |
| 32  | Set up CloudWatch Logs & Metrics      | 10/21  | 10/21    | https://cloudjourney.awsstudygroup.com/ |
| 33  | Configure SNS Notifications           | 10/22  | 10/22    | https://cloudjourney.awsstudygroup.com/ |
| 34  | Learn SQS Queues                      | 10/23  | 10/23    | https://cloudjourney.awsstudygroup.com/ |
| 35  | Integrate Monitoring with Application | 10/24  | 10/24    | https://cloudjourney.awsstudygroup.com/ |

### Week 7 Achievements:

- **Mastered AWS CloudWatch fundamentals**, including:
  - Metrics (system, AWS service metrics, custom metrics)
  - Log Groups & Log Streams
  - CloudWatch Agent installation
  - EC2, Lambda, and API Gateway integrations
  - Dashboard creation & visualization
  - Knowledge source: https://cloudjourney.awsstudygroup.com/

- **Configured CloudWatch Logs**, including:
  - Installed CloudWatch Agent on EC2
  - Configured `amazon-cloudwatch-agent.json`
  - Pushed NGINX/Apache logs to Log Groups
  - Verified log ingestion & timestamps

- **Worked with CloudWatch Metrics**, such as:
  - CPUUtilization
  - NetworkIn / NetworkOut
  - DiskReadOps / DiskWriteOps
  - Custom app metrics (via CLI)

- **Created CloudWatch Alarms**, including:
  - CPU > 70% for 5 minutes → SNS notification
  - StatusCheckFailed > 0 → Email alert
  - Billing Alarm using USD threshold

- **Configured SNS Topics for alerts**:
  - Created Topic
  - Subscribed email + verified endpoint
  - Linked Alarm → SNS → Email pipeline
  - Tested alarm triggers with scaled load

- **Learned Amazon SQS message queueing system**, including:
  - Queue types: **Standard** vs **FIFO**
  - Visibility Timeout
  - Dead-Letter Queue (DLQ)
  - Long polling vs short polling
  - Use cases: microservices, decoupling applications

- **Developed SQS workflows**, including:
  - Created queues
  - Sent/received messages via Console + CLI
  - Batch message processing
  - Purging queues

- **Integrated application logs with CloudWatch**, gaining:
  - Real-time log viewing
  - Metrics extraction from logs
  - Monitoring alert flow

- **Gained ability to monitor, alert, and decouple applications using CloudWatch + SNS + SQS.**
