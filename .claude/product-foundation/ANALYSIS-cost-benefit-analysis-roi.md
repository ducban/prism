---
# Core Metadata
title: "Cost-Benefit Analysis & ROI"
title_vi: "Phân Tích Chi Phí-Lợi Ích & ROI"
framework_type: "Financial"
category: ["Product Management", "Financial Analysis", "Prioritization"]

# Origin & Authority
author: "Various (Standard Financial Practice)"
organization: "Business & Economics"
year_developed: "1970s"
original_source: "Cost-Benefit Analysis: Concepts and Practice"

# Root Integration
root_phase: ["Phase 2: Prioritize & Decide"]
root_commands: ["/phase2:roi", "/phase2:cba"]
when_to_use: "When Finance questions feature investment, or need to justify budget to leadership with objective numbers"

# Difficulty & Time
complexity: "Medium"
estimated_time: "3-5 days (data collection + analysis)"
skill_level: "Intermediate"

# Classification
tags: ["financial-analysis", "roi", "prioritization", "business-case", "decision-making"]
related_frameworks: ["RICE Prioritization", "Balanced Trade-Off Matrix", "Kano Model"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-20"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Book"
    title: "Cost-Benefit Analysis: Concepts and Practice"
    url: "https://www.worldcat.org/title/cost-benefit-analysis-concepts-and-practice/oclc/70046903"
    author: "Anthony E. Boardman et al."
    year: "2017"
  - type: "Article"
    title: "Cost-Benefit Analysis in Product Management"
    url: "https://www.geeksforgeeks.org/product-management/cost-benefit-analysis-in-product-management/"
    author: "GeeksforGeeks"
    year: "2024"
  - type: "Tool"
    title: "ROI Calculator Template"
    url: "https://productschool.com/blog/analytics/roi-template"
    author: "Product School"
    year: "2024"
  - type: "Article"
    title: "How to Calculate ROI of Digital Product"
    url: "https://www.boldare.com/blog/how-to-calculate-roi-of-digital-product/"
    author: "Boldare"
    year: "2024"
  - type: "Tutorial"
    title: "Feature ROI Calculator Guide"
    url: "https://productschool.com/blog/skills/product-templates-feature-roi-calculator"
    author: "Product School"
    year: "2024"
---

# Cost-Benefit Analysis (CBA) & ROI / Phân Tích Chi Phí-Lợi Ích

## Overview

**English:**
Cost-Benefit Analysis (CBA) and ROI (Return on Investment) are financial frameworks for evaluating whether a feature/project is worth the investment. Critical when cross-functional teams disagree—Finance wants low cost, UX wants high investment. Numbers cut through opinions.

**When to use it:**
- Finance team questions feature investment
- Multiple expensive options to choose from
- Need to justify budget to leadership
- Cross-functional conflict about resource allocation

**Vietnamese:**
Phân tích Chi phí-Lợi ích (CBA) và ROI là framework tài chính để đánh giá xem một tính năng/dự án có đáng đầu tư không. Quan trọng khi các phòng ban xung đột—Finance muốn chi phí thấp, UX muốn đầu tư cao. Con số giúp vượt qua ý kiến chủ quan.

---

## Core Formulas

### 1. ROI (Return on Investment)

```
ROI = (Net Benefit / Total Cost) × 100%

Where:
Net Benefit = Total Benefits - Total Costs
```

**Example:**
- Total Benefits: $500,000 (increased revenue)
- Total Costs: $200,000 (development + ops)
- Net Benefit: $500,000 - $200,000 = $300,000
- ROI = ($300,000 / $200,000) × 100% = **150% ROI**

**Interpretation**: For every $1 invested, you get $1.50 back (or 150% return).

---

### 2. Benefit-Cost Ratio (BCR)

```
BCR = Total Benefits / Total Costs
```

**Decision Rule:**
- BCR > 1 → Benefits exceed costs (GO!)
- BCR = 1 → Break even (MAYBE)
- BCR < 1 → Costs exceed benefits (NO GO)

**Example:**
- Benefits: $500,000
- Costs: $200,000
- BCR = $500,000 / $200,000 = **2.5**

**Interpretation**: For every $1 spent, you get $2.50 in benefits.

---

### 3. Payback Period

```
Payback Period = Total Investment / Annual Net Cash Flow
```

**Example:**
- Investment: $200,000
- Annual benefit: $100,000/year
- Payback Period = $200,000 / $100,000 = **2 years**

**Interpretation**: Takes 2 years to recover the investment.

---

### 4. Net Present Value (NPV)

```
NPV = Σ (Cash Flow / (1 + Discount Rate)^Year) - Initial Investment
```

**Why it matters**: Money today is worth more than money tomorrow (due to inflation, opportunity cost).

**Example:**
- Year 0: -$200,000 (investment)
- Year 1: +$100,000
- Year 2: +$100,000
- Year 3: +$100,000
- Discount rate: 10%

NPV = ($100K / 1.1) + ($100K / 1.21) + ($100K / 1.331) - $200K
NPV = $90.9K + $82.6K + $75.1K - $200K
NPV = **$48.6K**

**Interpretation**: After accounting for time value of money, project creates $48.6K in value.

---

## Step-by-Step CBA Process

### Step 1: Define All Costs

#### Categories to Consider:

#### 1. Development Costs
- Engineering time: (Engineers × Hours × Hourly Rate)
- Design time
- PM time
- QA/Testing time

**Example: Instant Refund Feature**
- 2 engineers × 160 hours × $100/hour = $32,000
- 1 designer × 40 hours × $80/hour = $3,200
- 1 PM × 60 hours × $90/hour = $5,400
- 1 QA × 80 hours × $70/hour = $5,600
**Development Total: $46,200**

---

#### 2. Infrastructure Costs
- Server costs (monthly/annual)
- Third-party API fees
- Database storage
- Security/compliance tools

**Example: Instant Refund Feature**
- Payment gateway fees: 2.9% + $0.30 per transaction
- Assume 1,000 refunds/month at avg $50:
  - Monthly: (1,000 × $50 × 0.029) + (1,000 × $0.30) = $1,450 + $300 = $1,750/month
  - Annual: $21,000/year

---

#### 3. Operational Costs
- Support team training
- Ongoing maintenance (bugs, updates)
- Customer support inquiries
- Financial reconciliation work

**Example: Instant Refund Feature**
- Finance team: 10 hours/week reconciliation × $60/hour × 52 weeks = $31,200/year
- Support training: $5,000 one-time
- Ongoing support: 5 hours/week × $50/hour × 52 weeks = $13,000/year

---

#### 4. Opportunity Costs
- What else could team build instead?
- Revenue lost while building this vs. other features

**Example:**
- Could have built "Enterprise SSO" instead
- Enterprise SSO estimated to bring $200K/year new revenue
- Opportunity cost = $200,000

---

**Total Costs (Year 1):**
- Development: $46,200
- Infrastructure: $21,000
- Operational: $49,200 ($5K + $31.2K + $13K)
- **Total Year 1: $116,400**

**Ongoing Costs (Year 2+):**
- Infrastructure: $21,000/year
- Operational: $44,200/year ($31.2K + $13K, no training)
- **Total Ongoing: $65,200/year**

---

### Step 2: Define All Benefits

#### Categories to Consider:

#### 1. Revenue Impact
- Increased sales (new customers)
- Reduced churn (retain existing customers)
- Upsells/cross-sells
- Higher pricing power

**Example: Instant Refund Feature**

**Reduced Churn:**
- Current: 500 customers churn/year due to refund frustration
- Each customer worth $1,200/year lifetime value
- 30% churn reduction expected (based on survey)
- Benefit: 500 × 0.30 × $1,200 = **$180,000/year**

**Increased Conversion:**
- 15% of trial users cite "refund policy" as concern
- 10,000 trials/year → 1,500 concerned about refunds
- 20% of these will convert with instant refunds
- 1,500 × 0.20 × $1,200 = **$360,000/year**

**Total Revenue Impact: $540,000/year**

---

#### 2. Cost Savings
- Reduced support tickets
- Less manual processing
- Automation savings
- Reduced errors/rework

**Example:**
- Current: 200 refund support tickets/month × 30 min each × $50/hour = $5,000/month
- With instant refunds: 80% reduction in tickets
- Savings: $5,000 × 0.80 × 12 months = **$48,000/year**

---

#### 3. Productivity Gains
- Time saved for users
- Faster processes
- Less context switching

**Example:**
- Operations team saves 15 hours/week on manual refund processing
- 15 hours × $60/hour × 52 weeks = **$46,800/year**

---

#### 4. Strategic Benefits (harder to quantify)
- Brand reputation improvement
- Competitive differentiation
- Customer satisfaction
- Employee morale

**Example:**
- Instant refunds become a competitive advantage
- Estimated worth: **$100,000/year** (based on competitor pricing difference)

---

**Total Benefits (Year 1):**
- Revenue impact: $540,000
- Cost savings: $48,000
- Productivity: $46,800
- Strategic: $100,000
**Total: $734,800/year**

---

### Step 3: Calculate ROI & Make Decision

**Year 1:**
- Total Costs: $116,400
- Total Benefits: $734,800
- Net Benefit: $734,800 - $116,400 = $618,400
- **ROI: ($618,400 / $116,400) × 100% = 531%**
- **BCR: $734,800 / $116,400 = 6.3**
- **Payback Period: $116,400 / $734,800 = 0.16 years = 2 months**

**3-Year NPV** (Discount rate: 10%):
- Year 0: -$116,400
- Year 1: +$734,800
- Year 2: +$669,600 ($734.8K benefits - $65.2K ongoing costs)
- Year 3: +$669,600

NPV = ($734.8K / 1.1) + ($669.6K / 1.21) + ($669.6K / 1.331) - $116.4K
NPV = $668K + $553K + $503K - $116K
NPV = **$1,608,000**

**Decision: STRONG GO** ✅

---

## Complete Example: Instant Refund Feature (Cross-Functional Conflict)

### Scenario Recap:
- UX Team: "Must build for customer experience!"
- Finance Team: "Cashflow nightmare!"
- Operations Team: "Please! Current process is killing us!"
- Product Team: "Is this worth it?"

**Traditional Approach**: Endless meetings, emotional arguments, compromise that satisfies no one.

**CBA Approach**: Let the numbers decide.

---

### Option A: Full Instant Digital Wallet

**Costs:**
- Development: $240,000 (6 months, 3 engineers)
- Infrastructure: $50,000/year (wallet system)
- Operational: $80,000/year (fraud monitoring, reconciliation)
- Financial risk: $500,000 (cashflow fronting)
**Total Year 1: $870,000**

**Benefits:**
- Revenue impact: $600,000/year
- Cost savings: $50,000/year
- Strategic: $150,000/year
**Total: $800,000/year**

**ROI: ($800K - $870K) / $870K = -8%** ❌
**BCR: 0.92** (Less than 1 = Costs exceed benefits)
**Payback: Never (negative in year 1)**

**Decision: NO GO**

---

### Option B: Instant Store Credit

**Costs** (from earlier calculation):
- Development: $46,200
- Infrastructure: $21,000/year
- Operational: $49,200/year
**Total Year 1: $116,400**

**Benefits:**
- Revenue impact: $540,000/year
- Cost savings: $48,000/year
- Productivity: $46,800/year
- Strategic: $100,000/year
**Total: $734,800/year**

**ROI: 531%** ✅
**BCR: 6.3** (Huge benefit vs. cost)
**Payback: 2 months**

**Decision: STRONG GO**

---

### Option C: 24-48 Hour Expedited Refund

**Costs:**
- Development: $15,000 (process change, minimal engineering)
- Infrastructure: $0
- Operational: $20,000/year (manual processing)
**Total Year 1: $35,000**

**Benefits:**
- Revenue impact: $250,000/year (45% satisfaction improvement)
- Cost savings: $20,000/year
- Strategic: $30,000/year
**Total: $300,000/year**

**ROI: ($300K - $35K) / $35K = 757%** ✅✅
**BCR: 8.6** (Best BCR!)
**Payback: 1.4 months**

**Decision: QUICK WIN**

---

### Step 4: Present to Leadership

**Data-Driven Recommendation:**

| Option | ROI | BCR | Payback | Risk | Recommendation |
|--------|-----|-----|---------|------|----------------|
| **A: Digital Wallet** | -8% | 0.92 | Never | High | ❌ Don't build |
| **B: Store Credit** | 531% | 6.3 | 2 months | Low | ✅ Build Phase 2 |
| **C: Expedited** | 757% | 8.6 | 1.4 months | Very Low | ✅✅ Build Phase 1 |

**Phased Approach:**
1. **Immediate** (Month 1): Ship Option C (Expedited 24-48hr)
   - Best ROI, lowest risk, fastest payback
   - Satisfies 45% of customer dissatisfaction

2. **Follow-up** (Month 3-4): Ship Option B (Store Credit)
   - Addresses remaining 60% dissatisfaction
   - Still great ROI with manageable risk

3. **Never**: Don't build Option A (Digital Wallet)
   - Negative ROI, high risk, poor BCR

**Result:**
- ✅ Finance happy: Phase 1 costs only $35K, not $870K
- ✅ UX happy: Customers get faster refunds immediately
- ✅ Operations happy: Less manual work
- ✅ Product happy: Data-driven decision with clear ROI

**Everyone wins because CBA provided objective financial analysis.**

---

## Common Mistakes

| Mistake | Why It's Bad | Better Approach |
|---------|-------------|-----------------|
| **Only counting obvious costs** | Miss infrastructure, ops, opportunity costs | Use comprehensive cost checklist |
| **Only counting revenue benefits** | Ignore cost savings, productivity, strategic value | Count ALL benefit categories |
| **Ignoring time value of money** | $100 today ≠ $100 in 3 years | Use NPV for multi-year projects |
| **Not validating assumptions** | "Assume 50% conversion increase" (guess) | Base on data, surveys, or conservative estimates |
| **Forgetting ongoing costs** | Feature costs money every year, not just year 1 | Calculate year 2+ costs |
| **Comparing options without same timeframe** | 1-year ROI vs. 3-year ROI = unfair | Use same timeframe for all options |

---

## Quick Decision Matrix

**When to use each metric:**

| Metric | Best For | Example Use Case |
|--------|----------|------------------|
| **ROI %** | Comparing multiple options | "Which of 3 features has best return?" |
| **BCR** | Go/No-go decisions | "Is this feature worth building at all?" |
| **Payback Period** | Leadership wants fast returns | "How quickly do we recover investment?" |
| **NPV** | Multi-year projects | "Is this 3-year platform investment worth it?" |

---

## Vietnamese Summary

Phân tích Chi phí-Lợi ích sử dụng 4 công thức chính:
- **ROI (Return on Investment)**: (Lợi ích ròng / Chi phí) × 100%
- **BCR (Benefit-Cost Ratio)**: Tổng lợi ích / Tổng chi phí (>1 = nên làm)
- **Payback Period**: Thời gian hoàn vốn = Đầu tư / Lợi ích hàng năm
- **NPV (Net Present Value)**: Giá trị hiện tại ròng (tính giá trị tiền theo thời gian)

Quy trình: Liệt kê tất cả chi phí (phát triển, infrastructure, vận hành, cơ hội), liệt kê tất cả lợi ích (doanh thu, tiết kiệm, năng suất), tính toán ROI/BCR/NPV, ra quyết định dựa trên số liệu.

---

## Related Frameworks

### Complementary Frameworks:
1. **RICE Prioritization** - Use CBA/ROI to validate the "Impact" score in RICE
2. **Balanced Trade-Off Matrix** - Use CBA/ROI as one dimension in the trade-off analysis
3. **Kano Model** - Combine with CBA to understand which delighters have best ROI
4. **Value Proposition Canvas** - Validate that your value propositions have positive ROI
5. **North Star Metric** - Use CBA to prioritize initiatives that move the North Star

### When to Combine:
- **CBA + RICE**: Calculate ROI for top RICE-scored features to validate financial viability
- **CBA + Kano**: Prioritize "Delighters" with highest ROI rather than all delighters
- **CBA + Trade-Off Matrix**: Add financial impact as a dimension in your trade-off decisions

---

## Expanded Learning Resources

### Books & Publications
1. **Cost-Benefit Analysis: Concepts and Practice** (4th Edition)
   - Authors: Anthony E. Boardman, David H. Greenberg, Aidan R. Vining, David L. Weimer
   - Publisher: Cambridge University Press (2017)
   - Focus: Comprehensive guide to CBA methodology with real-world applications
   - [WorldCat Link](https://www.worldcat.org/title/cost-benefit-analysis-concepts-and-practice/oclc/70046903)

2. **The Lean Product Playbook** by Dan Olsen
   - Chapter on prioritization includes ROI frameworks
   - Practical product management context

3. **Measuring and Managing Information Risk: A FAIR Approach** by Jack Freund & Jack Jones
   - Advanced risk-adjusted ROI calculations
   - Particularly useful for security/infrastructure investments

### Online Articles & Guides
1. **Cost-Benefit Analysis in Product Management** (GeeksforGeeks, 2024)
   - [Read Article](https://www.geeksforgeeks.org/product-management/cost-benefit-analysis-in-product-management/)
   - Step-by-step guide with product management examples
   - Includes templates and checklists

2. **How to Calculate ROI of Digital Product** (Boldare, 2024)
   - [Read Article](https://www.boldare.com/blog/how-to-calculate-roi-of-digital-product/)
   - Focus on digital products and SaaS
   - Real-world case studies

3. **Feature ROI Calculator Guide** (Product School, 2024)
   - [Read Guide](https://productschool.com/blog/skills/product-templates-feature-roi-calculator)
   - Tutorial on building feature-level ROI models
   - Includes Excel/Google Sheets templates

### Tools & Templates
1. **ROI Calculator Template** (Product School)
   - [Download Template](https://productschool.com/blog/analytics/roi-template)
   - Excel-based calculator with pre-built formulas
   - Customizable for different project types

2. **Business Case Template** (Aha!)
   - Comprehensive business case framework
   - Integrates CBA with strategic planning

3. **NPV Calculator** (Corporate Finance Institute)
   - Advanced financial modeling tools
   - Multi-year projection capabilities

### Video Courses
1. **Financial Analysis for Product Managers** (Product School)
   - 2-hour course covering ROI, NPV, and financial modeling
   - Real PM scenarios and exercises

2. **Data-Driven Product Management** (Udemy)
   - Section on financial analysis and prioritization
   - Includes CBA case studies

### Industry Reports
1. **The State of Product Management** (Product Management Institute)
   - Annual report including CBA adoption rates
   - Industry benchmarks for ROI expectations

2. **Tech Company Financial Metrics** (McKinsey)
   - How top tech companies evaluate investments
   - Benchmark ROI expectations by industry

---

## Quick Reference Cheat Sheet

### ROI Calculation Checklist

**COSTS:**
- [ ] Engineering time (hours × rate)
- [ ] Design time
- [ ] PM time
- [ ] QA time
- [ ] Infrastructure (servers, APIs, storage)
- [ ] Third-party tools/services
- [ ] Support team training
- [ ] Ongoing maintenance
- [ ] Opportunity cost (what else could we build?)

**BENEFITS:**
- [ ] Revenue increase (new customers)
- [ ] Churn reduction (retained customers)
- [ ] Conversion rate improvement
- [ ] Support ticket reduction
- [ ] Manual process automation
- [ ] Time savings (productivity)
- [ ] Strategic/competitive advantage

**CALCULATIONS:**
- [ ] ROI = (Net Benefit / Total Cost) × 100%
- [ ] BCR = Total Benefits / Total Costs
- [ ] Payback Period = Investment / Annual Benefit
- [ ] NPV (if multi-year project)

**DECISION:**
- [ ] ROI > 100%? (Getting more than invested)
- [ ] BCR > 1? (Benefits exceed costs)
- [ ] Payback < 2 years? (Reasonable timeframe)
- [ ] Compare against alternative options
- [ ] Validate assumptions with data

---

## Notes for Root Users

This framework is part of **Phase 2: Prioritize & Decide** in the Root workflow.

### Available Commands:
- `/phase2:roi` - Calculate ROI for a specific feature or initiative
- `/phase2:cba` - Run complete Cost-Benefit Analysis with all categories

### Integration with Other Root Tools:
1. **Before CBA**: Use Discovery frameworks (Jobs-to-be-Done, User Story Mapping) to understand what to build
2. **During CBA**: Use this framework to validate financial viability
3. **After CBA**: Use RICE or Trade-Off Matrix to compare validated options

### Best Practices in Root:
- Always start with customer research, then validate with CBA
- Use conservative estimates (better to under-promise)
- Document all assumptions for future reference
- Re-calculate ROI quarterly as actuals come in
- Share CBA results with all stakeholders for alignment

---

## Changelog

### Version 1.0 (2025-11-20)
- Initial framework documentation
- Complete extraction from PRODUCT-FOUNDATION.md
- Added comprehensive learning resources
- Structured for Root integration
- Bilingual content (English/Vietnamese)

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
