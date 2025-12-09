---
title: "Event 2"
date: "2025-11-19"
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Summary Report: “Defense from Public Threat: AWS WAF & Application Protection”

### Event Objectives

- Highlight common security risks for internet-facing applications and outline effective mitigation strategies.  
- Explain AWS WAF operations, deployment best practices, and advanced rule configurations.  
- Describe AWS WAF Bot Control capabilities for defending against automated threats.  
- Provide an overview of AWS Shield’s DDoS protection mechanisms and enhancements, including the new flat-rate pricing model for bundled services.  

### Speakers

- Nguyen Gia Hung
- Julian Ju

---

# Key Highlights

### Security Risks in a Typical 3-Tier Web Architecture

- Direct internet exposure introduces vulnerabilities that may result in prolonged outages, resource exhaustion, and compliance failures.  
- Business impacts include elevated infrastructure spend, data breaches, leaked credentials, spam surges, downtime, operational instability, staff fatigue, and loss of customer trust.  

### Major Categories of Internet Threats

- **Denial of Service (DoS/DDoS):**  
  Includes L3/L4 volumetric attacks and L7 application floods. AWS reports a 29% year-over-year increase in application-layer events.  

- **Application Vulnerabilities:**  
  CVEs and OWASP Top 10 risks such as XSS and injection attacks.  

- **Bot Activity:**  
  Scrapers, scalpers, spoofed clients, and rapidly growing AI-driven bots (GPT, Claude, Perplexity, ByteDance, Meta AI), with a 155% increase in traffic.

### Rising Attack Trends

- DDoS incidents continue to escalate, with infrastructure-level and application-level impact patterns illustrated from 2021 to Q1 2025.  
- AI-powered bots introduce new challenges across a diverse range of customer workloads.

---

# Defensive Strategies Using AWS Services

### Route 53 – DNS Resilience

- Global traffic management, auto-scaling, built-in DDoS protections, and a 100% uptime SLA.

### Amazon CloudFront – Edge Protection

- Routes traffic through the nearest Point of Presence.  
- Restricts requests to HTTP/S ports, adds inline L3/L4 DDoS mitigation, and increases resilience through caching.  
- With **VPC Origin Protection**, the ALB stays private and only CloudFront may access it.

### AWS Shield – Infrastructure Defense

- **Edge & Border Protections:** SYN proxies, packet inspection, geo controls, traffic scrubbing, and health-based mitigation.  
- **Advanced Features:**  
  Automatically generated L7 rules, attack cost-protection credits, and support from the Shield Response Team (SRT).

---

# New CloudFront Flat-Rate Pricing Model

### Fixed Monthly Bundles

- Free ($0), Pro ($15), Business ($200), Premium ($1,000)  
- No long-term contracts

### Included Services

- CloudFront CDN  
- AWS WAF & DDoS protection  
- Bot management & analytics  
- Route 53 DNS  
- CloudWatch Logs ingestion  
- Serverless compute at the edge  
- Monthly S3 storage credits  

### Usage Allowances

- Free tier: 1M requests + 100 GB data  
- Pro tier: 10M requests + 50 TB data  
- Alerts triggered at 50%, 80%, and 100% consumption  
- No overage fees — performance throttling may apply  

### Important Exclusion

- WAF-blocked traffic and DDoS attack traffic **do not count** toward usage quotas → prevents unexpected bills during attacks, viral events, or sudden spikes.

### Purpose

- Eliminates unpredictable multi-service expenses.  
- Prevents billing shocks caused by marketing surges, bot attacks, or unexpected virality.  
- Encourages teams to focus on product development instead of infrastructure cost risks.

---

# AWS WAF – Core Functions and Deployment

### Web ACL Structure

- Rules, rule groups (managed, custom, marketplace), and default actions.  
- Support for logging and traffic sampling.

### Rule Logic

- Inspects IPs, headers, bodies, and other attributes.  
- Supports Allow, Block, Challenge, CAPTCHA, and Count actions.  
- Highly customizable.

### Rate-Based Rules

- Track requests by IP or custom keys.  
- Thresholds from 10 to 20M requests over 1–10 minutes.

### Labels for Fine-Grained Control

- Tag bot, fraud, geo, or match behaviors.  
- Enable selective exceptions (e.g., allow XSS for specific endpoints if required).

---

# Recommended WAF Rule Ordering

