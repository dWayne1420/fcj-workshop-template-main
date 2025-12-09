---
title: "Xây dựng các dịch vụ đám mây công cộng kiên cường: Tại sao đã đến lúc cập nhật chiến lược của bạn"
date: 2025-09-22
draft: false
---

AWS Public Sector Blog  
Xây dựng các dịch vụ đám mây công cộng kiên cường: Tại sao đã đến lúc cập nhật chiến lược của bạn  
bởi Jeff Kratz | 22 tháng 9 năm 2025 | tại Best Practices, Public Sector, Resilience | Permalink 

Khách hàng trong khu vực công của chúng tôi dựa vào tính kiên cường (resilience) của Amazon Web Services (AWS) Cloud để có thể hoàn thành các sứ mệnh quan trọng của họ. Trước những rủi ro ngày càng tăng của các cuộc tấn công mạng (cyberattacks), các mối đe dọa môi trường như lũ lụt hoặc động đất, và các rủi ro vật lý như lỗi thiết bị (equipment failures), các nhà lãnh đạo khu vực công có một công việc ngày càng phức tạp. Tuy nhiên, người dân kỳ vọng các dịch vụ chính phủ như bầu cử hoặc gia hạn hộ chiếu phải hoạt động hiệu quả và đáng tin cậy như các nền tảng thương mại trực tuyến mà họ sử dụng.

Các chính phủ và các ngành chịu sự quản lý như dịch vụ tài chính vận hành các dịch vụ số thiết yếu, chẳng hạn như ngân hàng hoặc các nền tảng thuế số (digital tax platforms). Những dịch vụ này là một phần cơ bản trong cuộc sống của chúng ta, và chúng cần phải tiếp tục hoạt động hoặc khôi phục sau các sự cố gián đoạn—một đặc tính được gọi là resilience (tính kiên cường). Ngoài ra, chúng phải duy trì hoạt động với thời gian ngừng hoạt động tối thiểu, trạng thái mà chúng tôi gọi là high availability (tính sẵn sàng cao).

Trong lịch sử, tính kiên cường của các dịch vụ này chủ yếu phụ thuộc vào cơ sở hạ tầng vật lý. Trước khi có đám mây, để tăng tính kiên cường cho ứng dụng, bạn sẽ thêm một giá đỡ (rack) khác trong một trung tâm dữ liệu (data center) khác, và để cải thiện hơn nữa, bạn sẽ sử dụng một trung tâm dữ liệu cách xa hàng chục hoặc hàng trăm kilomet.

Nhưng giờ đây, tính kiên cường không chỉ đơn thuần là cơ sở hạ tầng. Cách các tổ chức xây dựng ứng dụng đang thay đổi không ngừng; cũng giống như bảo mật (security) là một trách nhiệm chung (shared responsibility), tính kiên cường cũng vậy. Điều quan trọng là các tổ chức cần tìm hiểu về các công cụ và kỹ thuật giúp họ xây dựng và quản lý các ứng dụng đám mây kiên cường và hiểu cách duy trì các dịch vụ kiên cường nhất cho cộng đồng mà họ phục vụ.

## Xây dựng văn hóa vận hành kiên cường

Để trả lời các câu hỏi này, AWS Principal Technologist Rob Charlton và đội ngũ Public Sector Industries đã tạo ra một loạt video chia sẻ lý do tại sao các cách tiếp cận truyền thống đối với tính kiên cường của dịch vụ số cần được cập nhật để tận dụng tối đa tính kiên cường mà đám mây mang lại.

Trong loạt video gồm tám phần, được xem như một resilience playbook (sổ tay về tính kiên cường), Rob đưa người xem qua quá trình phát triển từ tính kiên cường tập trung vào cơ sở hạ tầng truyền thống đến cách tiếp cận toàn diện ngày nay, bao gồm microservices (dịch vụ vi mô), cơ sở hạ tầng, giám sát (monitoring), và sự xuất sắc trong vận hành (operational excellence).

**Building Resilient Cloud Services (Part 1): A modern approach | Amazon Web Services**

