---
title: "3.3. Blog 3"
date: 2025-09-22
draft: false
---
# Hướng dẫn giảm thiểu lãng phí và nâng cao hiệu quả với AWS

AWS Public Sector Blog  
Hướng dẫn giảm thiểu lãng phí và nâng cao hiệu quả với AWS  
bởi Henrik Balle, Bhanu Jasthi, và Maia Haile | 22 tháng 9 năm 2025 | tại Artificial Intelligence, Best Practices, Cloud Adoption, Generative AI, Government, Mainframe Migration, Migration Solutions, Public Sector | Permalink 

## Giới thiệu

Tổng cục Quản lý Dịch vụ Hoa Kỳ (U.S. General Services Administration - GSA) gần đây đã công bố một thỏa thuận OneGov đột phá với Amazon Web Services (AWS) nhằm cung cấp khoản tiết kiệm lên đến 1 tỷ USD cho việc áp dụng công nghệ đám mây, hiện đại hóa và đào tạo cho các cơ quan liên bang. Cùng với thông báo này là các giải pháp để giảm lãng phí và nâng cao hiệu quả.

Để giúp các tổ chức đẩy nhanh các sáng kiến này và giảm thiểu gian lận, lãng phí và lạm dụng (FWA), hướng dẫn này đưa ra các chiến lược thực tiễn để tối ưu hóa chi tiêu công nghệ đồng thời cải thiện hiệu quả vận hành. Chúng tôi sẽ trình bày một cách tiếp cận ba cấp độ để tối ưu hóa:

- Sáng kiến chuyển đổi số toàn cơ quan  
- Tinh chỉnh môi trường AWS  
- Cải tiến ở cấp độ dịch vụ  

Mỗi cách tiếp cận bao gồm các tài nguyên và các bước hành động mà các tổ chức có thể bắt đầu thực hiện ngay hôm nay.

## Sáng kiến chuyển đổi số toàn cơ quan

Chuyển đổi công nghệ thông tin quy mô lớn bằng cách sử dụng các ưu đãi OneGov bắt đầu với việc migration và modernization thông qua áp dụng công nghệ đám mây. Ngoài việc hưởng lợi từ thỏa thuận OneGov, nghiên cứu của The Hackett Group cho thấy các tổ chức chuyển đổi sang AWS đạt được mức giảm chi phí cơ sở hạ tầng trung bình 20%, với các tổ chức hàng đầu đạt được mức tiết kiệm lên đến 47%. Ngoài hiệu quả chi phí, các cơ quan còn đạt được mức tăng 66% về năng suất cơ sở hạ tầng và chuyển hướng 29% thời gian để đổi mới sáng tạo.

Dù bạn chọn thoát hoàn toàn khỏi các trung tâm dữ liệu (data centers) hay dần dần di chuyển các ứng dụng theo thời gian, bước đầu tiên quan trọng là thu thập dữ liệu danh mục ứng dụng (application portfolio data). Dữ liệu này phải được đánh giá dựa trên bảy chiến lược di chuyển phổ biến, được gọi là **7 Rs**: refactor, replatform, repurchase, rehost, relocate, retain, và retire. Theo các chiến lược này, các cơ quan có thể xác định con đường di chuyển tốt nhất cho từng ứng dụng.

Đối với một số khối lượng công việc được xây dựng trên các công nghệ được cấp phép thương mại, bạn cũng có thể cân nhắc chương trình **AWS Optimization and Licensing Assessment (AWS OLA)** bổ sung, giúp tăng hiệu quả cấp phép lên đến 60% bằng cách xác định các giấy phép sử dụng chưa đầy đủ và đề xuất các lựa chọn thay thế tiết kiệm chi phí hơn.

Các hệ thống kế thừa (legacy systems) tiêu tốn một phần ngân sách công nghệ thông tin không cân đối. Với **AWS Transform**, các ứng dụng .NET có thể được hiện đại hóa nhanh hơn đến bốn lần đồng thời giảm chi phí vận hành lên đến 40% thông qua việc loại bỏ giấy phép Windows. Việc di chuyển VMware loại bỏ các chi phí cấp phép bên thứ ba đắt đỏ và tăng tốc độ chuyển đổi mạng lên đến 80 lần. Với sức mạnh của agentic AI, việc hiện đại hóa mainframe rút ngắn thời gian từ vài năm xuống vài tháng, giảm chi phí mainframe liên tục và bảo toàn logic kinh doanh quan trọng.

Các cơ quan liên bang có thể đơn giản hóa hoạt động trung tâm liên lạc (contact center) và loại bỏ lãng phí bằng cách hợp nhất nhiều nền tảng trung tâm liên lạc thành một nền tảng dựa trên đám mây thống nhất. **Amazon Connect** cung cấp mô hình pay-as-you-go và không yêu cầu cam kết tối thiểu. Các khả năng AI tích hợp tạo ra một vòng lặp hiệu quả mạnh mẽ, cho phép tự phục vụ người gọi, hỗ trợ nhân viên theo thời gian thực và tự động tạo tóm tắt, đồng thời triển khai các AI agents cho các công việc thường xuyên.  

