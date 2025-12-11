---
title: "Week 2 Worklog"
date: 2025-09-15
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:
- Master IAM access control, policies, and identity management.
- Build VPC networking foundations for private/public environments.
- Understand and apply network firewalls (SG + NACL).
- Deploy EC2 instances inside custom VPC.
- Establish hybrid network connectivity using VPN.

### Tasks:

| Day | Task                                                          | Start | Completion | Reference |
| --- | ------------------------------------------------------------- | ------ | ---------- | --------- |
| 6   | IAM Access Control                                            | 09/15  | 09/15      | https://cloudjourney.awsstudygroup.com/ |
| 7   | Learn and build Amazon VPC                                   | 09/16  | 09/16      | https://cloudjourney.awsstudygroup.com/ |
| 8   | VPC Firewalls (SG + NACL)                                    | 09/17  | 09/17      | https://cloudjourney.awsstudygroup.com/ |
| 9   | Deploy EC2 in custom VPC                                     | 09/18  | 09/18      | https://cloudjourney.awsstudygroup.com/ |
| 10  | Site-to-Site VPN Setup                                       | 09/19  | 09/19      | https://cloudjourney.awsstudygroup.com/ |

### Week 2 Achievements:

- **Deep understanding of IAM access control**, including:
  - Users, Groups, Roles, Policies
  - Inline vs Managed Policies
  - Permission Boundaries
  - Least Privilege Model
  - IAM Best Practices from  
    ➝ https://cloudjourney.awsstudygroup.com/

- **Hands-on policy creation**, including:
  - Custom IAM policy JSON
  - Attaching/detaching policies
  - Using IAM Access Analyzer to validate permission risks

- **Built a complete Amazon VPC from scratch**, including:
  - Custom IPv4 CIDR (10.0.0.0/16)
  - Public + Private Subnets
  - Internet Gateway
  - NAT Gateway
  - Routing Tables
  - Subnet Associations

- **Configured VPC Firewalls**:
  - **Security Groups**
    - Allowed HTTP/HTTPS/SSH
    - Instance-level firewall rules
  - **Network ACLs**
    - Stateless rules
    - Custom inbound/outbound rules
  - Understood differences between SG & NACL

- **Deployed EC2 inside custom VPC**:
  - Launched EC2 in Public Subnet
  - Attached SG + Key Pair
  - Connected via SSH
  - Installed NGINX for connectivity test
  - Validated routing and NAT behavior

- **Set up Site-to-Site VPN concepts**, including:
  - Customer Gateway (CGW)
  - Virtual Private Gateway (VGW)
  - VPN Tunnels
  - How encrypted traffic flows through IPSec
  - Routing propagation concepts

- **Used CLI for VPC operations**, such as:
  - `describe-vpcs`
  - `describe-security-groups`
  - `describe-route-tables`
  - `describe-subnets`

- **Gained solid networking foundation** for future EC2, RDS, and ECS deployments.
