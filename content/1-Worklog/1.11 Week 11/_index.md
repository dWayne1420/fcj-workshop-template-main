---
title: "Week 11 Worklog"
date: 2025-11-17
weight: 1
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:
- Learn Docker containerization fundamentals.
- Push images to Amazon ECR.
- Deploy services on Amazon ECS (EC2/Fargate).
- Configure ECS Networking and Auto Scaling.
- Understand container orchestration workflows.

### Tasks:

| Day | Task                          | Date | Completed | Ref |
| --- | ----------------------------- | ------ | -------- | ---- |
| 51  | Learn Docker Basics           | 11/17  | 11/17    | https://cloudjourney.awsstudygroup.com/ |
| 52  | Create ECR Repository         | 11/18  | 11/18    | https://cloudjourney.awsstudygroup.com/ |
| 53  | Build & Push Images to ECR    | 11/19  | 11/19    | https://cloudjourney.awsstudygroup.com/ |
| 54  | Deploy on ECS (EC2/Fargate)   | 11/20  | 11/20    | https://cloudjourney.awsstudygroup.com/ |
| 55  | ECS Networking & Auto Scaling | 11/21  | 11/21    | https://cloudjourney.awsstudygroup.com/ |

### Week 11 Achievements:

- **Learned Docker core concepts**, including:
  - Images vs Containers
  - Dockerfile instructions (FROM, RUN, CMD, EXPOSE…)
  - Multi-stage builds
  - Tagging & versioning images
  - Container networking

- **Built Docker Images**:
  - Created Dockerfile for Node.js app
  - Optimized layers to reduce image size
  - Used `.dockerignore`
  - Tested containers locally

- **Created Amazon ECR Repository**, including:
  - Private registry configuration
  - Authenticated via AWS CLI
  - Tagging & pushing images to ECR

- **Deployed applications using ECS**, including:
  - Created Task Definitions
  - Configured CPU, memory, environment variables
  - Created ECS Service
  - Integrated ALB for service routing
  - Set desired count for replicas

- **Used AWS Fargate for serverless containers**, achieving:
  - No need for EC2 hosts
  - Fully managed compute
  - Scaling based on CPU/memory thresholds

- **Configured ECS Networking**, including:
  - VPC subnets selection
  - Public/Private subnet deployment
  - Security Group for tasks
  - IAM Role for ECS Tasks

- **Tested Auto Scaling with ECS**, including:
  - CPU-based scaling out/in
  - Minimum & maximum task count
  - Load test to trigger new tasks

- **Gained ability to deploy containerized applications on AWS using ECS + ECR + Fargate.**