Để tìm hiểu cách khách hàng đã giảm 60% khối lượng cuộc gọi và giảm 50% thời gian đào tạo nhân viên, hãy truy cập *Unleash AI để chuyển đổi mọi tương tác với khách hàng*.

Các cơ quan ngày càng tìm kiếm cải tiến trong năng suất nhân viên. **Amazon Q Business** giúp generative AI dễ dàng tiếp cận một cách an toàn cho mọi người trong tổ chức. Amazon Q Developer có thể tăng năng suất của nhà phát triển lên đến 40%, giúp họ viết mã nhanh hơn và an toàn hơn.

## Tinh chỉnh môi trường AWS

Cách tốt nhất để tối ưu hóa chi tiêu lãng phí là tránh các chi phí không cần thiết ngay từ đầu. AWS khuyến nghị sử dụng các phương pháp bảo mật tốt nhất trong **AWS Identity and Access Management (IAM)** khi thiết lập người dùng mới trong môi trường AWS. Điều này bao gồm việc thường xuyên xem xét và xóa các đặc quyền không sử dụng.

Khách hàng có thể tinh chỉnh thêm bằng cách sử dụng **AWS Service Catalog**, cung cấp cho người dùng cuối một cổng để khám phá và khởi chạy các sản phẩm tuân thủ chính sách tổ chức và giới hạn ngân sách.

AWS cung cấp một bộ giải pháp để hỗ trợ quản lý và tối ưu hóa chi phí:

- theo dõi chi phí và mức sử dụng  
- consolidated billing  
- lập ngân sách và dự báo  
- tối ưu hóa tài nguyên và giá  

Các tài nguyên như backups phát sinh chi phí ngay khi tạo. **AWS Backup** loại bỏ chi phí quản lý phần mềm sao lưu và cơ sở hạ tầng, đồng thời cung cấp các tính năng tiết kiệm chi phí thông qua *automated lifecycle policies*.  

Bạn có thể giảm chi phí bằng cách:

- chuyển bản sao lưu ít được truy cập sang cold storage  
- tự động xóa bản sao lưu hết hạn  

**SageMaker Unified Studio** cho phép tìm và truy cập dữ liệu trong tổ chức để phân tích và xây dựng ứng dụng generative AI.

Nếu vẫn dùng công cụ hiện có, bạn có thể giảm chi phí dữ liệu bằng kiến trúc **data mesh** sử dụng AWS Lake Formation để quản trị dữ liệu phi tập trung.

## Tối ưu hóa chi phí ở cấp độ dịch vụ

Kiến trúc **serverless** giúp giảm total cost of ownership bằng mô hình pay-for-value. AWS Well-Architected Framework cung cấp best practices cho serverless.

Đối với ứng dụng chạy máy ảo:

- **AWS Graviton** mang lại hiệu suất giá tốt hơn đến 40%.  
- **Auto Scaling** duy trì hiệu suất ổn định với chi phí thấp.  

Chuyển từ cơ sở dữ liệu thương mại sang **Amazon Aurora** có thể giảm chi phí xuống còn 1/10.

Nâng cấp từ **EBS gp2 → gp3** tiết kiệm đến 20%.

**Amazon CloudFront** giảm độ trễ và giúp tiết kiệm chi phí phân phối nội dung.

**AWS Compute Optimizer** giúp rightsizing EC2 và RDS.  

**Savings Plans** tiết kiệm đến 72% so với On-Demand.

**Amazon EC2 Spot Instances** tiết kiệm đến 90% cho batch, analytics và AI pre-training.

**Amazon S3 Intelligent-Tiering** tự động tối ưu chi phí lưu trữ.

Với generative AI:

- dùng Amazon Q Business / Developer trước khi tự xây dựng  
- dùng mô hình nhỏ như *Amazon Nova Micro* tiết kiệm đến 70%  
- mô hình distilled trên Bedrock nhanh hơn 500% và rẻ hơn 75%  
- dùng **S3 Vectors** giảm chi phí RAG lên đến 90%  
- **prompt caching** giảm chi phí inference 90%  

## Kết luận

Các khuyến nghị trong tài liệu này sẽ giúp bạn giảm lãng phí và tối ưu hóa chi phí dù bạn đang ở đâu trên hành trình đám mây của mình. Để đi sâu hơn, hãy tham khảo **Cost Optimization Pillar** của AWS Well-Architected Framework.

Liên hệ đội ngũ AWS của bạn để tìm hiểu cách tối đa hóa lợi ích từ thỏa thuận OneGov.

**THẺ:** Artificial Intelligence, AWS Public Sector, best practices, cloud migration, government, mainframe migration, modernization

## Tác Giả

### Henrik Balle
Principal solutions architect tại AWS, hỗ trợ khu vực công Hoa Kỳ. Anh làm việc với nhiều chủ đề từ machine learning đến security và governance quy mô lớn.

### Bhanu Jasthi
Senior solutions architect tại AWS, với hơn 20 năm kinh nghiệm trong cloud architecture, disaster recovery và high availability.

### Maia Haile
Solutions architect tại AWS khu vực Washington DC, chuyên hỗ trợ khách hàng khu vực công với các giải pháp AWS well-architected.  
