### Production Deployment TODO

File này ghi lại các việc cần hoàn thiện trước khi deploy website lên production.

## 1. Trạng thái page hiện tại

### Đã triển khai

```text
✅ index.html
✅ services.html
✅ industries.html
✅ success-stories.html
✅ about.html
✅ resources.html
✅ contact.html
✅ WEBSITE_PRESENTATION.md
```

### Chưa triển khai — page chi tiết cấp 2

Các trang này chưa bắt buộc cho MVP, nhưng nên làm nếu muốn website chuyên nghiệp/SEO tốt hơn.

```text
❌ services/cloud-migration.html
❌ services/managed-cloud-services.html
❌ services/devops-automation.html
❌ services/cloud-security.html
❌ services/data-analytics.html
❌ services/generative-ai-on-aws.html
❌ services/finops-cost-optimization.html
❌ services/well-architected-review.html

❌ industries/financial-services.html
❌ industries/retail-ecommerce.html
❌ industries/manufacturing.html
❌ industries/healthcare.html
❌ industries/education.html
❌ industries/saas-startup.html

❌ success-stories/case-study-1.html
❌ success-stories/case-study-2.html
❌ success-stories/case-study-3.html
```

---

## 2. Việc bắt buộc trước khi deploy production

### Brand / công ty

```text
[ ] Thay tên CloudNexus bằng tên công ty thật
[ ] Thay logo placeholder CN bằng logo thật
[ ] Thay tagline / brand promise thật
[ ] Thay email placeholder hello@cloudnexus.example
[ ] Thêm số điện thoại thật
[ ] Thêm địa chỉ công ty nếu có
[ ] Thêm social links thật: LinkedIn, Facebook, YouTube, v.v.
```

### AWS Partner / chứng nhận

```text
[ ] Xác minh AWS Partner tier thật
[ ] Xác minh quyền sử dụng AWS Partner badge/logo
[ ] Thêm chứng chỉ AWS thật
[ ] Thêm AWS competencies nếu có
[ ] Thêm AWS service delivery validations nếu có
[ ] Xóa hoặc sửa mọi claim chưa xác minh
```

### Nội dung dịch vụ

```text
[ ] Rà soát danh sách service có đúng năng lực thật không
[ ] Viết lại mô tả từng service theo offering thật
[ ] Xác định service core cần ưu tiên bán
[ ] Xác định package nếu có: Assessment, Migration, Managed Services, FinOps, GenAI Workshop
[ ] Thêm deliverables cụ thể cho từng service
[ ] Thêm công nghệ/AWS services sử dụng thật
```

### Case study / khách hàng

```text
[ ] Thay case study mẫu bằng case study thật
[ ] Xin quyền dùng logo/tên khách hàng nếu cần
[ ] Nếu không được public tên khách hàng, viết case dạng ẩn danh
[ ] Thêm challenge, solution, impact thật
[ ] Thêm số liệu thật, không dùng số bịa
[ ] Thêm testimonial thật nếu có
```

### Metrics / số liệu

```text
[ ] Thay các số liệu placeholder bằng số liệu đã xác minh
[ ] Số dự án cloud đã triển khai
[ ] Số khách hàng đã phục vụ
[ ] Số workload đã migration
[ ] Số chứng chỉ AWS
[ ] Số năm kinh nghiệm
[ ] SLA thật nếu có managed services
```

### Industries

```text
[ ] Chỉ giữ những ngành công ty có kinh nghiệm thật
[ ] Viết lại pain point theo từng ngành
[ ] Thêm use case thật theo từng ngành
[ ] Gắn case study tương ứng nếu có
```

### Resources / blog

```text
[ ] Viết bài blog thật hoặc bỏ link chưa có nội dung
[ ] Tạo ít nhất 3 bài nền tảng trước khi launch nếu muốn có Resources page
[ ] Chuẩn bị checklist/whitepaper nếu dùng làm lead magnet
[ ] Thêm ảnh thumbnail hoặc visual system cho bài viết
```

### Contact form

```text
[ ] Nối form với email hoặc CRM
[ ] Thêm validation frontend/backend
[ ] Thêm spam protection
[ ] Thêm privacy consent checkbox
[ ] Tạo thank-you message hoặc thank-you page
[ ] Test submit form thật
[ ] Mapping field form với sales pipeline
```

### SEO / metadata

```text
[ ] Viết lại title từng trang
[ ] Viết lại meta description từng trang
[ ] Thêm Open Graph image thật
[ ] Thêm favicon/logo đúng brand
[ ] Kiểm tra heading H1/H2 từng trang
[ ] Tạo sitemap.xml
[ ] Tạo robots.txt production
[ ] Kiểm tra canonical URL nếu cần
```

### Legal / compliance

```text
[ ] Thêm Privacy Policy
[ ] Thêm Terms & Conditions nếu cần
[ ] Kiểm tra quyền dùng logo AWS
[ ] Kiểm tra quyền dùng logo khách hàng
[ ] Kiểm tra claim về uptime/SLA/cost saving
[ ] Kiểm tra nội dung không vi phạm chính sách AWS brand usage
```

### Tracking / analytics

```text
[ ] Gắn Google Analytics / Plausible / công cụ analytics
[ ] Gắn conversion tracking cho form submit
[ ] Gắn event tracking cho CTA chính
[ ] Gắn tracking cho download tài liệu nếu có
```

### Technical deployment

```text
[ ] Chạy npm install nếu dùng build pipeline hiện tại
[ ] Chạy npm run build thành công
[ ] Kiểm tra HTML/CSS/JS trên production-like server
[ ] Kiểm tra responsive desktop/tablet/mobile
[ ] Kiểm tra mobile menu
[ ] Kiểm tra tất cả link nav/footer
[ ] Kiểm tra lỗi console browser
[ ] Tối ưu performance nếu cần
[ ] Tối ưu ảnh/logo nếu thêm asset thật
[ ] Kiểm tra HTTPS/domain
```

---

## 3. Ưu tiên triển khai đề xuất

### Phase 1 — MVP production

Làm trước khi public website.

```text
1. Thay brand thật
2. Thay contact thật
3. Rà soát service thật
4. Xóa/sửa mọi claim chưa xác minh
5. Nối contact form
6. SEO metadata cơ bản
7. Kiểm tra responsive và link
8. Deploy production
```

### Phase 2 — Trust upgrade

Làm sau MVP để tăng độ tin cậy.

```text
1. Thêm AWS badge/chứng chỉ hợp lệ
2. Thêm case study thật
3. Thêm testimonial thật
4. Thêm số liệu năng lực thật
5. Viết lại About theo câu chuyện công ty thật
```

### Phase 3 — SEO / growth

Làm khi muốn phát triển traffic và lead.

```text
1. Tạo service detail pages
2. Tạo industry detail pages
3. Tạo blog/resources thật
4. Tạo downloadable checklist/whitepaper
5. Tối ưu schema/SEO nâng cao
```

---

## 4. Ghi chú quan trọng

Hiện website là bản prototype/marketing foundation. Các phần sau đang là placeholder và không nên deploy nguyên trạng nếu chưa chỉnh:

```text
CloudNexus
CN logo
AWS Partner Placeholder
hello@cloudnexus.example
Case study mẫu
Metrics dạng target/capability
Resources chưa có bài thật
Contact form static
```

Trước khi production, ưu tiên quan trọng nhất là thay bằng:

```text
Tên thật
Logo thật
Chứng nhận thật
Case thật
Số liệu thật
Form hoạt động thật
Thông tin liên hệ thật
```
