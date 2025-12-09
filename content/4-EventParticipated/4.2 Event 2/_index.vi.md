---
title: "Event 2"
date: "2025-11-19"
weight: 4
chapter: false
pre: " <b> 4.2. </b> "
---

# Báo Cáo Tổng Kết: “Defense from Public Threat: AWS WAF & Application Protection”

### Mục tiêu sự kiện

- Trình bày các rủi ro bảo mật phổ biến đối với ứng dụng tiếp xúc Internet và cách giảm thiểu hiệu quả.  
- Giải thích hoạt động của AWS WAF, chiến lược triển khai và cách cấu hình rule nâng cao.  
- Mô tả khả năng AWS WAF Bot Control trong việc xử lý các mối đe dọa tự động.  
- Tổng quan cơ chế bảo vệ DDoS của AWS Shield, bao gồm các cải tiến mới như mô hình giá trọn gói (flat-rate).  

### Diễn giả

- Nguyễn Gia Hưng
- Julian Ju

---

# Điểm nổi bật

### Rủi ro trong kiến trúc web 3-tier truyền thống

- Việc tiếp xúc trực tiếp với Internet mở ra nhiều lỗ hổng, có thể dẫn đến downtime kéo dài, tiêu tốn tài nguyên và vi phạm quy định.  
- Ảnh hưởng kinh doanh: chi phí hạ tầng tăng cao, rò rỉ dữ liệu, lộ thông tin đăng nhập, spam, downtime tăng, hệ thống kém ổn định, nhân viên bị quá tải và giảm uy tín doanh nghiệp.  

### Ba nhóm mối đe dọa chính từ Internet

- **Tấn công từ chối dịch vụ (DoS/DDoS):**  
  Bao gồm các cuộc tấn công volumetric L3/L4 và flood L7. AWS ghi nhận mức tăng 29% mỗi năm đối với tấn công tầng ứng dụng.

- **Lỗ hổng ứng dụng:**  
  CVE, OWASP Top 10 như XSS, SQL injection, path traversal...

- **Bot hoạt động tự động:**  
  Scraper, bot săn hàng, bot giả mạo, và đặc biệt là bot AI (GPT, Claude, Perplexity, ByteDance, Meta AI) tăng tới **155%**.

### Xu hướng tấn công gia tăng

- DDoS tăng mạnh từ 2021 đến Q1 2025, ở cả lớp hạ tầng và lớp ứng dụng.  
- Bot AI phát triển nhanh, tạo ra thách thức mới cho hệ thống bảo mật.

---

# Chiến lược phòng thủ với các dịch vụ AWS

### Route 53 – Tăng cường khả năng chịu lỗi DNS

- Mạng DNS toàn cầu, tự động mở rộng, tích hợp DDoS protection, SLA uptime 100%.

### Amazon CloudFront – Lớp bảo vệ tại Edge

- Điều hướng người dùng đến PoP gần nhất, chỉ cho phép cổng HTTP/S, hỗ trợ giảm thiểu DDoS L3/L4.  
- Tăng khả năng chống chịu nhờ caching.  
- **VPC Origin Protection:** ALB đặt trong private subnet, chỉ CloudFront được phép truy cập.

### AWS Shield – Bảo vệ chống DDoS

- **Lớp bảo vệ biên:** SYN proxy, phân tích gói tin, lọc traffic, geo restriction, và cơ chế dựa trên sức khỏe hệ thống.  
- **Shield Advanced:**  
  - Tự động sinh rule L7  
  - Bù chi phí do tấn công  
  - Hỗ trợ chủ động từ Shield Response Team (SRT)

---

# Mô hình giá trọn gói CloudFront mới

### Gói cố định theo tháng

- Free ($0), Pro ($15), Business ($200), Premium ($1,000)  
- Không yêu cầu cam kết dài hạn.

### Bao gồm trong gói

- CloudFront CDN  
- AWS WAF & DDoS Protection  
- Bot management & analytics  
- Route 53 DNS  
- CloudWatch Logs  
- Serverless compute at edge  
- Tín dụng lưu trữ S3 hàng tháng  

### Hạn mức sử dụng

- Free: 1M requests + 100GB data  
- Pro: 10M requests + 50TB data  
- Cảnh báo tại 50% / 80% / 100%  
- Không phát sinh phí vượt mức – có thể giảm hiệu năng khi quá tải

### Lưu ý quan trọng

- Traffic bị WAF chặn và traffic tấn công DDoS **không tính vào hạn mức**  
→ Loại bỏ hoàn toàn nguy cơ “sốc hóa đơn”.

### Giá trị mang lại

- Xóa bỏ chi phí khó dự đoán do spike, bot attack, viral, marketing.  
- Giúp team tập trung vào sản phẩm thay vì lo về chi phí phát sinh.

---

# AWS WAF – Chức năng và triển khai

### Cấu trúc Web ACL

- Rule, rule group (managed/custom/marketplace) và default action.  
- Hỗ trợ ghi log và sampling.

### Cơ chế rule

- Kiểm tra IP, header, body, URI...  
- Action: Allow / Block / Challenge / CAPTCHA / Count.  
- Tùy chỉnh linh hoạt.

### Rate-based rule

- Theo dõi request theo IP hoặc custom key.  
- Threshold từ 10 đến 20 triệu request trong 1–10 phút.

### Labels – Tinh chỉnh logic

