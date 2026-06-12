# CloudNexus AWS Partner Website — Presentation & Production Brief

## 1. Mục tiêu của website

Website này được thiết kế như một nền tảng giới thiệu chuyên nghiệp cho một công ty là **AWS Partner / Cloud Consulting Partner**.

Mục tiêu chính:

1. **Tạo niềm tin nhanh với khách hàng doanh nghiệp**  
   Thể hiện công ty có năng lực tư vấn, triển khai, vận hành và tối ưu hệ thống cloud trên AWS.

2. **Định vị công ty là đối tác chuyển đổi cloud end-to-end**  
   Không chỉ bán dịch vụ kỹ thuật đơn lẻ, mà đồng hành từ chiến lược, migration, modernization, security, managed services, FinOps đến GenAI/Data.

3. **Thu hút lead chất lượng**  
   Các CTA như `Book a Cloud Consultation`, `Tư vấn Cloud miễn phí`, `Nhận tư vấn dịch vụ` được đặt xuyên suốt để hướng khách hàng về trang contact.

4. **Tạo cảm giác enterprise-grade**  
   Bố cục, màu sắc, typography và nội dung được xây theo hướng chuyên nghiệp, phù hợp khách hàng B2B/enterprise.

5. **Có cấu trúc mở rộng về sau**  
   Website hiện đã có homepage và các subpage chính, đủ nền để phát triển thêm landing page riêng cho từng dịch vụ, ngành hoặc case study.

---

## 2. Cơ sở tham khảo

Website được định hướng từ các site AWS/cloud partner sau:

- `https://www.ecloudvalley.com/vn/`
- `https://renovacloud.com/en/`
- `https://www.cloud-kinetics.com/`

Các pattern chính được học từ những site này:

- Có hero mạnh, thể hiện rõ năng lực cloud/AWS.
- Có menu rõ: Services, Industries, Success Stories, Resources, About, Contact.
- Nhấn mạnh trust signals: AWS Partner, certifications, cloud experts, managed services, competencies.
- Có success stories/case studies để chứng minh năng lực.
- Có các dịch vụ trending: GenAI, Data & Analytics, FinOps, DevOps, Security.
- Có CTA tư vấn ở nhiều vị trí.
- Bố cục chuyên nghiệp, enterprise, không quá startup/sloppy.

---

## 3. Lý do chọn bố cục hiện tại

### 3.1 Homepage

Homepage được thiết kế như một **executive landing page** cho khách hàng lần đầu vào website.

Luồng nội dung:

```text
Hero
→ Trust signals
→ Pain points
→ Services overview
→ Transformation framework
→ Industries
→ Success story samples
→ Vision / Mission
→ Resources
→ Contact CTA
```

Lý do:

- Khách hàng cần hiểu ngay công ty làm gì.
- Sau đó cần thấy công ty hiểu vấn đề của họ.
- Tiếp theo mới giới thiệu dịch vụ.
- Cuối cùng tạo niềm tin bằng framework, ngành, case study và CTA.

### 3.2 Services page

Trang `services.html` dùng để trình bày đầy đủ năng lực dịch vụ.

Các service lines hiện có:

1. AWS Cloud Migration
2. Managed Cloud Services
3. DevOps & Automation
4. Cloud Security
5. Data & Analytics
6. Generative AI on AWS
7. FinOps / Cost Optimization
8. Well-Architected Review

Lý do:

- Đây là portfolio chuẩn của một AWS/cloud partner hiện đại.
- Bao phủ cả migration, vận hành, security, cost và innovation.
- Có thể tách mỗi service thành landing page riêng khi triển khai production.

### 3.3 Industries page

Trang `industries.html` cho thấy công ty không chỉ biết công nghệ, mà hiểu từng bối cảnh ngành.

Các ngành hiện có:

- Financial Services
- Retail & E-commerce
- Manufacturing
- Healthcare
- Education
- SaaS / Startup

Lý do:

- Khách enterprise thường mua theo pain point ngành.
- Trang ngành giúp tăng độ tin cậy và SEO.
- Dễ dẫn khách từ ngành sang dịch vụ phù hợp.

### 3.4 Success Stories page

Trang `success-stories.html` hiện dùng các case study mẫu, chưa bịa tên khách hàng thật.

Lý do:

- Case study là bằng chứng bán hàng mạnh nhất.
- Tuy nhiên ở bản prototype không nên bịa logo, khách hàng hoặc số liệu.
- Khi production cần thay bằng dữ liệu thật.

