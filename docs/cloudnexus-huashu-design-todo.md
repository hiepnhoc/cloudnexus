# CloudNexus AWS Partner Website — Huashu-Design Improvement Brief

> Mục tiêu: biến trang `https://hiepnhoc.github.io/cloudnexus/` từ một AWS/SaaS landing page concept thành một website AWS Partner có visual direction rõ ràng theo tinh thần `huashu-design`: có chủ đích, tránh generic AI-slop, lấy nội dung/dẫn chứng làm trung tâm, và có một visual signature đủ mạnh.

## 0. Implementation status — 2026-06-12

### Đã triển khai trong source

- [x] Xóa placeholder/internal copy khỏi UI HTML (`Placeholder`, `Mẫu`, `concept`, `Replace`, `static prototype`, `hello@cloudnexus.example`).
- [x] Softening AWS claim: UI chuyển từ claim trực tiếp `AWS Partner` sang `AWS-focused Cloud` / `AWS-focused cloud consulting` để an toàn khi chưa có partner tier xác thực.
- [x] Navigation và CTA chuyển theo hướng Vietnam-first: `Trang chủ`, `Dịch vụ`, `Ngành`, `Câu chuyện khách hàng`, `Về CloudNexus`, `Tài nguyên`, `Đặt lịch tư vấn`.
- [x] Hero visual chuyển thành AWS Operating Model Diagram có flow `Assess → Foundation → Migrate → Secure → Optimize → Operate`.
- [x] Homepage Services chuyển từ card list sang `CloudNexus AWS Capability System` theo layer: Foundation, Migration, Operate, Optimize, Data & AI.
- [x] Framework section chuyển thành `The CloudNexus AWS Operating Model` với 6 bước có arrow/process visual.
- [x] Success Stories chuyển thành customer-facing `Representative engagement` / `Anonymized blueprint`, không dùng từ `Mẫu case study` trên UI.
- [x] Footer production-safe hơn, có mô tả công ty và AWS trademark disclaimer.
- [x] QA text trên `*.html`: không còn các từ khóa placeholder/internal copy nêu trong checklist.
- [x] `node --check js/app.js` pass.
- [x] Đã chụp lại desktop 1440×1200 và mobile 390×1200 cho homepage sau thay đổi.

### Còn cần business input trước production thật

- [ ] Xác nhận AWS Partner tier / AWS Partner profile / quyền dùng badge chính thức nếu muốn claim `AWS Partner`.
- [ ] Thay `CloudNexus` / logo `CN` / email `contact@cloudnexus.vn` bằng brand asset và contact thật.
- [ ] Bổ sung số liệu thật: số project, số chứng chỉ, số workload migrate, SLA nếu có.
- [ ] Thay representative engagement bằng case study thật hoặc anonymized story đã được xác nhận.
- [ ] Nối contact form với backend/email/CRM và privacy consent.

### Ghi chú

Các mục bên dưới được giữ lại làm design rationale và checklist tham chiếu. Một số mục P0/P1 đã được xử lý trong source, nhưng vẫn cần rà soát lại sau khi có dữ liệu business thật.

## 1. Context hiện tại

CloudNexus đang được định vị là website cho một đơn vị AWS Partner / AWS-focused cloud consulting.

Reference tham khảo:

- https://www.ecloudvalley.com/vn/
- https://renovacloud.com/en/
- https://www.cloud-kinetics.com/
- https://www.techxcorp.com/

Trang hiện tại đã có các section chính:

- Hero
- Trust strip
- Why Change / Pain points
- Services
- Framework
- Industries
- Success Stories
- About
- Resources
- Contact
- Footer

## 2. Đánh giá nhanh

### Đang đúng

- Nội dung tổng thể đúng hướng AWS Partner / cloud transformation.
- Hero có positioning rõ: AWS Cloud Transformation, Migration, Security, FinOps, GenAI, Managed Ops.
- Service taxonomy đúng nhóm dịch vụ AWS partner thường có.
- Visual polish ổn: dark navy, orange accent, card layout, CTA rõ.
- Page structure đủ khung để phát triển thành landing page production.

