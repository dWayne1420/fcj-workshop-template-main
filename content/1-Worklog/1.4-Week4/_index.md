---
title: "Week 4 Worklog"
date: 2025-09-29
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:
- Understand Amazon S3 fundamentals and storage concepts.
- Host a static website using S3 Website Hosting.
- Accelerate content delivery using CloudFront CDN.
- Implement S3 versioning and lifecycle management.
- Enable Cross-Region Replication (CRR) for durability.

### Tasks:

| Day | Task                                       | Date | Completed | Ref |
| --- | ------------------------------------------ | ------ | -------- | ---- |
| 16  | Starting with Amazon S3                    | 09/29  | 09/29    | https://cloudjourney.awsstudygroup.com/ |
| 17  | Enable Static Website on S3                | 09/30  | 09/30    | https://cloudjourney.awsstudygroup.com/ |
| 18  | Accelerate Static Website with CloudFront  | 10/01  | 10/01    | https://cloudjourney.awsstudygroup.com/ |
| 19  | Enable Bucket Versioning & Lifecycle Rules | 10/02  | 10/02    | https://cloudjourney.awsstudygroup.com/ |
| 20  | Cross-Region Replication Setup             | 10/03  | 10/03    | https://cloudjourney.awsstudygroup.com/ |

### Week 4 Achievements:

- **Mastered Amazon S3 storage fundamentals**, including:
  - Buckets, Objects, Folders, Prefixes
  - Object immutability & durability model (11 9s)
  - S3 Storage Classes (Standard, IA, Glacier, Deep Archive)
  - Object-Level Security Concepts:
    - Bucket Policy
    - ACL
    - Block Public Access controls
  - Theory source: https://cloudjourney.awsstudygroup.com/

- **Created and configured S3 bucket**, including:
  - Custom bucket naming compliance (global namespace)
  - Region selection for latency/cost
  - Enabling/Disabling public access settings
  - Understanding static website endpoint format

- **Hosted a static website on S3**, including:
  - Enabled **Static Website Hosting**
  - Set **index.html** & **error.html**
  - Uploaded site objects (HTML, CSS, JS)
  - Configured bucket policy for public read
  - Verified website availability via S3 endpoint

- **Integrated CloudFront with the S3 website**, including:
  - Created new CloudFront distribution
  - Configured S3 Origin
  - Restricted bucket access using OAI (Origin Access Identity)
  - Set caching behaviors (TTL, invalidation)
  - Observed global CDN propagation

- **Implemented S3 Versioning**, enabling:
  - Object history tracking
  - Protection against accidental deletion
  - Multiple version retention

- **Configured S3 Lifecycle Rules**, such as:
  - Transitioning objects to IA / Glacier
  - Expiration rules for unused data
  - Clean-up for outdated versions

- **Enabled Cross-Region Replication (CRR)**:
  - Created secondary bucket in another region
  - Enabled versioning on both buckets
  - Configured IAM role for replication
  - Validated automatic replication triggering

- **Conducted S3 CLI operations**, such as:
  - `aws s3 ls`
  - `aws s3 sync`
  - `aws s3 cp`
  - Viewing bucket policies & versioning config

- **Gained the ability to deploy, secure, accelerate, and automate storage operations with S3.**
