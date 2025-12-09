---
title: "Event 1"
date: "2025-10-3"
weight: 4
chapter: false
pre: " <b> 4.1. </b> "
---

# Summary Report: “GenAI-powered App-DB Modernization Workshop”

### Event Objectives

- Introduce how Generative AI is reshaping the entire software development lifecycle.
- Showcase Amazon Q Developer’s features for coding, testing, documentation, and architectural support.
- Demonstrate how Kiro enhances DevOps and operations through log analysis, troubleshooting, and automation.
- Explain the AI-Driven Development model and how teams can incorporate AI into daily workflows.
- Provide practical demonstrations to help participants understand how to apply these tools effectively.

### Speakers

- **Toan Huynh** – PMP, Senior Solutions Architect (AWS)  
- **My Nguyen** – Senior Solutions Architect | Applied AI Specialist | Thought Leader

---

### Key Highlights

- Understanding common challenges in legacy systems such as limited scalability, high maintenance costs, tight coupling, and slow release cycles.
- **Scalability limitations** – systems struggle to meet increasing user demand.
- **High maintenance costs** – older systems require more resources and effort to keep running.
- **Tight coupling** – components depend on each other, making changes risky.

#### Identifying the drawbacks of legacy application architecture

- Long product release cycles → lost revenue and missed opportunities  
- Inefficient operations → reduced productivity and higher costs  
- Non-compliance with security standards → increased risk and reputational damage  

---

### Transitioning to Modern Architecture – Microservices

Modernization involves shifting to a modular architecture in which each feature is an **independent service** communicating through **events**. This approach is built on three core principles:

- **Queue Management**: Manages asynchronous tasks reliably and prevents workflow bottlenecks.  
- **Caching Strategy**: Improves performance, minimizes latency, and reduces load on databases.  
- **Message Handling**: Enables flexible, event-driven communication through pub/sub, point-to-point, and streaming patterns.

---

### Domain-Driven Design (DDD) – Workshop Notes

**Overview:**  
DDD aligns software design with real business needs, making large systems easier to manage. The workshop leveraged DDD alongside AI tools like Amazon Q Developer to support modernization.

**Four-Step Method (from the workshop):**

1. **Identify Domain Events** – Capture key business events that drive system behavior.  
2. **Arrange Timeline** – Lay out the events in chronological order to visualize workflows.  
3. **Identify Actors** – Identify the users or systems that interact with each event.  
4. **Define Bounded Contexts** – Divide the system into clear, independent domains to support scalability.

**Workshop Case Study – Bookstore Example:**

- Demonstrated practical DDD application.  
- Domain events included: “Order Placed”, “Payment Completed”, “Book Shipped”.  
- Bounded contexts: Order Management, Payment Processing, Inventory.

**Context Mapping – 7 Patterns Introduced:**

Shared Kernel, Customer-Supplier, Conformist, Anticorruption Layer, Open Host Service, Published Language, Separate Ways.

**Key Takeaways:**

- DDD helps reduce tight coupling and increases clarity in system design.  
- Amazon Q Developer supports modeling, generating code, and producing documentation for bounded contexts.  
- Context mapping ensures smooth communication across microservices during modernization.

---

### Event-Driven Architecture

- **Integration patterns**: Publish/Subscribe, Point-to-Point, Streaming  
- **Benefits**: reduced coupling, higher scalability, improved resilience  
- **Sync vs Async**: trade-offs based on performance and reliability requirements  

---

### Compute Evolution

- **Shared Responsibility Progression**: EC2 → ECS → Fargate → Lambda  
- **Serverless Benefits**: no server management, automatic scaling, pay-per-use model  
- **Choosing Compute**: select functions or containers based on workload characteristics  

---

### Amazon Q Developer

- Automates the entire SDLC: planning → coding → testing → deployment → maintenance  
- Supports **code transformation**: Java upgrades, .NET modernization  
- Works with **AWS Transform agents** for VMware, Mainframe, and .NET migrations  

---

### Key Takeaways

#### Design Mindset  
- Adopt a **business-first approach** to guide architecture decisions.  
- Establish a **ubiquitous language** shared by business and technical teams.  
- Use bounded contexts to handle complexity in large systems.

#### Technical Architecture  
- Apply **event storming** to model business processes effectively.  
- Use event-driven communication to reduce coupling.  
- Select appropriate integration patterns: sync, async, pub/sub, streaming.  
- Choose compute options—VMs, containers, or serverless—based on workload needs.

#### Modernization Strategy  
- Follow a phased modernization roadmap to avoid unnecessary risk.  
- Use the **7Rs Framework** to choose the right modernization path for each application.  
- Measure ROI to ensure business value and cost reduction.

---

### Applying to Work

- Conduct event storming sessions with business stakeholders.  
- Refactor systems into microservices using bounded contexts.  
- Implement event-driven communication to replace certain synchronous workflows.  
- Adopt serverless using AWS Lambda for appropriate workloads.  
- Integrate Amazon Q Developer into development workflows to improve productivity.  

---

### Event Experience

#### Learning from Speakers  
- Gained actionable insights into modern application design and AWS best practices.  
- Understood how DDD and Event-Driven Architecture work in real-world scenarios.

#### Hands-On Exposure  
- Participated in event storming sessions to map domain events.  
- Practiced splitting microservices and defining bounded contexts.  
- Explored communication patterns including sync, async, pub/sub, and streaming.

#### Leveraging Tools  
- Experimented with Amazon Q Developer for SDLC automation.  
- Tried code transformation and serverless deployment using AWS Lambda.

#### Networking and Discussions  
- Engaged with experts and peers to exchange ideas and perspectives.  
- Strengthened communication between business and technical teams.  
- Saw how the business-first mindset enhances architecture decisions.

#### Lessons Learned  
- Combining DDD with event-driven patterns reduces coupling and improves scalability and resilience.  
- Modernization requires a structured, phased plan with clear ROI tracking.  
- AI tools like Amazon Q Developer significantly boost productivity when integrated into workflows.

---


> Overall, the workshop delivered valuable technical knowledge and reshaped perspectives on application design, modernization strategy, and cross-team collaboration.