- Gắn nhãn bot, fraud, geo hoặc dấu hiệu phù hợp khác.  
- Cho phép ngoại lệ (ví dụ allow XSS ở endpoint test).

---

# Thứ tự rule được khuyến nghị

1. IP allow/block, rule chống DDoS, rate limit  
2. Rule danh tiếng, chống tấn công phổ biến, rule chuyên biệt  
3. Bot/fraud detection và custom override (bắt đầu ở Count mode)

**Tối ưu chi phí:**  
- Ưu tiên rule rẻ hơn ở đầu pipeline  
- Dùng scope-down để giảm chi phí rule premium

---

# Bot Control – Phân tích chuyên sâu

### Bot hợp lệ

- Nhận diện theo User-Agent, IP range, TLS fingerprint.  
- Gắn nhãn: category / verified.

### Bot né tránh

- Chặn bằng thử thách JS/CAPTCHA, theo dõi telemetry, kiểm tra trình duyệt và token.  
- Dấu hiệu nhận diện: thiếu token, số lượng request bất thường, dấu hiệu automation, hành vi không nhất quán.  
- Hành động: Challenge → Block.

---

# Shield Advanced – Tính năng mở rộng

- **Insights:** Metrics CloudWatch theo dõi traffic, drop, timeline  
- **Hỗ trợ phản ứng:** Phân tích log, hướng dẫn tạo rule, tư vấn kiến trúc  
- **Auto–mitigation:** Rule áp dụng Count trước, Block sau; tự xóa khi sự kiện kết thúc

---

# CloudFront như reverse proxy – Ưu điểm kỹ thuật

- Kết thúc TLS tại PoP gần nhất  
- Truyền tải qua AWS backbone  
- Giảm tải backend (ALB/EC2/EKS/S3/API Gateway)  
- Chặn tấn công từ edge, tiết kiệm compute/database/network  

### Phù hợp với

- Startup / SaaS  
- Website & API public  
- E-commerce  
- Nền tảng giáo dục & cộng đồng  
- Hệ thống dễ bị bot hoặc DDoS tấn công  

---

# Key Takeaways

### Góc nhìn bảo mật

- Xem kết nối Internet là rủi ro chính → phòng thủ từ vòng ngoài.  
- Áp dụng chiến lược nhiều lớp: L3/L4 + L7.  
- Bắt đầu bằng Count mode để quan sát → sau đó bật Block.

### Góc kỹ thuật

- Sắp xếp priority rule hợp lý, dùng label để tinh chỉnh logic.  
- Phân biệt bot tốt/xấu bằng thử thách, token, hành vi.  
- Tăng khả năng chịu tải DDoS với Route 53 + CloudFront + Shield.  
- Tận dụng CloudFront để lọc traffic ngay tại edge.

### Chiến lược & chi phí

- Gói flat-rate giúp chi phí dự đoán được.  
- Không lo phí phát sinh khi bot/spike/attack.  
- Triển khai theo từng giai đoạn, theo dõi qua alert/metric.  
- Đảm bảo uptime, bảo vệ dữ liệu, tối ưu chi phí dài hạn.

---

# Ứng dụng vào công việc

- Đánh giá các thành phần lộ diện Internet và triển khai WAF để giảm thiểu OWASP/CVE.  
- Áp dụng challenge/token ở khu vực nhạy cảm để chống AI bot/scraper.  
- Bật Shield cho tài sản quan trọng, triển khai rate-limit hợp lý.  
- Kết nối CloudFront + WAF + rule managed và tinh chỉnh bằng label/exception.  
- Theo dõi CloudWatch và nhận hỗ trợ từ SRT khi cần.  
- Thử nghiệm gói flat-rate (Free/Pro), sau đó nâng lên Business/Premium khi chạy production.

---

# Trải nghiệm sự kiện

Workshop **“Defense from Public Threat: AWS WAF & Application Protection”** mang lại góc nhìn chuyên sâu về bảo vệ ứng dụng trước các mối đe dọa hiện đại, cùng với nhiều cập nhật mới từ AWS.

### Kiến thức từ chuyên gia

- Các chuyên gia AWS trình bày thông tin tình báo về tấn công thực tế và các mô hình phòng thủ.  
- Ví dụ về DDoS theo thời gian và sự gia tăng bot AI giúp hiểu rõ cách áp dụng WAF/Shield thực tế.

### Thực hành bảo mật

- Thao tác với rule WAF, rate limit, label/exception.  
- Tìm hiểu cách phân biệt bot hợp lệ và bot né tránh.  
- So sánh nhiều mô hình giảm thiểu: sync/async, inline/health-based.

### Tận dụng tính năng mới

- Hiểu rõ sức mạnh của CloudFront + Route 53 trong bảo vệ perimeter.  
- Tìm hiểu auto-rule và cost protection của Shield Advanced.  
- Tối ưu chi phí với scope-down và traffic exemption.

### Thảo luận & chia sẻ

- Tương tác về rule pattern, quy trình incident response và mô hình bảo mật nhiều lớp.  
- Chia sẻ kinh nghiệm triển khai từ cơ bản đến nâng cao.

### Bài học rút ra

- Hệ thống phòng thủ tự động là bắt buộc trước sự gia tăng bot & DDoS.  
- Giám sát trước khi bật Block giúp tránh sai sót.  
- Gói flat-rate thay đổi hoàn toàn cách dự toán chi phí, mang lại bảo mật mạnh với giá hợp lý.

