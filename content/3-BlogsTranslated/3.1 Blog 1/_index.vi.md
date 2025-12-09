---
title: "3.1. Blog 1"
date: 2025-09-22
draft: false
---
# Bản tin hàng tuần của AWS: Amazon Q Developer, AWS Step Functions, Hạn chót AWS Cloud Club Captain, và hơn thế nữa (22 tháng 9, 2025)

Bản tin hàng tuần của AWS: Amazon Q Developer, AWS Step Functions, Hạn chót AWS Cloud Club Captain, và hơn thế nữa (22 tháng 9, 2025)
bởi Donnie Prakoso | 22 tháng 9 năm 2025 | Amazon Bedrock, Amazon Q Developer, Amazon VPC, AWS Step Functions, News | Permalink 

Ba tuần trước, tôi đã đăng một bài viết về AWS Region mới tại New Zealand (ap-southeast-6). Điều này đã dẫn đến một cơ hội tuyệt vời để đến thăm New Zealand, nơi tôi gặp gỡ những nhà phát triển đầy nhiệt huyết và trình bày tại một số sự kiện bao gồm Serverless và Platform Engineering meetup, AWS Tools and Programming meetup, AWS Cloud Clubs tại Auckland, và AWS Community Day New Zealand.

Trong quá trình tạo nội dung cho các bài thuyết trình này, tôi đã khám phá ra một tính năng hữu ích trong Amazon Q CLI được gọi là tangent mode. Tính năng này đã thay đổi cách tôi duy trì sự tập trung bằng cách tạo ra các điểm kiểm tra hội thoại, cho phép bạn khám phá các chủ đề phụ mà không làm mất mạch chính.

Tính năng này đang ở chế độ thử nghiệm, và bạn có thể kích hoạt nó bằng lệnh q settings chat.enableTangentMode true. Hãy thử và xem liệu nó có hữu ích cho bạn không.

## Các cập nhật tuần trước

Dưới đây là một số cập nhật đã thu hút sự chú ý của tôi:

● Các mô hình nền tảng mới trong Amazon Bedrock — Amazon Bedrock mở rộng lựa chọn mô hình với dòng mô hình Qwen, DeepSeek-V3.1, và dịch vụ hình ảnh Stability AI hiện đã chính thức ra mắt, mang đến cho các nhà phát triển quyền truy cập vào các mô hình đa ngôn ngữ mạnh mẽ và khả năng tạo hình ảnh tiên tiến cho các tác vụ như tạo văn bản, tạo mã, tạo hình ảnh, và giải quyết các vấn đề phức tạp.

● Amazon VPC Reachability Analyzer mở rộng đến bảy vùng mới — Khả năng Network Access Analyzer hiện đã có sẵn ở các vùng bổ sung, giúp khách hàng phân tích và khắc phục sự cố kết nối mạng trong cơ sở hạ tầng VPC với phạm vi phủ sóng toàn cầu được cải thiện.

● Amazon Q Developer hỗ trợ máy chủ MCP từ xa — Amazon Q Developer giờ đây tích hợp với các máy chủ Model Context Protocol (MCP) từ xa, cho phép các nhà phát triển mở rộng khả năng trợ lý AI của họ với các công cụ và nguồn dữ liệu tùy chỉnh để cải thiện quy trình phát triển.

● AWS Step Functions nâng cấp Distributed Map với các tùy chọn nguồn dữ liệu mới — Step Functions giới thiệu các tùy chọn nguồn dữ liệu bổ sung và các tính năng quan sát cải tiến cho Distributed Map, giúp xử lý các khối lượng công việc song song quy mô lớn dễ dàng hơn với khả năng giám sát và gỡ lỗi tốt hơn.

● Amazon Corretto 25 chính thức ra mắt — Phân phối OpenJDK 25 miễn phí, đa nền tảng của Amazon hiện đã chính thức ra mắt, cung cấp cho các nhà phát triển Java hỗ trợ dài hạn, cải tiến hiệu suất và cập nhật bảo mật để xây dựng các ứng dụng hiện đại.

