---
title: "Week 6 Worklog"
date: 2025-10-13
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:
- Research and evaluate AWS services for final project architecture.
- Design complete system architecture diagram with AWS services.
- Build detailed database schema for application.
- Document architecture decisions and deployment strategy.
- Track learning journey and workshop participation.

### Tasks:

| Day | Task                                    | Date | Completed | Ref |
| --- | --------------------------------------- | ------ | -------- | ---- |
| 26  | Research project services               | 10/13  | 10/13    | https://cloudjourney.awsstudygroup.com/ |
| 27  | Draw architecture diagram               | 10/14  | 10/14    | https://cloudjourney.awsstudygroup.com/ |
| 28  | Design database schema                  | 10/15  | 10/15    | https://cloudjourney.awsstudygroup.com/ |
| 29  | Fix diagram and write documentation     | 10/16  | 10/16    | https://cloudjourney.awsstudygroup.com/ |
| 30  | Write Events Participated               | 10/17  | 10/17    | https://cloudjourney.awsstudygroup.com/ |

### Week 6 Achievements:

- **Completed detailed research on AWS services**, including:
  - Compute options: EC2, Lambda, Lightsail, Fargate
  - Storage: S3, EFS, RDS, DynamoDB
  - Networking: VPC, CloudFront, API Gateway, Route 53
  - Monitoring & DevOps tools
  - Compared cost, complexity, and performance of each option

- **Designed full AWS architecture diagram**:
  - VPC design with public/private subnets
  - Internet Gateway + NAT Gateway routing
  - EC2 or Lambda compute flows
  - RDS/DynamoDB data layer
  - CloudFront as CDN
  - S3 for static content or file storage
  - IAM roles for permissions
  - CloudWatch for monitoring
  - Used AWS Icons (official architecture set)

- **Created database design**, including:
  - Entity–Relationship Diagram (ERD)
  - Table structures
  - Primary & foreign keys
  - Normalization vs Optimization decisions
  - Indexing strategy
  - Schema migration plan

- **Wrote technical documentation to support architecture**, such as:
  - High-level overview
  - Component description
  - Data flow diagrams
  - API design
  - Deployment plan
  - IAM role assignments
  - Monitoring & logging plan

- **Refined diagrams based on design feedback**, improving:
  - Security posture (restrict SG rules)
  - Cost (replace NAT Gateway with NAT Instance when appropriate)
  - Performance (move static content to CloudFront)

- **Finished Events Participated section**, documenting:
  - All FCJ sessions attended
  - Lessons learned
  - Community participation activities

- **Achieved ability to plan, design, and document production-ready AWS architectures.**
