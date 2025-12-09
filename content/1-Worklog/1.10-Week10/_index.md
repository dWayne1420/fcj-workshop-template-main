---
title: "Week 10 Worklog"
date: 2025-11-10
weight: 1
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:
- Learn AWS DevOps tools for CI/CD automation.
- Create repositories using CodeCommit.
- Build and test applications using CodeBuild.
- Deploy applications using CodeDeploy.
- Automate entire CI/CD lifecycle using CodePipeline.

### Tasks:

| Day | Task                           | Date | Completed | Ref |
| --- | ------------------------------ | ------ | -------- | ---- |
| 46  | Learn AWS DevOps Toolchain     | 11/10  | 11/10    | https://cloudjourney.awsstudygroup.com/ |
| 47  | Set up CodeCommit Repo         | 11/11  | 11/11    | https://cloudjourney.awsstudygroup.com/ |
| 48  | Build App with CodeBuild       | 11/12  | 11/12    | https://cloudjourney.awsstudygroup.com/ |
| 49  | Deploy with CodeDeploy         | 11/13  | 11/13    | https://cloudjourney.awsstudygroup.com/ |
| 50  | Create Full CI/CD Pipeline     | 11/14  | 11/14    | https://cloudjourney.awsstudygroup.com/ |

### Week 10 Achievements:

- **Learned AWS DevOps Ecosystem**, understanding:
  - CodeCommit (Git hosting)
  - CodeBuild (build automation)
  - CodeDeploy (deployment automation)
  - CodePipeline (CI/CD orchestration)
  - Artifact storage (S3)
  - IAM Permissions for DevOps workflows

- **Created CodeCommit Repository**:
  - Configured Git credentials for IAM
  - Cloned repo & pushed code
  - Versioned application source via Git

- **Configured CodeBuild**, including:
  - Created build specifications (`buildspec.yml`)
  - Installed dependencies
  - Unit testing scripts
  - Build artifacts output to S3
  - Parallel builds + build logs

- **Deployed application using CodeDeploy**, including:
  - Deployment groups
  - AppSpec configuration (`appspec.yml`)
  - EC2 deployment lifecycle hooks
  - Managed automatic rollback on failure

- **Created Full CI/CD Pipeline**, including:
  - CodeCommit → CodeBuild → CodeDeploy → EC2
  - Configured event triggers on Git push
  - Automated deployments on every commit
  - Added manual approval stage for production

- **Verified CI/CD end-to-end flow**:
  - Made Git commits
  - Observed automatic build → deploy
  - Checked logs for build/deploy stages

- **Gained strong foundation in AWS DevOps automation for production readiness.**
