---
title: "Week 8 Worklog"
date: 2025-10-27
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:
- Understand Elastic Beanstalk architecture and components.
- Deploy multi-tier applications using EB.
- Learn Load Balancers & environment tiers.
- Configure Auto Scaling groups and scaling triggers.
- Manage application lifecycle on EB.

### Tasks:

| Day | Task                               | Date | Completed | Ref |
| --- | ---------------------------------- | ------ | -------- | ---- |
| 36  | Introduction to Elastic Beanstalk  | 10/27  | 10/27    | https://cloudjourney.awsstudygroup.com/ |
| 37  | Deploy App to EB                   | 10/28  | 10/28    | https://cloudjourney.awsstudygroup.com/ |
| 38  | Configure Load Balancer            | 10/29  | 10/29    | https://cloudjourney.awsstudygroup.com/ |
| 39  | Configure Auto Scaling Policies    | 10/30  | 10/30    | https://cloudjourney.awsstudygroup.com/ |
| 40  | Update & Redeploy Application      | 10/31  | 10/31    | https://cloudjourney.awsstudygroup.com/ |

### Week 8 Achievements:

- **Learned Elastic Beanstalk core concepts**, including:
  - EB Environments (Web Server vs Worker)
  - EB Platform versions (Node.js, Python, PHP...)
  - EC2 Auto Scaling Groups & Load Balancers provisioned automatically
  - Deployment strategies (Rolling, Immutable, Blue/Green)

- **Deployed a Full Application on Elastic Beanstalk**:
  - Created EB application & environment
  - Uploaded initial version via ZIP
  - EB automatically provisioned:
    - EC2 instance
    - Security Groups
    - Auto Scaling Group
    - Load Balancer
  - Verified environment health + logs

- **Configured Application Load Balancer (ALB)**:
  - Path-based routing
  - Health checks configuration
  - Listener rules
  - Sticky sessions off/on testing

- **Implemented Auto Scaling Policies**:
  - Target Tracking (CPU > 50%)
  - Step Scaling (CPU > 70% add instance)
  - Set min/max instance range
  - Simulated load test to trigger scaling

- **Performed EB lifecycle tasks**:
  - Deployed new application versions
  - Performed environment updates & rollbacks
  - Used `.ebextensions` to customize configuration
  - Viewed logs from EB console (tail logs, bundle logs)

- **CLI Experience**:
  - Installed EB CLI
  - `eb init`, `eb create`, `eb deploy`, `eb status`
  - Version control of EB application builds

- **Achieved ability to deploy and auto-scale production workloads using Elastic Beanstalk.**
