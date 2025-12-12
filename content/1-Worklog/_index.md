---
title: "Worklog"
date: "2025-12-07"
weight: 1
chapter: false
pre: " <b> 1. </b> "
---

# Worklog Introduction

## Overview
This Worklog records my entire 12-week journey of learning and practicing AWS.  
The goal was to combine **theoretical knowledge** from the course materials  
(reference: https://cloudjourney.awsstudygroup.com/) with **hands-on practice**  
directly on the AWS platform (using Free Tier whenever possible) to build the  
skills required to deploy, operate, and optimize cloud systems at a  
production-ready level.

## How I Completed It
- **Learning approach:** each week I focused on a specific group of topics  
  (e.g., IAM & VPC, EC2 & LAMP, S3 & CloudFront, ...), studied the reference  
  materials, and practiced directly on AWS using both the **Console** and  
  **AWS CLI**.  
- **Structured practice:** every week contained a clear task table  
  (Day / Task / Start / Completion / Ref), and each task was completed through  
  steps involving setup, configuration, testing, and logging results.  
- **Documentation & reporting:** all operations, CLI commands, configurations,  
  and test results were recorded in the weekly Worklog to ensure reproducibility  
  and easy review.  
- **Testing & optimization:** after deploying resources, I performed tests  
  (connectivity, basic load tests, health checks), monitored metrics via  
  CloudWatch, and tuned configurations (SG rules, sizing, lifecycle rules, etc.)  
  to improve performance and cost efficiency.

## Timeframe
- **Total duration:** 12 weeks (starting from 09/09/2025 according to Week 1).  
- **Weekly workload:** each week contained structured tasks (usually 5 tasks per  
  week) — combining theory and practice, typically completing 1–2 tasks per day  
  depending on complexity.

## Weekly Summary
- [**Week 1 — AWS Foundations:**](/content/1-Worklog/1.1-Week1/) Created Free Tier account, built IAM baseline,  
  installed Hugo, explored Console, configured AWS Budgets and AWS CLI.  
- [**Week 2 — IAM & VPC:**](/content/1-Worklog/1.2-Week2/) Managed IAM (users/groups/roles/policies), built VPC  
  (public/private subnets), configured SGs & NACLs, deployed EC2, studied  
  site-to-site VPN.  
- [**Week 3 — EC2 Advanced & LAMP/Node.js:**](/content/1-Worklog/1.3-Week3/) Explored EC2 internals, installed  
  LAMP stack, deployed Node.js apps, implemented IAM cost governance.  
- [**Week 4 — S3 & CloudFront:**](/content/1-Worklog/1.4-Week4/) Managed S3 buckets, hosted static website,  
  integrated CloudFront, enabled versioning, lifecycle rules, CRR.  
- [**Week 5 — RDS / Lightsail / DynamoDB / SDK:**](/content/1-Worklog/1.5-Week5/) Deployed RDS, Lightsail  
  database, Lightsail containers, learned DynamoDB, wrote scripts using AWS SDK.  
- [**Week 6 — Architecture & Database Design:**](/content/1-Worklog/1.6-Week6/) Researched AWS services, designed  
  full architecture, created ERD/schema, completed technical documentation.  
- [**Week 7 — CloudWatch / SNS / SQS:**](/content/1-Worklog/1.7-Week7/) Configured logs, metrics, dashboards,  
  alarms; integrated SNS; built SQS workflows.  
- [**Week 8 — Elastic Beanstalk & Auto Scaling:**](/content/1-Worklog/1.8-Week8/) Deployed multi-tier app on EB,  
  configured ALB, Auto Scaling, deployment lifecycle.  
- [**Week 9 — Serverless (Lambda & API Gateway):**](/content/1-Worklog/1.9-Week9/) Built Lambda functions,  
  created REST APIs, integrated with S3/DynamoDB/SNS/EventBridge, configured IAM  
  for serverless.  
- [**Week 10 — CI/CD (CodeCommit/CodeBuild/CodeDeploy/CodePipeline):**](/content/1-Worklog/1.10-Week10/) Built full  
  CI/CD pipeline, wrote `buildspec.yml` and `appspec.yml`, tested end-to-end flow.  
- [**Week 11 — Containers (Docker, ECR, ECS, Fargate):**](/content/1-Worklog/1.11-Week11/) Created Docker images,  
  pushed to ECR, deployed via ECS EC2/Fargate, configured networking &  
  auto-scaling.  
- [**Week 12 — Final Deployment & Optimization:**](/content/1-Worklog/1.12-Week12/) Deployed final project,  
  integrated monitoring and CI/CD, optimized performance/cost/security,  
  performed load tests, completed full documentation.

## Outcomes Achieved
- Ability to deploy and operate an end-to-end cloud application system on AWS  
  (compute, storage, database, networking, monitoring).  
- Proficiency in managing AWS using **both Console and CLI**, and combining them  
  for automation.  
- Built complete CI/CD pipelines; deployed serverless and containerized  
  workloads.  
- Produced a full set of architecture documents, database designs, and  
  deployment guidelines suitable for reproducing and scaling the project.

## Main Reference
- Theoretical resources & hands-on guides: https://cloudjourney.awsstudygroup.com/
