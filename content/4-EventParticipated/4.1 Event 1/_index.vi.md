---
title: "Event 1"
date: "2025-10-3"
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

# Summary Report: “GenAI-powered App-DB Modernization Workshop”

### Event Objectives

- Giới thiệu cách Generative AI đang thay đổi toàn bộ vòng đời phát triển phần mềm.
- Trình bày khả năng của Amazon Q Developer trong viết mã, kiểm thử, tạo tài liệu và hỗ trợ kiến trúc.
- Minh họa vai trò của Kiro trong DevOps và vận hành thông qua phân tích log, xử lý sự cố và tự động hóa.
- Giải thích mô hình AI-Driven Development và cách tích hợp AI vào quy trình làm việc hằng ngày.
- Cung cấp các demo thực tế giúp người tham dự nắm rõ cách áp dụng các công cụ trên.

### Speakers

- **Toan Huynh** – PMP, Senior Solutions Architect (AWS)  
- **My Nguyen** – Senior Solutions Architect | Applied AI Specialist | Thought Leader

---

### Key Highlights

- Hiểu rõ các điểm hạn chế của hệ thống cũ như khó mở rộng, chi phí bảo trì cao, phụ thuộc lẫn nhau và chu kỳ triển khai chậm.
- **Scalability hạn chế** – khó đáp ứng khi lượng người dùng tăng.
- **Chi phí bảo trì cao** – ứng dụng kế thừa yêu cầu nhiều tài nguyên hơn.
- **Tight coupling** – các thành phần ràng buộc nhau, gây khó khăn khi nâng cấp.

#### Nhận diện nhược điểm của kiến trúc ứng dụng cũ

- Chu kỳ phát hành dài → mất doanh thu và bỏ lỡ cơ hội.  
- Quy trình vận hành kém hiệu quả → giảm năng suất, tăng chi phí.  
- Không tuân thủ quy định bảo mật → rủi ro lộ dữ liệu, ảnh hưởng uy tín.

---

### Transitioning to Modern Architecture – Microservices

Việc chuyển đổi sang kiến trúc hiện đại tập trung vào mô hình modular, nơi mỗi chức năng là một **dịch vụ độc lập** và giao tiếp thông qua **events**, dựa trên ba yếu tố chính:

- **Queue Management**: xử lý tác vụ bất đồng bộ, đảm bảo giao tiếp ổn định mà không gây nghẽn.
- **Caching Strategy**: cải thiện hiệu năng, giảm độ trễ và giảm tải cho database.
- **Message Handling**: hỗ trợ mô hình pub/sub, point-to-point và streaming để tăng tính linh hoạt.

---

### Domain-Driven Design (DDD) – Workshop Notes

**Tổng quan:**  
DDD tạo sự liên kết chặt chẽ giữa phần mềm và nghiệp vụ, từ đó giảm độ phức tạp trong các hệ thống lớn. Tại workshop, DDD được áp dụng kết hợp cùng Amazon Q Developer để tăng hiệu quả trong quá trình hiện đại hóa.

**Quy trình 4 bước (theo workshop):**

1. **Identify Domain Events** – Xác định các sự kiện nghiệp vụ quan trọng.  
2. **Arrange Timeline** – Sắp xếp các sự kiện theo trình tự thời gian.  
3. **Identify Actors** – Xác định các tác nhân liên quan (người dùng/hệ thống).  
4. **Define Bounded Contexts** – Tách hệ thống thành các domain độc lập để dễ mở rộng.

**Case Study – Bookstore:**

- Ví dụ thực tế áp dụng DDD.  
- Domain events: "Order Placed", "Payment Completed", "Book Shipped".  
- Bounded contexts: Order Management, Payment Processing, Inventory.

**Context Mapping – 7 Patterns**:

Shared Kernel, Customer-Supplier, Conformist, Anticorruption Layer, Open Host Service, Published Language, Separate Ways.

