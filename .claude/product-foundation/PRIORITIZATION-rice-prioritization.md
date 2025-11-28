---
# Core Metadata
title: "RICE Prioritization"
title_vi: "Ưu Tiên RICE"
framework_type: "Prioritization"
category: ["Product Management", "Prioritization", "Scoring"]

# Origin & Authority
author: "Intercom Product Team"
organization: "Intercom"
year_developed: "2016"
original_source: "RICE: Simple prioritization for product managers"

# Root Integration
root_phase: ["Phase 2: Prioritize & Decide"]
root_commands: ["/phase2:rice"]
when_to_use: "When you need objective, data-driven prioritization with multiple competing features"

# Difficulty & Time
complexity: "Medium"
estimated_time: "2-4 hours per batch of features"
skill_level: "Intermediate"

# Classification
tags: ["prioritization", "scoring", "data-driven", "objective", "quantitative"]
related_frameworks: ["ICE Scoring", "MoSCoW Prioritization", "Cost-Benefit Analysis"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-20"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Article"
    title: "RICE: Simple prioritization for product managers"
    url: "https://www.intercom.com/blog/rice-simple-prioritization-for-product-managers/"
    author: "Intercom"
    year: "2016"
  - type: "Tool"
    title: "RICE Scoring Calculator"
    url: "https://www.productplan.com/glossary/rice-scoring-model/"
    author: "ProductPlan"
    year: "2024"
  - type: "Guide"
    title: "RICE Prioritization Framework Guide"
    url: "https://www.productplan.com/learn/rice-prioritization/"
    author: "Roadmunk"
    year: "2024"
---

# RICE Prioritization / Ưu Tiên RICE

## Overview / Tổng Quan

**English:**
RICE helps you decide which features to build first by scoring them on 4 factors.

**RICE stands for:**
- **R**each: How many users will this affect?
- **I**mpact: How much will it help each user?
- **C**onfidence: How sure are you about your estimates?
- **E**ffort: How long will it take to build?

**Formula:** Score = (Reach × Impact × Confidence) / Effort

**Real example - Spotify's "Wrapped" feature:**
- **Reach**: 200 million users (everyone gets a Wrapped)
- **Impact**: 3 (massive - users share it everywhere)
- **Confidence**: 90% (they've done it before)
- **Effort**: 6 person-months
- **Score**: (200,000,000 × 3 × 0.9) / 6 = 90,000,000

This high score explains why Spotify does Wrapped every year!

**Vietnamese:**
RICE giúp bạn quyết định tính năng nào nên được xây dựng trước bằng cách chấm điểm dựa trên 4 yếu tố.

**RICE là viết tắt của:**
- **R**each (Phạm vi): Bao nhiêu người dùng sẽ bị ảnh hưởng?
- **I**mpact (Tác động): Nó sẽ giúp mỗi người dùng nhiều như thế nào?
- **C**onfidence (Độ tự tin): Bạn chắc chắn đến mức nào về ước tính của mình?
- **E**ffort (Nỗ lực): Mất bao lâu để xây dựng?

**Công thức:** Điểm = (Phạm vi × Tác động × Độ tự tin) / Nỗ lực

**Ví dụ thực tế - Tính năng "Wrapped" của Spotify:**
- **Phạm vi**: 200 triệu người dùng (mọi người đều nhận Wrapped)
- **Tác động**: 3 (rất lớn - người dùng chia sẻ khắp nơi)
- **Độ tự tin**: 90% (họ đã làm trước đây)
- **Nỗ lực**: 6 người-tháng
- **Điểm**: (200,000,000 × 3 × 0.9) / 6 = 90,000,000

Điểm số cao này giải thích tại sao Spotify làm Wrapped hàng năm!

---

## RICE Scoring Playbook / Hướng Dẫn Chấm Điểm RICE

**English:**

This playbook provides detailed instructions for scoring each RICE factor. Use this when prioritizing features for the Root project.

### Factor 1: Reach (Phạm vi)

**Definition**: How many users/customers will this feature affect within a specific time period (usually per quarter or per month)?

**How to Score**:
- Use **actual numbers**, not percentages
- Be specific about the time period (e.g., "per quarter", "per month")
- Base it on data when possible

**Scoring Guide**:

| Reach Score | Meaning | Example |
|------------|---------|---------|
| 0-100 | Tiny niche segment | Internal tool for 5 team members |
| 100-1,000 | Small user group | Feature for enterprise customers (50 companies × 20 users each) |
| 1,000-10,000 | Moderate segment | Mobile app feature (10% of 100K users) |
| 10,000-100,000 | Large segment | Core feature (50% of 200K users) |
| 100,000+ | Mass market | Platform-wide change (all users) |

**How to Calculate Reach for Root**:

1. **New Capability**: Estimate how many PMs will use this specific capability per quarter
   - Example: `/phase3:prd` command → Assume 70% of active users need PRDs → Reach = 700 (if 1,000 active users)

2. **Enhancement**: Count existing users who will benefit
   - Example: Improve RICE scoring → All users who prioritize → Reach = 1,000

3. **Fix/Improvement**: Count affected users
   - Example: Fix broken command → Users who tried and failed → Reach = 50

**Common Mistakes to Avoid**:
- ❌ Don't use percentages (use actual numbers)
- ❌ Don't count potential future users (use current user base)
- ❌ Don't double-count (if a user benefits multiple times, count them once)

---

### Factor 2: Impact (Tác động)

**Definition**: How much will this feature improve the experience for each affected user?

**How to Score**:
- Use the scale: 0.25 (minimal), 0.5 (low), 1 (medium), 2 (high), 3 (massive)
- Choose ONE value per feature
- Consider: Does this solve a critical pain point or just a nice-to-have?

**Scoring Guide**:

| Impact Score | Meaning | User Reaction | Example |
|-------------|---------|---------------|---------|
| **3 - Massive** | Transformative change | "This changes everything!" | Spotify Wrapped (massive viral sharing), Dark mode (highly requested) |
| **2 - High** | Significant improvement | "This is really helpful!" | Slack Threads (solves major pain point), Auto-save feature |
| **1 - Medium** | Noticeable benefit | "That's nice to have" | UI polish, minor convenience feature |
| **0.5 - Low** | Small improvement | "Barely noticed but useful" | Tooltip improvement, color adjustment |
| **0.25 - Minimal** | Tiny enhancement | "Meh, okay I guess" | Edge case fix, obscure setting |

**How to Determine Impact for Root**:

Ask yourself these questions:

1. **Pain Point Severity**:
   - Does this solve a **blocker** (can't do their job)? → Impact = 3
   - Does this solve a **major frustration** (can do it, but it's painful)? → Impact = 2
   - Does this make something **easier** (already works, just faster)? → Impact = 1
   - Is this just **polish** (minor improvement)? → Impact = 0.5

2. **Frequency of Use**:
   - Will users hit this **daily**? → Higher impact
   - Will users hit this **weekly**? → Medium impact
   - Will users hit this **rarely**? → Lower impact

3. **Business Impact**:
   - Does this directly affect **revenue** or **retention**? → Higher impact
   - Does this improve **efficiency** significantly? → Medium-high impact
   - Is this just **nice to have**? → Lower impact

**Examples for Root**:

| Feature | Impact Score | Reasoning |
|---------|-------------|-----------|
| Add `/phase3:prd` command (PRD generation) | 3 (Massive) | Solves major blocker - PMs spend 8 hours on PRDs, reduces to 3 hours |
| Add RICE calculation to `/phase2:rice` | 2 (High) | Significantly improves prioritization - automatic calculation saves time and reduces errors |
| Add color coding to status | 1 (Medium) | Nice visual improvement, easier to scan |
| Fix typo in help text | 0.25 (Minimal) | Barely noticed, doesn't affect functionality |

**Common Mistakes to Avoid**:
- ❌ Don't score everything as 3 (be honest - most features are 1 or 2)
- ❌ Don't let personal preference bias you (use data and user feedback)
- ❌ Don't confuse "cool technology" with "user impact" (users care about value, not tech)

---

### Factor 3: Confidence (Độ tự tin)

**Definition**: How confident are you in your Reach and Impact estimates? Express as percentage.

**How to Score**:
- Use percentages: 10%, 20%, 30%... up to 100%
- Be honest - it's better to have low confidence than to overestimate
- Based on quality of data/evidence you have

**Scoring Guide**:

| Confidence % | Meaning | Evidence Quality | Example |
|-------------|---------|------------------|---------|
| **100%** | Absolute certainty | Proven with data from similar feature | Re-launching something that worked before (Spotify Wrapped year 2+) |
| **80%** | Very confident | Strong data supporting estimates | A/B test showed positive results, or validated with users |
| **50%** | Moderate confidence | Some data or qualitative feedback | User interviews suggest need, but no hard data |
| **30%** | Low confidence | Mostly assumptions/intuition | "We think users might want this" |
| **10%** | Very uncertain | Pure speculation | "Maybe this could be useful?" |

**How to Determine Confidence for Root**:

Ask yourself: **What evidence do I have?**

1. **You have STRONG evidence (80-100%)**:
   - ✅ Direct user feedback / feature requests
   - ✅ Usage data from similar features
   - ✅ Competitive analysis (competitors have this)
   - ✅ We've done this before successfully

   Example: Adding `/phase1:incident` command
   - Evidence: 15 users explicitly requested it in surveys
   - Similar: `/phase1:idea` is used 200 times/week
   - Confidence: 80%

2. **You have SOME evidence (50-70%)**:
   - ✅ User interviews mentioned the pain point
   - ✅ Industry best practices suggest it
   - ✅ No data but strong logical reasoning

   Example: Adding RICE scoring guide
   - Evidence: 3 team members asked "how do I score Impact?"
   - Logic: If we provide the tool, we should teach how to use it
   - Confidence: 60%

3. **You're mostly GUESSING (10-40%)**:
   - ❌ No user requests
   - ❌ No similar features to compare to
   - ❌ Just an idea you think is cool

   Example: Adding a "feature mood analyzer"
   - Evidence: None
   - Just an idea: "AI could analyze if features sound exciting"
   - Confidence: 20%

**Common Mistakes to Avoid**:
- ❌ Don't default to 100% confidence (rarely justified)
- ❌ Don't use confidence to game the score (be honest)
- ❌ Don't confuse "I really want this" with "I'm confident in the estimates"

---

### Factor 4: Effort (Nỗ lực)

**Definition**: How much time will this take to build, test, and ship? Measured in person-months.

**How to Score**:
- Use **person-months**: 1 person working for 1 month = 1 person-month
- Include ALL work: design, development, testing, documentation, deployment
- Be realistic - most things take longer than you think

**Scoring Guide**:

| Effort Score | Time | Complexity | Example |
|------------|------|------------|---------|
| **0.5** | 1-2 weeks | Trivial | Fix typo, update text, minor config change |
| **1** | 1 month | Small | Simple command, basic CRUD, small feature |
| **2** | 2 months | Moderate | Feature with multiple components, integration work |
| **4** | 4 months | Large | Complex feature, new architecture, cross-platform |
| **6+** | 6+ months | Very large | Major platform change, new infrastructure |

**How to Calculate Effort for Root**:

Use this formula:
```
Effort = (Design + Development + Testing + Documentation + Deployment) / Team Size
```

**Example Calculation**:

Feature: Add `/phase3:prd` PRD generation command

1. **Design** (0.5 weeks):
   - Define PRD template structure
   - Design prompt for AI

2. **Development** (2 weeks):
   - Create command files for 5 platforms
   - Implement PRD generation logic
   - Add YAML frontmatter handling

3. **Testing** (1 week):
   - Test on all 5 platforms
   - Fix bugs
   - Validate output quality

4. **Documentation** (0.5 weeks):
   - Add usage examples
   - Update WORKFLOW.md

5. **Deployment** (0.5 weeks):
   - Deploy to all platforms
   - Monitor for issues

**Total**: 4.5 weeks = ~1 month = **Effort: 1**

**Adjustment Factors**:

Multiply effort if:
- 🔴 High uncertainty / new technology → 1.5x
- 🔴 Requires coordination across teams → 1.3x
- 🔴 High risk / sensitive area → 1.5x
- 🟢 Very similar to existing work → 0.8x
- 🟢 Template/pattern already exists → 0.7x

**Common Mistakes to Avoid**:
- ❌ Don't forget testing and documentation (often 30-40% of total effort)
- ❌ Don't use "ideal case" estimates (use realistic timelines)
- ❌ Don't forget deployment and bug fixes post-launch
- ❌ Don't count parallel work as additive (2 people for 1 month = 1 person-month if they can work fully in parallel)

---

## Putting It All Together / Tổng Hợp

### Final RICE Score Formula

```
RICE Score = (Reach × Impact × Confidence) / Effort
```

### Complete Example: Adding Dark Mode to Root

**1. Reach**: 1,000 users per quarter (assume 70% of 1,500 active users will use it)

**2. Impact**: 2 (High)
   - Solves major pain point for users working at night
   - Requested by 45 users in surveys
   - Reduces eye strain (measurable benefit)

**3. Confidence**: 80%
   - Strong evidence: Direct user requests
   - Similar features in other tools are highly adopted
   - Industry standard (most apps have dark mode)

**4. Effort**: 3 person-months
   - Design: 1 week (create dark theme palette)
   - Development: 8 weeks (implement across all platforms, test combinations)
   - Testing: 2 weeks (accessibility testing, edge cases)
   - Documentation: 1 week

**Calculation**:
```
RICE = (1,000 × 2 × 0.8) / 3
     = 1,600 / 3
     = 533.33
```

**Interpretation**: Score of 533 is HIGH - should prioritize this feature!

---

## When to Use RICE vs Other Frameworks

### Use RICE When:
- ✅ You have some data about reach and impact
- ✅ You're comparing multiple features against each other
- ✅ You need an objective scoring system
- ✅ Your team tends to disagree on priorities
- ✅ You want to balance quick wins with strategic bets

### Use ICE Instead When:
- 🔄 You need faster, simpler scoring
- 🔄 You don't have reach data
- 🔄 You're doing quick prioritization in a meeting

### Use MoSCoW Instead When:
- 🔄 You need to communicate to stakeholders simply
- 🔄 You're working with fixed deadlines/budgets
- 🔄 The decision is more about dependencies than value

### Use Cost-Benefit Analysis Instead When:
- 🔄 You need to justify ROI to executives
- 🔄 You're evaluating very expensive initiatives
- 🔄 Revenue impact is the primary concern

---

## Common Mistakes & How to Avoid Them

### Mistake 1: Inflating Scores to Get Your Feature Prioritized
**Problem**: Teams game the system by inflating impact or reach

**Solution**:
- Require evidence for all scores
- Have a second person validate scoring
- Track actual results vs. predicted scores to build calibration

### Mistake 2: Scoring in a Vacuum
**Problem**: Each PM scores their own features without coordination

**Solution**:
- Score features together as a team
- Use the same benchmarks across all features
- Create a "reference feature" everyone knows

### Mistake 3: Forgetting to Update Scores
**Problem**: You score features once and never revisit

**Solution**:
- Re-score quarterly or when new data emerges
- Update confidence as you learn more
- Archive features that are no longer relevant

### Mistake 4: Over-Precision
**Problem**: Spending hours debating if reach is 1,247 or 1,253

**Solution**:
- Use round numbers (1,000 not 1,247)
- Remember: RICE is a prioritization tool, not a scientific formula
- Speed matters more than perfect accuracy

### Mistake 5: Ignoring Strategic Importance
**Problem**: Low-scoring features that are strategically critical get deprioritized

**Solution**:
- Add a "strategic multiplier" for key initiatives
- Separate "strategic bets" from "incremental improvements"
- Be explicit when overriding RICE for strategy

---

## Related Frameworks

### ICE Scoring
**Relationship**: Simpler version of RICE
- Uses 1-10 scales instead of actual numbers
- Faster but less precise
- Good for brainstorming sessions

**When to use ICE**: Quick prioritization, no data available

### MoSCoW Prioritization
**Relationship**: Categorical vs. numerical
- Groups features into Must/Should/Could/Won't
- Less granular than RICE
- Better for stakeholder communication

**When to use MoSCoW**: Fixed scope projects, communicating to non-technical stakeholders

### Cost-Benefit Analysis
**Relationship**: More financial focus
- Emphasizes revenue impact
- Requires more detailed cost modeling
- Better for business cases

**When to use CBA**: Large investments, need executive buy-in

### Kano Model
**Relationship**: Complements RICE
- Classifies features by user satisfaction impact
- Can inform your Impact score in RICE
- Better for understanding feature types

**When to use Kano**: Understanding what delights users vs. what's expected

---

## Learning Resources

### Official Resources
- [RICE: Simple prioritization for product managers](https://www.intercom.com/blog/rice-simple-prioritization-for-product-managers/) - Original article by Intercom (2016)
- [RICE Scoring Calculator](https://www.productplan.com/glossary/rice-scoring-model/) - ProductPlan interactive tool

### Additional Reading
- [How to Use RICE Scoring](https://roadmunk.com/guides/rice-score-prioritization/) - Roadmunk guide
- [RICE Prioritization: The Ultimate Guide](https://www.productboard.com/glossary/rice-scoring/) - Productboard comprehensive guide
- [When RICE Prioritization Fails](https://www.reforge.com/blog/product-prioritization) - Reforge critical analysis

### Templates & Tools
- [RICE Scoring Spreadsheet Template](https://docs.google.com/spreadsheets/d/1VXvwZqLtLwMbBmxhKqgKZvtRLJGHQ5g_JxLPL9LJQiM/edit) - Google Sheets template
- [RICE Score Calculator](https://www.prioritizr.com/rice-calculator) - Online calculator
- [Root `/phase2:rice` command](#) - Built-in Root command

### Case Studies
- **Spotify Wrapped**: How RICE justified annual investment
- **Slack Threads**: Prioritizing collaboration features
- **Notion Database Views**: Balancing power-user vs. casual features

---

## Quick Reference Card

### The Formula
```
RICE = (Reach × Impact × Confidence) / Effort
```

### Scoring Quick Guide

| Factor | Range | Key Question |
|--------|-------|--------------|
| **Reach** | Actual number | How many users per quarter? |
| **Impact** | 0.25, 0.5, 1, 2, 3 | How much does it help each user? |
| **Confidence** | 10%-100% | How sure are you? |
| **Effort** | Person-months | How long to build? |

### Interpreting Scores

| RICE Score | Priority | Action |
|-----------|----------|--------|
| **500+** | Very High | Do this now |
| **100-500** | High | Schedule this quarter |
| **50-100** | Medium | Consider for backlog |
| **10-50** | Low | Nice to have |
| **<10** | Very Low | Probably skip |

### Common Pitfalls Checklist
- [ ] Did you use actual numbers for Reach (not percentages)?
- [ ] Did you choose only ONE Impact value (not a range)?
- [ ] Did you express Confidence as a decimal (80% = 0.8)?
- [ ] Did you include testing & documentation in Effort?
- [ ] Did you score relative to other features (not in isolation)?
- [ ] Did you document your assumptions and evidence?

---

## Vietnamese Summary / Tóm Tắt Tiếng Việt

### Công Thức RICE
```
Điểm RICE = (Phạm vi × Tác động × Độ tự tin) / Nỗ lực
```

### Hướng Dẫn Chấm Điểm Nhanh

| Yếu Tố | Khoảng Giá Trị | Câu Hỏi Chính |
|--------|----------------|---------------|
| **Phạm vi** | Số thực tế | Bao nhiêu người dùng mỗi quý? |
| **Tác động** | 0.25, 0.5, 1, 2, 3 | Giúp mỗi người dùng nhiều như thế nào? |
| **Độ tự tin** | 10%-100% | Bạn chắc chắn đến mức nào? |
| **Nỗ lực** | Người-tháng | Mất bao lâu để xây dựng? |

### Khi Nào Sử Dụng RICE
- ✅ Khi bạn có dữ liệu về phạm vi và tác động
- ✅ Khi so sánh nhiều tính năng với nhau
- ✅ Khi cần hệ thống chấm điểm khách quan
- ✅ Khi nhóm thường bất đồng về ưu tiên
- ✅ Khi muốn cân bằng giữa chiến thắng nhanh và đặt cược chiến lược

### Sai Lầm Thường Gặp
1. **Thổi phồng điểm số**: Yêu cầu bằng chứng cho tất cả điểm
2. **Chấm điểm riêng lẻ**: Chấm điểm cùng nhau như một nhóm
3. **Không cập nhật**: Chấm lại hàng quý hoặc khi có dữ liệu mới
4. **Quá chính xác**: Sử dụng số tròn, tốc độ quan trọng hơn độ chính xác hoàn hảo
5. **Bỏ qua tầm quan trọng chiến lược**: Thêm "hệ số chiến lược" cho sáng kiến chính

---

**Last Updated**: 2025-11-20
**Version**: 1.0
**Root Command**: `/phase2:rice`
**Next Review**: 2025-12-20

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