Case study nên theo format:

```text
Context → Challenge → Solution → Outcome
```

### 3.5 About page

Trang `about.html` tập trung vào:

- Vision
- Mission
- Brand promise
- Team capability
- Delivery principles

Lý do:

- Khách hàng B2B cần biết đội ngũ có phương pháp hay không.
- Không chỉ nói “chúng tôi chuyên nghiệp”, mà cần thể hiện bằng nguyên tắc làm việc.

### 3.6 Resources page

Trang `resources.html` tạo nền cho blog/insights.

Lý do:

- Tăng trust trước khi khách để lại lead.
- Hỗ trợ SEO.
- Cho thấy công ty có chuyên môn thật.
- Có thể dùng để nuôi lead qua bài viết, checklist, guide, event.

### 3.7 Contact page

Trang `contact.html` được thiết kế như entry point tư vấn cloud.

Lý do:

- Không chỉ là form liên hệ chung.
- Form hỏi rõ nhu cầu cloud, quy mô workload, service quan tâm.
- Dễ nối CRM/email khi production.

---

## 4. Sitemap hiện tại

```text
CloudNexus Website
│
├── index.html
│   ├── Hero
│   ├── Trust Signals
│   ├── Pain Points
│   ├── Services Overview
│   ├── Transformation Framework
│   ├── Industries Overview
│   ├── Success Story Samples
│   ├── Vision / Mission
│   ├── Resources Preview
│   └── Contact CTA
│
├── services.html
│   ├── AWS Cloud Migration
│   ├── Managed Cloud Services
│   ├── DevOps & Automation
│   ├── Cloud Security
│   ├── Data & Analytics
│   ├── Generative AI on AWS
│   ├── FinOps / Cost Optimization
│   └── Well-Architected Review
│
├── industries.html
│   ├── Financial Services
│   ├── Retail & E-commerce
│   ├── Manufacturing
│   ├── Healthcare
│   ├── Education
│   └── SaaS / Startup
│
├── success-stories.html
│   ├── Featured Case Study Template
│   ├── GenAI / Retail Sample
│   ├── FinOps Sample
│   ├── Disaster Recovery Sample
│   ├── Data Platform Sample
│   ├── DevOps Sample
│   └── Well-Architected Sample
│
├── about.html
│   ├── Vision
│   ├── Mission
│   ├── Brand Promise
│   ├── Team Capability
│   └── Delivery Principles
│
├── resources.html
│   ├── Featured Guide
│   ├── Migration Articles
│   ├── Architecture Articles
│   ├── FinOps Articles
│   ├── GenAI Articles
│   ├── Security Articles
│   └── Data Articles
│
└── contact.html
    ├── Consultation Intro
    ├── What Happens Next
    ├── Contact Points
    └── Lead Form
```

---

## 5. Sitemap đề xuất khi triển khai production

Khi công ty có đủ nội dung thật, nên mở rộng thành:

```text
/
├── /services/
│   ├── /cloud-migration/
│   ├── /managed-cloud-services/
│   ├── /devops-automation/
│   ├── /cloud-security/
│   ├── /data-analytics/
│   ├── /generative-ai-on-aws/
│   ├── /finops-cost-optimization/
│   └── /well-architected-review/
│
├── /industries/
│   ├── /financial-services/
│   ├── /retail-ecommerce/
│   ├── /manufacturing/
│   ├── /healthcare/
│   ├── /education/
│   └── /saas-startup/
│
├── /success-stories/
│   ├── /case-study-1/
│   ├── /case-study-2/
│   └── /case-study-3/
│
├── /resources/
│   ├── /blog/
│   ├── /events/
│   ├── /whitepapers/
│   └── /aws-insights/
│
├── /about/
│   ├── /company/
│   ├── /leadership/
│   ├── /certifications/
│   ├── /partners/
│   └── /careers/
│
└── /contact/
```

---

## 6. Các nội dung cần chỉnh theo thực tế công ty

### 6.1 Brand identity

Hiện tại đang dùng placeholder:

```text
CloudNexus
CN logo mark
AWS Partner
```

Cần thay bằng:

- Tên công ty thật.
- Logo thật.
- Brand color thật.
- Font/VI nếu có.
- Tagline thật.
- Địa chỉ, email, số điện thoại thật.
- Social links thật.

### 6.2 AWS Partner status

Hiện tại có text placeholder:

```text
AWS Partner Placeholder
Certified Cloud Experts
Well-Architected Practice
CloudOps 24/7
FinOps Ready
GenAI on AWS
```

