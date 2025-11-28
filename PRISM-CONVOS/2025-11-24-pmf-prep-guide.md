---
conversation_id: "2025-11-24-pmf-prep-guide"
date_created: "2025-11-24"
date_modified: "2025-11-24"
topic: "PMF Preparation Guide"
status: "active"
participants:
  - role: "user"
    name: "User"
  - role: "assistant"
    platform: "iFlow"
tags:
  - "pmf"
  - "product-market-fit"
  - "ceo-meeting"
  - "investor-presentation"
  - "preparation-guide"
summary: "CEO asking about PMF and investor meeting preparation guide"
related_files:
  - "03-PRODUCT-FOUNDATION/VALIDATION-product-market-fit.md"
  - "03-PRODUCT-FOUNDATION/METRICS-retention-churn-analysis.md"
file_hash: "pmf-guide-20251124"
---

# 🎯 Product-Market Fit Preparation Guide

## Tình huống của bạn

CEO đang hỏi về product-market fit và bạn có cuộc gặp với nhà đầu tư vào tuần tới. Bạn cần đo lường và chuẩn bị báo cáo PMF một cách chuyên nghiệp.

## 📚 Framework được đề xuất

**CHÍNH**: [VALIDATION-product-market-fit.md](../03-PRODUCT-FOUNDATION/VALIDATION-product-market-fit.md)
- **Tại sao framework này**: Cung cấp các phương pháp đo lường PMF chuẩn hóa và được chấp nhận rộng rãi trong giới đầu tư
- **Bạn sẽ học được**: Cách thực hiện Sean Ellis test, phân tích retention curve, và các tín hiệu PMF quan trọng
- **Thời gian đọc**: 45-60 phút
- **Phần trọng tâm**: "Sean Ellis Test" và "PMF Signals"

**PHỤ**: [METRICS-retention-churn-analysis.md](../03-PRODUCT-FOUNDATION/METRICS-retention-churn-analysis.md)
- **Tại sao cũng cần này**: Retention là chỉ số PMF quan trọng nhất để chứng minh với nhà đầu tư
- **Giá trị bổ sung**: Cách phân tích và trực quan hóa dữ liệu retention cho presentation

## ⚡ Kế hoạch hành động nhanh

- [ ] Đọc phần "Sean Ellis Test" trong VALIDATION-product-market-fit.md
- [ ] Thiết lập và gửi survey Sean Ellis cho users của bạn (cần 40% "very disappointed" để đạt PMF)
- [ ] Phân tích retention curve theo cohorts 30-60 ngày
- [ ] Chuẩn bị slide deck với 3 metrics chính: Sean Ellis score, Retention curve, và Growth indicators
- [ ] Luyện tập trình bày dữ liệu với câu chuyện "why users stay"

**Thời gian dự kiến**: 3-4 ngày để thu thập dữ liệu, 1 ngày để chuẩn bị presentation

## 🎓 Điểm chính cần nhớ

Product-market fit không phải là cảm tính - nó là số liệu: ≥40% users "very disappointed" nếu mất sản phẩm + retention curve đang làm phẳng.

## 💡 Mẹo chuyên nghiệp

1. **Chuẩn bị 2 kịch bản**: Nếu đạt PMF → kêu gọi scaling; Nếu chưa đạt → kêu gọi iteration funding
2. **Visualize retention curve** theo cohorts - nhà đầu tư muốn thấy curve đang làm phẳng
3. **So sánh với benchmarks** ngành của bạn để cho thấy context
4. **Chuẩn bị câu hỏi khó**: "What if your biggest competitor copied this?"

---

**Ngày tạo**: 2025-11-24
**Framework liên quan**: VALIDATION-product-market-fit.md, METRICS-retention-churn-analysis.md

## Actions Taken

1. ✅ Moved PMF-Prep-Guide.md to 04-ROOT-CONVOS/ folder
2. ✅ Updated file with conversation YAML header following RULES.md format
3. ✅ Updated relative paths to frameworks (./ → ../03-PRODUCT-FOUNDATION/)
4. ✅ Added entry to 00-CONVO-LOGS.md
5. ✅ Updated search index

## Context Notes

- This file was originally PMF-Prep-Guide.md in project root
- Converted to conversation format for better tracking
- Maintains all original content while following conversation structure
- Ready for CEO and investor meeting preparation

## Related Root Commands Available

For PMF assessment, you can use:
- `/scenario:pmf are we achieving product-market fit`
- `/phase7:analyze "current PMF status" timeframe="90d"`
- `/phase7:metrics define PMF metric="sean_ellis_score" target=40 unit="percent"`