**Takeaways:**

- DDD giảm coupling và tăng khả năng mở rộng.  
- Amazon Q Developer hỗ trợ mô hình hóa, sinh code và tài liệu cho các bounded contexts.  
- Context mapping đảm bảo giao tiếp trơn tru giữa các microservices.

---

### Event-Driven Architecture

- **Patterns**: Publish/Subscribe, Point-to-Point, Streaming  
- **Lợi ích**: giảm phụ thuộc, tăng khả năng mở rộng và độ bền hệ thống  
- **Sync vs Async**: lựa chọn tùy thuộc yêu cầu hiệu năng và độ tin cậy  

---

### Compute Evolution

- **Shared Responsibility**: từ EC2 → ECS → Fargate → Lambda  
- **Serverless**: không cần quản lý server, tự động scale, trả phí theo mức sử dụng  
- **Compute Selection**: chọn functions hay containers dựa vào đặc thù workload  

---

### Amazon Q Developer

- Tự động hóa toàn bộ SDLC: planning → coding → testing → deployment → maintenance.  
- Hỗ trợ **code transformation**: nâng cấp Java, hiện đại hóa .NET.  
- Tích hợp với **AWS Transform agents**: chuyển đổi VMware, Mainframe, .NET.

---

### Key Takeaways

#### Design Mindset  
- Luôn xuất phát từ nhu cầu nghiệp vụ.  
- Duy trì **ubiquitous language** giữa business và tech.  
- Sử dụng bounded contexts để giảm độ phức tạp.

#### Technical Architecture  
- Áp dụng **event storming** để mô hình hóa nghiệp vụ.  
- Tối ưu giao tiếp giữa services bằng event-driven.  
- Kết hợp nhiều integration patterns phù hợp từng trường hợp.  
- Chọn compute hợp lý: VM / Container / Serverless.

#### Modernization Strategy  
- Tiếp cận theo từng giai đoạn, tránh chuyển đổi đột ngột.  
- Áp dụng mô hình **7Rs** tùy ứng dụng.  
- Đánh giá ROI để đo lường hiệu quả.

---

### Applying to Work

- Tổ chức các buổi event storming với business.  
- Tách microservices dựa trên bounded contexts.  
- Áp dụng event-driven để thay thế một số workflow sync.  
- Thử nghiệm serverless với AWS Lambda.  
- Tích hợp Amazon Q Developer vào quy trình phát triển.

---

### Event Experience

#### Learning from Speakers  
- Nắm được các best practices về thiết kế ứng dụng hiện đại và kiến trúc AWS.  
- Hiểu rõ cách áp dụng DDD và EDA trong môi trường thực tế.

#### Hands-On Exposure  
- Thực hành event storming để mô hình hóa domain events.  
- Học cách chia microservices và xác định bounded contexts.  
- Trải nghiệm nhiều mô hình giao tiếp: sync, async, pub/sub, streaming.

#### Leveraging Tools  
- Tìm hiểu Amazon Q Developer cho tự động hóa SDLC.  
- Thử nghiệm code transformation và serverless với AWS Lambda.

#### Networking and Discussions  
- Giao lưu cùng chuyên gia và đồng nghiệp.  
- Tăng cường khả năng giao tiếp giữa business và kỹ thuật.  
- Hiểu rõ tầm quan trọng của business-first approach.

#### Lessons Learned  
- DDD + Event-Driven giúp giảm coupling, tăng scalability và resilience.  
- Hiện đại hóa cần lộ trình rõ ràng và đánh giá ROI liên tục.  
- AI như Amazon Q Developer có thể tăng mạnh năng suất nếu tích hợp đúng cách.

---


> Workshop mang đến nhiều kiến thức hữu ích và thay đổi góc nhìn về thiết kế ứng dụng, chiến lược hiện đại hóa và cách các đội nhóm hợp tác hiệu quả hơn.