● Amazon SageMaker HyperPod giới thiệu Autoscaling — SageMaker HyperPod giờ đây hỗ trợ khả năng tự động mở rộng, cho phép các nhóm học máy điều chỉnh động tài nguyên tính toán dựa trên nhu cầu khối lượng công việc, tối ưu hóa cả hiệu suất và chi phí cho các công việc huấn luyện phân tán.

## Các cập nhật khác

● AWS được vinh danh là Leader trong Gartner Magic Quadrant 2025 cho AI Code Assistants – AWS đã được công nhận là Leader trong Gartner’s Magic Quadrant cho AI Code Assistants, làm nổi bật khả năng của Amazon Q Developer trong việc giúp các nhà phát triển viết mã nhanh hơn và an toàn hơn với các gợi ý được hỗ trợ bởi AI.

● Trở thành AWS Cloud Club Captain – Chỉ còn vài ngày trước khi đóng đăng ký! Tham gia mạng lưới ngày càng phát triển của các sinh viên đam mê công nghệ đám mây bằng cách trở thành AWS Cloud Club Captain! Là một Captain, bạn sẽ tổ chức các sự kiện và xây dựng cộng đồng đám mây trong khi phát triển kỹ năng lãnh đạo. Cửa sổ đăng ký mở từ ngày 1 đến 28 tháng 9, 2025.

## Các sự kiện AWS sắp tới

Hãy kiểm tra lịch của bạn và đăng ký cho các sự kiện AWS sắp tới cũng như AWS re:Invent và AWS Summits:

● AWS AI Agent Global Hackathon – Đây là cơ hội để bạn khám phá sâu vào bộ công cụ AI sinh tạo mạnh mẽ của chúng tôi và tạo ra một thứ gì đó thực sự tuyệt vời. Từ ngày 8 tháng 9 đến ngày 20 tháng 10, bạn có cơ hội tạo ra các tác nhân AI bằng bộ dịch vụ AI của AWS, cạnh tranh để giành hơn 45.000 USD tiền thưởng và các cơ hội tiếp cận thị trường độc quyền.

● AWS Gen AI Lofts – Bạn có thể tìm hiểu về các sản phẩm và dịch vụ AI của AWS với các phiên độc quyền, gặp gỡ các chuyên gia hàng đầu trong ngành, và có cơ hội kết nối giá trị với các nhà đầu tư và đồng nghiệp. Đăng ký tại thành phố gần bạn nhất: Mexico City (30 tháng 9 – 2 tháng 10), Paris (7–21 tháng 10), London (13–21 tháng 10), và Tel Aviv (11–19 tháng 11).

● AWS Community Days – Tham gia các hội nghị do cộng đồng dẫn dắt với các buổi thảo luận kỹ thuật, hội thảo, và các phòng thí nghiệm thực hành do các chuyên gia AWS và các nhà lãnh đạo ngành từ khắp nơi trên thế giới dẫn dắt: Nam Phi (20 tháng 9), Bolivia (20 tháng 9), Bồ Đào Nha (27 tháng 9), và Manila (4–5 tháng 10).

Bạn có thể xem tất cả các sự kiện AWS sắp tới và các sự kiện khởi nghiệp AWS.

Đó là tất cả cho tuần này. Hãy kiểm tra lại vào thứ Hai tới để đọc một Bản tin Hàng tuần khác!

Chúc bạn xây dựng vui vẻ!

— Donnie

THẺ: Week in Review

## Tác Giả

Donnie Prakoso  
Donnie Prakoso là một kỹ sư phần mềm, tự xưng là barista, và là Principal Developer Advocate tại AWS. Với hơn 17 năm kinh nghiệm trong ngành công nghệ, từ viễn thông, ngân hàng đến các công ty khởi nghiệp. Hiện tại, anh tập trung vào việc giúp các nhà phát triển hiểu về nhiều công nghệ khác nhau để biến ý tưởng của họ thành hiện thực. Anh yêu thích cà phê và bất kỳ cuộc thảo luận nào về bất kỳ chủ đề nào từ microservices đến AI/ML.