Cần xác minh và thay bằng thông tin thật:

- AWS Partner tier.
- AWS certifications.
- AWS competencies.
- AWS service delivery validations.
- AWS awards nếu có.
- Số lượng chứng chỉ AWS.
- Số lượng engineer certified.

Không nên hiển thị badge AWS nếu chưa có quyền sử dụng hoặc chưa được xác minh.

### 6.3 Metrics / số liệu

Hiện tại các số như `99.9% target uptime`, `24/7 managed ops` là capability/target, không phải claim thực tế.

Production cần thay bằng số liệu thật:

- Số dự án cloud đã triển khai.
- Số khách hàng.
- Số workload đã migrate.
- Số chứng chỉ AWS.
- Số năm kinh nghiệm.
- Mức tiết kiệm chi phí trung bình nếu có dữ liệu.
- SLA managed services nếu có hợp đồng rõ.

### 6.4 Case studies

Hiện đang là mẫu case study.

Production cần nhập:

- Tên khách hàng hoặc mô tả ẩn danh được phép công bố.
- Ngành.
- Vấn đề ban đầu.
- Kiến trúc/giải pháp AWS.
- Services đã dùng.
- Kết quả đo được.
- Quote/testimonial nếu có.
- Logo khách hàng nếu được phép.

Format đề xuất:

```text
Client / Industry
Challenge
Solution
AWS Services Used
Business Impact
Technical Impact
Testimonial
```

### 6.5 Services

Các dịch vụ hiện đang là portfolio chuẩn. Khi production cần xác định công ty thực sự mạnh nhất ở đâu.

Cần chỉnh:

- Dịch vụ nào là core.
- Dịch vụ nào là add-on.
- Dịch vụ nào chưa nên public.
- Mô tả service theo năng lực thực tế.
- Quy trình delivery thật.
- Công cụ/platform nội bộ nếu có.
- Package hoặc offering cụ thể nếu muốn bán nhanh.

Ví dụ:

```text
Cloud Migration Assessment Package
AWS Landing Zone Setup
Managed Services Starter / Standard / Enterprise
FinOps Monthly Optimization
Well-Architected Review Sprint
GenAI Discovery Workshop
```

### 6.6 Industries

Các ngành hiện là đề xuất phổ biến.

Production nên giữ những ngành công ty có kinh nghiệm thật.

Cần nhập:

- Ngành đã từng phục vụ.
- Pain point thật của ngành.
- Use case thật.
- Case study tương ứng.
- Compliance hoặc tiêu chuẩn ngành nếu có.

### 6.7 Resources

Hiện đang là danh sách bài viết đề xuất.

Cần sản xuất nội dung thật:

- Blog post.
- Whitepaper.
- Checklist.
- Webinar/event.
- AWS insight.
- Technical guide.

Nên ưu tiên các bài có khả năng tạo lead:

- Cloud Migration Readiness Checklist.
- AWS Cost Optimization Checklist.
- Well-Architected Review Guide.
- GenAI Use Cases for Enterprise.
- Cloud Security Baseline Before Go-live.

### 6.8 Contact form

Hiện form là static prototype.

Production cần:

- Nối email/CRM.
- Validation.
- Spam protection.
- Privacy consent.
- Thank-you page.
- Tracking conversion.
- Field mapping với sales pipeline.

---

## 7. Các component cần nhập liệu / chỉnh sửa khi production

### Global components

| Component | File hiện tại | Cần nhập/chỉnh |
|---|---|---|
| Header / Navigation | Tất cả HTML | Logo thật, link thật, active state |
| Footer | Tất cả HTML | Địa chỉ, email, social, legal links |
| CTA Button | Tất cả HTML | Text CTA theo sales strategy |
| Brand Mark | Tất cả HTML | Thay `CN` bằng logo SVG/PNG |
| SEO Meta | Tất cả HTML | Title, description, OG image thật |

### Homepage components

| Component | Cần nhập/chỉnh |
|---|---|
| Hero headline | Thông điệp định vị thật của công ty |
| Hero subcopy | Dịch vụ và thị trường mục tiêu thật |
| Trust strip | AWS badge/chứng chỉ/số liệu thật |
| Pain points | Pain point theo khách hàng mục tiêu |
| Service overview | Dịch vụ core đã xác nhận |
| Framework | Quy trình delivery thật |
| Case samples | Case study thật |
| Vision/Mission | Nội dung brand thật |