### Chưa đạt theo huashu-design

Trang hiện tại vẫn hơi giống generic SaaS/AWS landing page do AI tạo:

- Dark gradient + rounded cards + pill badges + abstract dashboard hơi phổ biến.
- Chưa có một visual signature thật sự riêng.
- Dịch vụ đang là list card, chưa thành một capability system / operating model rõ.
- Case study còn copy nội bộ/placeholder.
- Trust proof chưa đủ mạnh so với các AWS Partner reference.
- Một số section có spacing rộng, cảm giác chưa chặt.
- Language đang lẫn English/Vietnamese, cần chủ ý rõ hơn.

## 3. Design direction đề xuất

Không đổi business sang Huawei. Mục tiêu là dùng tinh thần `huashu-design` cho website AWS Partner.

### Direction chính

**Diagram-driven enterprise consulting style**

Mix đề xuất:

- 60% `Diagram-Driven Isotype`: dùng operating model, architecture map, capability system, arrow flow, layered diagrams.
- 25% `Two-Font Consulting`: enterprise advisory, executive tone, structured proof, serif/sans hoặc display/body contrast.
- 15% AWS-inspired accent: deep navy / white / AWS orange, dùng tiết chế.

### Tránh

- Không dùng quá nhiều generic glassmorphism.
- Không lặp lại quá nhiều rounded card giống nhau.
- Không dùng decorative icon nếu không mang thông tin.
- Không thêm số liệu giả để làm đẹp.
- Không để placeholder/instruction nội bộ trên UI production.

### Visual thesis

CloudNexus không chỉ là một AWS reseller. Trang nên truyền tải:

> CloudNexus designs, migrates, secures, operates, and optimizes AWS environments through a measurable cloud operating model.

## 4. Checklist cần làm

## P0 — Bắt buộc trước khi public/demo nghiêm túc

### 4.1 Xóa placeholder và internal copy

Hiện đang có một số nội dung phá trust:

- `AWS Partner Placeholder`
- `MẪU CASE STUDY`
- `Case study format nên kể bằng kết quả kinh doanh.`
- `Các card dưới đây là mẫu cấu trúc nội dung...`
- Footer: `AWS Partner website concept · Replace logo, metrics and case studies with verified assets.`

Yêu cầu:

- Xóa hoặc thay toàn bộ bằng production-safe copy.
- Nếu chưa có dữ liệu thật, dùng wording trung thực nhưng customer-facing.
- Không để bất kỳ câu nào giống note cho designer/dev xuất hiện trên UI.

Gợi ý thay thế:

```text
AWS-focused Cloud Delivery
Certified Cloud Specialists
Well-Architected Approach
Managed CloudOps
FinOps Advisory
Generative AI on AWS
```

Nếu có AWS Partner tier thật thì dùng đúng tier thật. Nếu chưa được AWS xác nhận, không claim chính thức là AWS Partner.

---

### 4.2 Làm rõ AWS brand/legal credibility

Dev/content cần xác nhận các claim sau có thật không:

- Có phải AWS Partner chính thức không?
- Tier là gì: Select / Advanced / Premier?
- Có AWS certifications bao nhiêu?
- Có AWS competencies / service delivery designations không?
- Có AWS Partner Network profile link không?
- Có được phép dùng AWS Partner logo/badge không?

Yêu cầu implementation:

- Nếu có xác thực: thêm partner badge / partner profile link / tier.
- Nếu chưa có xác thực: đổi wording thành `AWS-focused`, `AWS cloud consulting`, `cloud transformation on AWS` thay vì claim official.
- Footer cần có AWS trademark disclaimer nếu dùng AWS name/logo nhiều.

---

### 4.3 Thống nhất ngôn ngữ

Hiện page lẫn English và Vietnamese. Cần chọn 1 hướng.

Option A — Vietnam-first:

- Navigation tiếng Việt.
- CTA tiếng Việt.
- Body copy tiếng Việt.
- Technical keywords AWS có thể giữ English.

Ví dụ nav:

```text
Trang chủ · Dịch vụ · Ngành · Câu chuyện khách hàng · Về CloudNexus · Tài nguyên · Đặt lịch tư vấn
```

Option B — International-first:

- Toàn bộ nav, hero, body copy tiếng Anh.
- Có thể thêm language switcher sau.

Recommendation: nếu target là doanh nghiệp Việt, chọn **Vietnam-first với technical keywords English**.

---

## P1 — Nâng visual theo huashu-design

### 4.4 Thiết kế lại hero visual thành AWS Operating Model Diagram

Hero hiện tại đang là abstract dashboard/floating cards. Nên chuyển thành diagram có cấu trúc hơn.

Yêu cầu:

- Hero visual phải thể hiện operating model thật, không chỉ decoration.
- Nên có flow rõ:

```text
Assess → Foundation → Migrate → Secure → Optimize → Operate
```

Hoặc:

```text
Business Goal
  ↓
AWS Foundation
  ↓
Migration Waves
  ↓
Security / FinOps / Observability
  ↓
Managed CloudOps
```

Các node nên có nội dung cụ thể:

- Landing Zone
- Account Strategy
- IAM / Network / Logging
- Migration Waves
- SecOps Guardrails
- FinOps Cadence
- Managed Operations

Acceptance criteria:

- Người xem nhìn hero visual là hiểu CloudNexus có methodology.
- Visual không còn giống generic SaaS dashboard.
- Ít nhất một phần hero là chi tiết được làm 120%, đủ khác biệt để screenshot.

---

### 4.5 Chuyển Services từ card list thành Capability System

Hiện services là list 8 card. Đúng nội dung nhưng hơi template.

Đề xuất layout mới:

```text
CloudNexus AWS Capability System

Foundation Layer
- Landing Zone
- AWS Organizations
- IAM Identity Center
- Network baseline
- Logging baseline

Migration Layer
- Assessment
- Wave planning
- Cutover
- Rollback plan
- Application modernization

Operate Layer
- Monitoring
- Incident response
- Backup / DR
- Patch management
- Managed CloudOps

Optimize Layer
- FinOps
- Rightsizing
- Savings Plans
- Well-Architected Review

Data & AI Layer
- Data lake
- Analytics
- Amazon Bedrock
- Search / chatbot / automation
```

Yêu cầu:

- Có thể vẫn dùng card, nhưng card phải thể hiện hệ thống/layer/process.
- Thêm AWS service tags ở mức vừa phải.
- Không dùng icon trang trí nếu không cần.

---

### 4.6 Framework section phải là visual signature chính

Framework nên là section mạnh nhất sau hero.

Nội dung đề xuất:

```text
The CloudNexus AWS Operating Model

1. Discover
2. Design Landing Zone
3. Migrate by Waves
4. Secure & Govern
5. Optimize Costs
6. Operate 24/7
7. Innovate with Data & AI
```

Yêu cầu visual:

- Dùng diagram / timeline / layered architecture.
- Có arrow, layer, line grid hoặc numbered system.
- Không chỉ là 6 text blocks rời rạc.
- Có thể dùng style `Diagram-Driven Isotype` trong huashu-design.

---

## P1 — Nội dung credibility cần bổ sung

### 4.7 Thêm Trust / Proof section gần hero

Reference như eCloudValley, TechX, Cloud Kinetics đều có proof mạnh. CloudNexus cần một trust section ngay sau hero hoặc sau trust strip.

Nội dung tùy dữ liệu thật:

Nếu có số thật:

```text
XX AWS-certified engineers
XX workloads migrated
XX managed AWS accounts
XX Well-Architected reviews
24/7 managed operations
XX% average cost optimization
```

Nếu chưa có số thật:

```text
AWS-focused delivery team
Structured migration methodology
Security-first cloud foundation
FinOps operating cadence
Managed operations playbook
```

Không invent số liệu.

---

### 4.8 Làm lại Success Stories thành customer-facing

Hiện section này đang giống internal content note.

Heading đề xuất:

```text
Customer outcomes built on AWS
```

Hoặc tiếng Việt:

```text
Kết quả kinh doanh từ các dự án AWS thực chiến
```

Card format đề xuất:

```text
Industry / Customer type
Main outcome metric or target outcome
Problem
CloudNexus solution
AWS services used
Business impact
CTA: Read case study / Request similar assessment
```

Ví dụ nếu chưa có tên khách hàng thật:

```text
Leading Vietnamese Retail Platform
Goal: Improve product discovery and reduce manual tagging
Solution: Amazon Bedrock + OpenSearch + serverless data pipeline
AWS services: Bedrock, OpenSearch, Lambda, S3
Outcome: Metric pending / representative engagement blueprint
```

Yêu cầu:

- Không ghi `MẪU CASE STUDY` trên UI.
- Nếu là case ẩn danh, ghi rõ theo kiểu production-safe: `Representative engagement`, `Anonymized customer story`, hoặc `Example engagement blueprint`.
- Không tạo metric giả.

---

### 4.9 About section cần có company credibility

About hiện tại cần làm rõ CloudNexus là ai.

Nội dung cần có:

- CloudNexus phục vụ nhóm khách hàng nào?
- Thị trường chính: Vietnam / SEA / global?
- Điểm mạnh: migration, managed services, security, FinOps, GenAI?
- Delivery model: assessment, implementation, managed operations.
- Team/certification/partner proof nếu có.

Đề xuất block:

```text
About CloudNexus
CloudNexus helps modern enterprises design, migrate, secure, operate, and optimize AWS environments through a structured cloud operating model.

What makes us different:
- AWS operating model, not one-off migration
- Security and governance from day one
- FinOps cadence built into operations
- Data and GenAI readiness after foundation is stable
```

---

### 4.10 Resources section cần có nội dung thật hơn

Thay vì link chung chung, tạo 3-4 resource item cụ thể:

- AWS Migration Readiness Checklist
- Landing Zone Starter Guide
- FinOps Cost Optimization Playbook
- Well-Architected Review Guide
- GenAI on AWS: From Prototype to Production

Mỗi item nên có:

- Title
- Short description
- Type: Guide / Checklist / Whitepaper / Blog
- CTA: Read guide / Download checklist

---

## P2 — UI/UX polish

### 4.11 Rà spacing và section rhythm

Một số section có cảm giác cao/rộng hơn nội dung cần thiết.

Yêu cầu:

- Kiểm tra CSS `padding-block`, `min-height`, `height`.
- Tránh section trống hoặc quá nhiều vertical whitespace.
- Mỗi viewport scroll nên có nội dung rõ ràng.
- Light/dark alternating section phải có mục đích, không chỉ để chia block.

Acceptance criteria:

- Không có đoạn scroll nào nhìn như blank band.
- Body page có nhịp: Hero → Proof → Problem → Capability → Methodology → Stories → About → Resources → CTA.

---

### 4.12 CTA flow

Hiện CTA chính:

- `Book a Cloud Consultation`
- `Tư vấn Cloud miễn phí`
- `Khám phá dịch vụ`

Yêu cầu:

- Tất cả CTA phải link đúng target.
- Primary CTA nên dẫn tới contact section/form/scheduling.
- Secondary CTA scroll tới Services/Capability.
- Case study CTA nếu chưa có page detail thì có thể scroll contact với query/context.

Nếu không có backend form, dùng mailto hoặc static contact block rõ ràng.

---

### 4.13 Accessibility/readability

Yêu cầu:

- Kiểm tra contrast của gray text trên dark background.
- Font size body tối thiểu dễ đọc.
- Button hover/focus state rõ.
- Header sticky không che content khi anchor scroll.
- Mobile responsive: nav collapse hoặc layout hợp lý.

Acceptance criteria:

- Không có text nhỏ/nhạt khó đọc ở service cards.
- Anchor click không bị header che heading.
- Mobile hero không vỡ layout.

---

### 4.14 Footer production-ready

Footer hiện còn concept note. Cần thay bằng footer thật.

Nội dung đề xuất:

- Short brand description
- Services links
- Company/About links
- Resources links
- Contact email/phone nếu có
- LinkedIn nếu có
- Privacy Policy / Terms nếu có
- AWS trademark disclaimer nếu dùng AWS name/logo

Ví dụ disclaimer:

```text
Amazon Web Services, AWS, and related marks are trademarks of Amazon.com, Inc. or its affiliates. CloudNexus is an independent cloud services provider.
```

Điều chỉnh theo trạng thái partner/legal thật.

---

## 5. Copy cụ thể đề xuất

### Hero headline options

Option 1:

```text
Modernize, secure, and operate on AWS with confidence.
```

Option 2:

```text
AWS transformation from strategy to managed operations.
```

Option 3:

```text
Build your AWS operating model, not just your cloud infrastructure.
```

### Hero subcopy Vietnam-first

```text
CloudNexus đồng hành cùng doanh nghiệp từ assessment, landing zone, migration theo từng wave đến bảo mật, vận hành 24/7, FinOps và nền tảng dữ liệu/AI trên AWS.
```

### Trust strip production-safe

```text
AWS-focused Delivery
Cloud Foundation
Migration Waves
Security Guardrails
FinOps Cadence
Managed CloudOps
GenAI Readiness
```

### Success Stories heading

```text
Kết quả kinh doanh từ các dự án AWS thực chiến
```

Subcopy:

```text
Các engagement dưới đây thể hiện cách CloudNexus tiếp cận migration, security, FinOps và GenAI trên AWS bằng outcome có thể đo lường.
```

Nếu chưa có case thật, dùng:

```text
Representative engagement blueprints based on common AWS transformation scenarios.
```

### Final CTA

```text
Không chắc nên bắt đầu AWS từ đâu?
Đặt lịch 30 phút để rà soát cloud readiness, rủi ro migration, security baseline và cơ hội tối ưu chi phí.
```

CTA button:

```text
Đặt lịch AWS assessment
```

---

## 6. Suggested final page structure

```text
1. Header
2. Hero: AWS transformation + Operating Model Diagram
3. Trust/Proof Strip
4. Why Change: business pains
5. CloudNexus Capability System
6. AWS Operating Model / Methodology Diagram
7. Industries + use cases
8. Customer Outcomes / Engagement Blueprints
9. About CloudNexus + AWS credibility
10. Resources
11. Final CTA / Contact
12. Footer
```

## 7. Acceptance criteria tổng

Dev/design được coi là done khi:

- Không còn placeholder/internal instruction trên UI.
- AWS partner claim đã được xác thực hoặc wording đã được soften.
- Page có một visual signature rõ: operating model / capability diagram.
- Services không chỉ là generic cards, mà thành system/layer/process.
- Case studies/customer outcomes customer-facing, không fake metric.
- Language nhất quán theo direction đã chọn.
- Spacing không tạo cảm giác blank section.
- CTA link đúng.
- Mobile không vỡ layout.
- Console không có JS error nghiêm trọng.
- Visual không còn giống generic AI SaaS template.

## 8. Dev QA checklist

Sau khi implement, kiểm tra:

- [ ] Open page desktop 1440×900.
- [ ] Open page mobile 390×844.
- [ ] Click all nav anchors.
- [ ] Click all CTAs.
- [ ] Check sticky header does not cover anchors.
- [ ] Check console errors.
- [ ] Search page text for placeholder terms:
  - `Placeholder`
  - `MẪU`
  - `concept`
  - `Replace`
  - `sample`
  - `lorem`
- [ ] Verify AWS claims are accurate.
- [ ] Verify footer legal/trademark copy.
- [ ] Screenshot hero, services, framework, stories, mobile hero.

## 9. Priority summary for dev

Nếu thời gian ít, làm theo thứ tự:

1. Xóa placeholder/internal copy.
2. Softening/fix AWS Partner claims.
3. Làm hero visual thành operating model diagram.
4. Làm Services thành capability system.
5. Làm Success Stories thành customer-facing engagement blueprints.
6. Giảm whitespace/section height.
7. Footer production-ready.
8. Mobile/accessibility QA.