Trong tập một, Rob giới thiệu Resilience Equation (Phương trình Kiên cường), một khung công tác cho thấy cách cơ sở hạ tầng nền tảng của AWS kết hợp với kiến trúc ứng dụng (application architecture), thiết kế phần mềm (software design), và hoạt động (operations) để tạo ra các dịch vụ thực sự kiên cường. Thông qua các hình ảnh trực quan rõ ràng và các ví dụ thực tế, Rob khám phá cách các kiến trúc ứng dụng hiện đại đã thay đổi mô hình thất bại (failure patterns), cũng như mô hình trách nhiệm chung (shared responsibility model) về tính kiên cường giữa AWS và khách hàng.

Tiếp tục trong tập hai, Rob đi sâu vào cách mô hình lồng ghép toàn cầu độc đáo của cơ sở hạ tầng AWS—bao gồm các trung tâm dữ liệu (data centers), Availability Zones (Vùng sẵn sàng), và Regions (Khu vực)—là nền tảng cho các dịch vụ số kiên cường.

Trong tập ba, Rob cùng với Senior Principal Security Solutions Architect Stephen “Squigg” Quigg đi sâu hơn vào cách AWS thiết kế các trung tâm dữ liệu với tư duy “chấp nhận thất bại” (embrace failure mindset)—sử dụng phần cứng được thiết kế riêng (purpose-built hardware), mã hóa lại phần mềm (re-coding software), và các biện pháp bảo mật chặt chẽ. Từ phân phối nguồn điện (power distribution) đến dự phòng mạng (networking redundancy), mọi khía cạnh được thiết kế để tối đa hóa tính kiên cường trong khi nâng cao hiệu suất.

**Building Resilient Cloud Services (Part 4): Why multi–Availability Zone applications?**

Loạt video tiếp tục với việc khám phá các dịch vụ cụ thể của AWS, với Rob hướng dẫn người xem qua các mô hình triển khai (deployment models) của các dịch vụ AWS cụ thể, nhấn mạnh cách các lựa chọn kiến trúc này ảnh hưởng đến tính kiên cường và tính sẵn sàng của các ứng dụng khu vực công.

Trong tập bốn, Rob quay lại với cơ sở hạ tầng để giải thích cách chuyển ứng dụng tại chỗ (on-premises application) sang đám mây giúp giảm thiểu các rủi ro lớn nhất, trước khi chuyển sang các đội ngũ đứng sau các dịch vụ AWS, một số thực tiễn vận hành của họ, và cách họ triển khai các bản cập nhật trong tập năm. Loạt video kết thúc với các cuộc thảo luận về dịch vụ và giám sát (monitoring). Với các mẹo cụ thể xuyên suốt, loạt video kết thúc bằng một loạt các thực tiễn tốt nhất (best practices) để xây dựng các ứng dụng đám mây kiên cường trong khu vực công.

**Building Resilient Cloud Services 8: Building resilient applications on AWS**

## Kết luận

Dù bạn đang hoạt động trong lĩnh vực dịch vụ tài chính, chính phủ liên bang, tiểu bang, địa phương, hay bất kỳ ngành nào yêu cầu các dịch vụ có tính sẵn sàng cao (highly available services), loạt video này sẽ cho bạn thấy cách cơ sở hạ tầng toàn cầu, thiết kế dịch vụ, và các thực tiễn vận hành của AWS có thể tạo ra nền tảng kiên cường cho các khối lượng công việc quan trọng nhất của bạn.

Xem toàn bộ loạt video tại đây, và đọc thêm về tính kiên cường của AWS Cloud tại đây.

THẺ: AWS Public Sector, best practices, resiliency

## Tác Giả

**Jeff Kratz**  
Jeff dẫn dắt các hoạt động kinh doanh của AWS Worldwide Public Sector Industry và Nonprofit, phục vụ các tổ chức chính phủ, giáo dục, y tế công cộng, và phi lợi nhuận. Jeff định hướng việc tạo ra, hiện đại hóa, và thực hiện các giải pháp đám mây quan trọng đối với sứ mệnh (mission-critical cloud solutions) ảnh hưởng đến hàng triệu người trên toàn cầu.