### Services components

| Component | Cần nhập/chỉnh |
|---|---|
| Service cards | Tên service, scope, deliverables thật |
| Delivery model | Quy trình tư vấn/triển khai thật |
| Service CTA | CTA theo từng package |
| AWS services used | Danh sách AWS services thật nếu làm page chi tiết |

### Industries components

| Component | Cần nhập/chỉnh |
|---|---|
| Industry cards | Chỉ giữ ngành công ty có kinh nghiệm |
| Use cases | Use case thật |
| Industry proof | Case study/logo khách hàng theo ngành |

### Success Stories components

| Component | Cần nhập/chỉnh |
|---|---|
| Featured case | Case thật nổi bật nhất |
| Case cards | Tối thiểu 3 case thật hoặc ẩn danh |
| Metrics | Số liệu có thể xác minh |
| Testimonials | Quote được khách hàng cho phép |

### About components

| Component | Cần nhập/chỉnh |
|---|---|
| Vision | Vision thật |
| Mission | Mission thật |
| Team capability | Số lượng/team thật |
| Leadership | Ảnh/tên/chức danh nếu có |
| Certifications | Chứng chỉ thật |

### Resources components

| Component | Cần nhập/chỉnh |
|---|---|
| Featured guide | File PDF/checklist thật |
| Blog cards | Bài viết thật |
| Category | Migration, Security, FinOps, GenAI, Data |
| Lead magnet | Form tải tài liệu nếu cần |

### Contact components

| Component | Cần nhập/chỉnh |
|---|---|
| Contact info | Email, phone, address thật |
| Form fields | Theo CRM/sales process |
| Service options | Theo service thật |
| Privacy consent | Chính sách bảo mật |
| Submission action | API/email/CRM integration |

---

## 8. Text cần sửa lại cho phù hợp công ty

Các cụm đang là placeholder hoặc generic:

```text
CloudNexus
AWS Partner
Cloud transformation without complexity
AWS Cloud delivered with clarity
AWS Partner Placeholder
Certified Cloud Experts
CloudOps 24/7
Vietnam & ASEAN-ready delivery
hello@cloudnexus.example
```

Cần thay bằng:

- Tên công ty thật.
- Tagline thật.
- Mô tả năng lực thật.
- Email domain thật.
- Thị trường phục vụ thật.
- Chứng nhận AWS thật.
- Dịch vụ thật.

---

## 9. Production checklist

Trước khi đưa website lên production:

```text
[ ] Thay logo và brand asset thật
[ ] Xác minh AWS Partner status / badge usage
[ ] Thay toàn bộ placeholder metrics bằng số liệu thật
[ ] Thay case study mẫu bằng case thật hoặc ẩn danh hợp pháp
[ ] Rà soát service portfolio theo năng lực thật
[ ] Rà soát industries theo khách hàng thật
[ ] Viết lại SEO title/description từng trang
[ ] Thêm OG image/social sharing image
[ ] Nối contact form với email/CRM
[ ] Thêm privacy policy / terms nếu cần
[ ] Gắn analytics/conversion tracking
[ ] Kiểm tra responsive desktop/tablet/mobile
[ ] Kiểm tra performance/accessibility cơ bản
[ ] Kiểm tra legal/compliance về logo AWS và khách hàng
```

---

## 10. File hiện có trong prototype

```text
index.html
services.html
industries.html
success-stories.html
about.html
resources.html
contact.html
css/style.css
js/app.js
```

Các screenshot responsive đã tạo trong quá trình kiểm tra:

```text
cloudnexus-desktop.png
cloudnexus-tablet.png
cloudnexus-mobile.png
services-desktop.png
services-mobile.png
contact-mobile.png
about-tablet.png
```

---

## 11. Kết luận để present

Website này được thiết kế để giúp công ty xuất hiện như một **AWS/cloud transformation partner chuyên nghiệp**, có khả năng đồng hành với khách hàng doanh nghiệp từ chiến lược đến triển khai và vận hành.

Cấu trúc hiện tại ưu tiên:

- Niềm tin.
- Rõ dịch vụ.
- Rõ ngành.
- Rõ case study.
- Rõ đội ngũ/phương pháp.
- Rõ đường chuyển đổi thành lead.

Khi triển khai production, việc quan trọng nhất không phải thêm hiệu ứng, mà là thay toàn bộ placeholder bằng **dữ liệu thật, case thật, chứng nhận thật và thông điệp thương hiệu thật**.