1. Allow/Block IPs, anti-DDoS managed rules, and rate-based protections.  
2. Anonymous/reputation checks, core attack protections, and specialized signatures.  
3. Bot/fraud rules and custom overrides, starting in **Count** mode to avoid false positives.  

**Optimization Tips:**  
- Prioritize cheaper rules at the top.  
- Use scope-down statements to reduce premium rule costs.

---

# Bot Control – Detailed Capabilities

### Known Bots

- Identified through User-Agent, IP ranges, or TLS fingerprints.  
- Labeled by category and verification status.

### Evasive Bots

- Countered using JavaScript/CAPTCHA challenges, telemetry tracking, browser verification, and token-based anomaly detection.  
- Indicators include missing tokens, abnormal request volumes, automation signatures, or inconsistent behavior.  
- Mitigation ranges from Challenge to full Block.

---

# Shield Advanced – Additional Benefits

- **Insights:** CloudWatch metrics for traffic volume, drops, and timelines.  
- **Response Assistance:** Guidance on log analysis, rule creation, and architectural hardening.  
- **Auto-Mitigation:** Rules applied in Count mode first, then enforced; automatically removed after events.

---

# CloudFront as a Reverse Proxy – Technical Advantages

- Local TLS termination at edge locations.  
- Traffic routed through the AWS global backbone.  
- Offloads backend infrastructure (ALB, EC2, EKS, S3, API Gateway).  
- Blocks malicious traffic at the edge, reducing compute, database, and network load — even without caching.

### Ideal Users for Advanced Protections

- Startups & SaaS platforms  
- Public-facing websites and APIs  
- E-commerce applications  
- Education and community platforms  
- Environments susceptible to bots or DDoS attacks  

---

# Key Takeaways

### Security Perspective

- Treat public internet exposure as a primary threat vector.  
- Use a layered approach combining L3/L4 and L7 defenses.  
- Begin with Count mode, observe traffic, then enforce blocks gradually.

### Technical Safeguards

- Structure WAF rules thoughtfully, use labels for precision, and mix managed with custom protections.  
- Apply bot interrogation methods, tokens, and behavior tracking to differentiate malicious automation.  
- Strengthen DDoS resilience with Route 53, CloudFront, and Shield.  
- Utilize CloudFront for edge filtering and infrastructure offloading.

### Cost & Strategy Improvements

- Flat-rate bundles deliver predictable pricing and exclude attack traffic.  
- Remove risk of cost spikes from surges or threats.  
- Build protection incrementally, validate through alerts and metrics.  
- Evaluate long-term value: lower downtime, stronger security posture, predictable budgeting.

---

# Applying to Work

- Assess internet exposures and deploy WAF for OWASP/CVE risk mitigation.  
- Implement bot defenses (challenges/tokens) on sensitive endpoints.  
- Enable Shield for critical assets and configure rate-limiting.  
- Start using CloudFront with managed WAF rules and refine with labels/exceptions.  
- Use CloudWatch and SRT guidance for visibility and response enhancements.  
- Pilot flat-rate tiers (Free/Pro) and scale to Business/Premium for production workloads.

---

# Event Experience

Attending **“Defense from Public Threat: AWS WAF & Application Protection”** provided deep insights into securing modern applications against rapidly evolving online threats, enriched by recent AWS feature updates.

### Expert Insights

- AWS specialists shared practical threat intelligence and demonstrated integrations using architectural diagrams and global edge network maps.  
- Real-world examples of DDoS escalations and rising AI bot traffic helped clarify how to apply WAF and Shield effectively.

### Hands-On Defensive Exploration

- Explored WAF configurations, rate rules, and label-based exceptions to handle false positives.  
- Learned bot interrogation techniques using fingerprints, telemetry, and browser verification.  
- Compared synchronous vs. asynchronous mitigations and inline vs. health-based detection.

### Leveraging New Features

- Understood how CloudFront and Route 53 strengthen perimeter security.  
- Reviewed Shield’s auto-generated rules and cost protection benefits.  
- Learned cost optimization tactics such as scope-down rules and attack-based exclusions.

### Collaboration and Discussions

- Interactive discussions covered rule design, incident response, and bridging conceptual knowledge with operational practice.  
- Emphasis on evolving from foundational protection to layered, advanced security architectures.

### Lessons Learned

- Automated defenses are essential to counter rising bot and DDoS activity.  
- Start with monitoring phases before enforcing rules to minimize disruption.  
- Flat-rate pricing fundamentally improves cost predictability while strengthening security.

