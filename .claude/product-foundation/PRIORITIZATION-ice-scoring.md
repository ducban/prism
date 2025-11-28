---
# Core Metadata
title: "ICE Scoring"
title_vi: "Chấm Điểm ICE"
framework_type: "Prioritization"
category: ["Product Management", "Prioritization", "Scoring"]

# Origin & Authority
author: "Sean Ellis"
organization: "Growth Hacking"
year_developed: "2010"
original_source: "Growth Hacking Methodology"

# Root Integration
root_phase: ["Phase 2: Prioritize & Decide"]
root_commands: ["/phase2:ice"]
when_to_use: "When you need quick prioritization with limited data, or for growth experiments"

# Difficulty & Time
complexity: "Low"
estimated_time: "1-2 hours per batch"
skill_level: "Beginner"

# Classification
tags: ["prioritization", "scoring", "growth-hacking", "quick-wins", "experimentation"]
related_frameworks: ["RICE Prioritization", "MoSCoW Prioritization", "AARRR"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-20"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Tool"
    title: "ICE Score Calculator"
    url: "https://www.productplan.com/glossary/ice-scoring-model/"
    author: "ProductPlan"
    year: "2024"
  - type: "Article"
    title: "ICE Method: How to Choose Better Product Features"
    url: "https://hygger.io/blog/ice-method-helps-choose-better-product-features/"
    author: "Hygger"
    year: "2024"
  - type: "Guide"
    title: "ICE vs RICE: Which Framework to Use"
    url: "https://www.productplan.com/learn/ice-scoring-vs-rice-scoring/"
    author: "ProductPlan"
    year: "2024"
---

# ICE Scoring / Chấm Điểm ICE

## Overview / Tổng Quan

**English:**

ICE is simpler than RICE - it's for quick decisions when you don't have exact data. Perfect for early-stage products, growth experiments, and rapid prioritization sessions where speed matters more than precision.

**ICE stands for:**
- **I**mpact: 1-10 scale (how valuable?)
- **C**onfidence: 1-10 scale (how sure are you?)
- **E**ase: 1-10 scale (how easy to build?)

**Vietnamese:**

ICE đơn giản hơn RICE - dùng cho quyết định nhanh khi bạn không có dữ liệu chính xác. Hoàn hảo cho sản phẩm giai đoạn đầu, thử nghiệm tăng trưởng, và các phiên ưu tiên nhanh khi tốc độ quan trọng hơn độ chính xác.

---

## The ICE Formula / Công Thức ICE

**Two Calculation Methods:**

### Method 1: Average (Recommended for Beginners)
```
ICE Score = (Impact + Confidence + Ease) / 3
```

**Advantages:**
- Easy to understand and compare
- Scores range from 1-10 (familiar scale)
- Good for comparing features on similar scale

### Method 2: Multiplication (For Advanced Users)
```
ICE Score = Impact × Confidence × Ease
```

**Advantages:**
- Amplifies differences between features
- Low score in any single factor significantly reduces total
- Penalizes risky or difficult features more heavily
- Scores can range from 1-1000

**When to Use Which Formula:**
- **Average Method**: Quick prioritization, similar types of features, beginner-friendly
- **Multiplication Method**: When you want to heavily penalize features with low ease or confidence, growth experiments

---

## Factor 1: Impact (Tác động) / 1-10 Scale

**Definition**: How much value will this create for users and the business?

### Scoring Guide

| Score | Meaning | Business Effect | Example |
|-------|---------|----------------|---------|
| **9-10** | Game-changer | Transformative for business/users | New revenue stream, major competitive advantage |
| **7-8** | High impact | Significant improvement | Solves major pain point, retention driver |
| **5-6** | Moderate impact | Noticeable benefit | Efficiency improvement, nice-to-have feature |
| **3-4** | Low impact | Minor benefit | Small polish, edge case fix |
| **1-2** | Minimal impact | Barely noticeable | Cosmetic change, obscure feature |

### How to Score Impact

**Questions to ask:**

1. **User Value**: How much does this help users?
   - Solves critical pain point? → 9-10
   - Addresses common frustration? → 7-8
   - Nice improvement? → 5-6
   - Minor convenience? → 3-4
   - Barely noticeable? → 1-2

2. **Business Value**: Does this drive adoption, retention, or revenue?
   - Drives new revenue stream? → 9-10
   - Increases retention significantly? → 7-8
   - Improves metrics moderately? → 5-6
   - Small metric improvement? → 3-4
   - No measurable business impact? → 1-2

3. **Strategic Importance**: Is this aligned with product vision?
   - Critical to strategy? → 9-10
   - Strongly aligned? → 7-8
   - Somewhat aligned? → 5-6
   - Loosely aligned? → 3-4
   - Not aligned? → 1-2

### Impact Examples

**For Root:**
- `/phase3:prd` command (PRD generation): **9** - Major time saver for PMs
- Dark mode: **8** - Highly requested, reduces eye strain, improves retention
- Better error messages: **5** - Improves UX moderately
- Update logo: **2** - Minimal impact on user value

**For Instagram Stories (2016 Launch):**
- **Impact: 10** - Snapchat was dominating, critical competitive response needed

---

## Factor 2: Confidence (Độ tự tin) / 1-10 Scale

**Definition**: How confident are you this will achieve the expected impact?

### Scoring Guide

| Score | Meaning | Evidence | Example |
|-------|---------|----------|---------|
| **9-10** | Very confident | Proven data, done before | Re-running successful campaign, validated feature |
| **7-8** | Confident | Good evidence | Strong user requests, similar features work well |
| **5-6** | Moderate | Some evidence | User interviews, logical assumptions |
| **3-4** | Low | Weak evidence | Gut feeling, speculation |
| **1-2** | Very uncertain | No evidence | Complete guess, experimental |

### How to Score Confidence

**Evidence Types (Ranked by Strength):**

1. **Proven Data (9-10)**:
   - A/B test results
   - Analytics showing clear user behavior
   - Successfully implemented elsewhere
   - Direct user research with validation

2. **Strong Evidence (7-8)**:
   - Multiple user requests
   - Industry best practices
   - Similar features performing well
   - Expert recommendations

3. **Moderate Evidence (5-6)**:
   - User interviews (small sample)
   - Logical assumptions
   - Competitive analysis
   - Internal team insights

4. **Weak Evidence (3-4)**:
   - Gut feeling
   - Single stakeholder opinion
   - Speculation
   - Unvalidated hypothesis

5. **No Evidence (1-2)**:
   - Complete guess
   - Wild experimentation
   - No data or research

### Confidence Examples

- Adding highly-requested feature with 100+ user votes: **9** - Users explicitly asked
- Industry best practice (e.g., OAuth login): **7** - Works well for others
- Logical UX improvement: **5** - Makes sense but unvalidated
- Experimental growth hack: **3** - Just testing an idea
- Random feature idea: **1** - Complete speculation

**For Instagram Stories (2016 Launch):**
- **Confidence: 8** - They had the team, tech, and saw Snapchat's success

---

## Factor 3: Ease (Dễ dàng) / 1-10 Scale

**Definition**: How easy is this to implement? Consider development, testing, documentation, and deployment.

### Scoring Guide

| Score | Meaning | Time | Complexity | Example |
|-------|---------|------|------------|---------|
| **9-10** | Very easy | Hours-days | Trivial | Config change, text update |
| **7-8** | Easy | 1-2 weeks | Simple | Small feature, minor integration |
| **5-6** | Moderate | 1 month | Some complexity | Multiple components, testing needed |
| **3-4** | Hard | 2-3 months | Complex | New architecture, cross-team work |
| **1-2** | Very hard | 3+ months | Very complex | Platform overhaul, major infrastructure |

### How to Score Ease

**Factors to Consider:**

1. **Development Time**:
   - Hours to days? → 9-10
   - 1-2 weeks? → 7-8
   - 1 month? → 5-6
   - 2-3 months? → 3-4
   - 3+ months? → 1-2

2. **Technical Complexity**:
   - Simple config change? → 9-10
   - Straightforward code? → 7-8
   - Some architectural decisions? → 5-6
   - Major refactoring needed? → 3-4
   - Complete system redesign? → 1-2

3. **Dependencies & Coordination**:
   - No dependencies? → +2 points
   - One team involved? → +1 point
   - Multiple teams needed? → -2 points
   - External dependencies? → -3 points

4. **Testing & Deployment**:
   - Quick to test? → Higher score
   - Complex testing scenarios? → Lower score
   - Risky deployment? → Lower score

**Be Realistic**: Most things are 2x harder than they seem. When in doubt, score lower.

### Ease Examples

- Update help text: **10** - Minutes to change
- Add simple slash command: **7** - 1 week development
- Multi-platform feature: **5** - 1 month, testing across platforms
- Database migration: **3** - 2 months, risky
- New infrastructure: **2** - 3+ months, very complex

**For Instagram Stories (2016 Launch):**
- **Ease: 6** - Needed new infrastructure for ephemeral content, but had experienced team

---

## Complete ICE Scoring Example / Ví Dụ Hoàn Chỉnh

### Real-World Example: Instagram Stories (2016)

**Context**: Snapchat was dominating ephemeral content. Instagram needed to respond.

**Scoring**:

1. **Impact: 10**
   - Snapchat was eating Instagram's lunch with younger users
   - Critical competitive feature
   - Could retain/attract millions of users
   - Aligned with company strategy

2. **Confidence: 8**
   - Snapchat proved the concept works
   - Instagram had experienced team
   - Similar technology to existing video features
   - High user demand for ephemeral content

3. **Ease: 6**
   - Needed new infrastructure for 24-hour expiration
   - Required camera improvements
   - Had to work across iOS/Android
   - But team was experienced and had resources

**Calculation (Average Method)**:
```
ICE Score = (10 + 8 + 6) / 3 = 8.0
```

**Calculation (Multiplication Method)**:
```
ICE Score = 10 × 8 × 6 = 480
```

**Result**: High score → They prioritized and built it → Now has 500M+ daily users!

---

### Root Example: Command Autocomplete Feature

**Context**: Users want autocomplete when typing slash commands for easier discovery.

**Scoring**:

1. **Impact: 7** (High)
   - Makes commands easier to discover
   - Reduces learning curve for new users
   - Improves command usage efficiency
   - Competitive with other CLI tools

2. **Confidence: 6** (Moderate)
   - No direct user data yet
   - Logical UX improvement
   - Works well in similar tools (VS Code, Slack)
   - Some user requests in feedback

3. **Ease: 4** (Hard)
   - Needs implementation across 5 platforms
   - Complex autocomplete logic
   - Testing across different terminals
   - 2-3 months development time

**Calculation (Average Method)**:
```
ICE Score = (7 + 6 + 4) / 3 = 5.67
```

**Calculation (Multiplication Method)**:
```
ICE Score = 7 × 6 × 4 = 168
```

**Decision**: Moderate score. Consider breaking into phases (start with one platform) to improve Ease score.

---

## ICE vs RICE Comparison / So Sánh ICE và RICE

### When to Use ICE

**Use ICE when:**
- ✅ Need quick decisions (1-2 hours)
- ✅ Don't have detailed user data
- ✅ Early stage / brainstorming phase
- ✅ Internal features or experiments
- ✅ Growth hacking experiments
- ✅ Small team with limited resources
- ✅ Rapid iteration cycles

**Best For:**
- Startups in early stages
- Growth experiments (A/B tests)
- Internal tooling decisions
- Quick wins identification
- Hackathon projects

### When to Use RICE

**Use RICE when:**
- ✅ Have user data and metrics
- ✅ Making major prioritization decisions
- ✅ Need justification for stakeholders
- ✅ Features with measurable reach
- ✅ Quarterly planning
- ✅ Budget allocation decisions
- ✅ Cross-functional coordination needed

**Best For:**
- Established products with analytics
- Roadmap planning
- Stakeholder alignment
- Resource-intensive projects
- Public-facing features

### Key Differences

| Aspect | ICE | RICE |
|--------|-----|------|
| **Complexity** | Simple (3 factors) | More complex (4 factors) |
| **Data Needed** | Minimal | Requires user data |
| **Time Required** | 1-2 hours | Half day to full day |
| **Precision** | Lower | Higher |
| **Best For** | Speed | Accuracy |
| **Reach Factor** | Not included | Included (quantitative) |

---

## Common Mistakes & Pitfalls / Lỗi Thường Gặp

### 1. Scoring Based on Personal Preference

**Mistake**: Giving high Impact scores to features you personally like.

**Fix**:
- Base Impact on user research and data
- Consider business value, not personal taste
- Ask: "Would users pay for this?" or "Would this reduce churn?"

### 2. Overestimating Confidence

**Mistake**: Scoring 8-9 on Confidence without real evidence.

**Fix**:
- Be honest about what you don't know
- Score 5-6 for "logical assumptions"
- Only score 8+ if you have solid data
- Default to lower scores when uncertain

### 3. Underestimating Complexity (Overscoring Ease)

**Mistake**: Scoring 7-8 on Ease because "it seems simple."

**Fix**:
- Consult with engineers before scoring
- Remember: Most features are 2x harder than they seem
- Factor in testing, documentation, deployment
- Consider technical debt and dependencies

### 4. Not Considering Opportunity Cost

**Mistake**: Scoring features in isolation without considering alternatives.

**Fix**:
- Score multiple features together for comparison
- Ask: "What are we NOT building if we build this?"
- Relative scoring is more important than absolute scores

### 5. Using Only Average or Only Multiplication

**Mistake**: Sticking to one formula without understanding the difference.

**Fix**:
- Use Average for general prioritization
- Use Multiplication when you want to heavily penalize low scores
- Understand: Multiplication amplifies differences

### 6. Scoring Without Team Input

**Mistake**: PM scores alone without engineering, design, or data input.

**Fix**:
- Score as a team
- Get engineering input on Ease
- Get data/research input on Confidence
- Get business input on Impact

### 7. Not Revisiting Scores

**Mistake**: Scoring once and never updating as you learn more.

**Fix**:
- Revisit scores after user research
- Update Confidence as you get data
- Adjust Ease after technical discovery
- Keep scores as living documents

### 8. Treating ICE as Absolute Truth

**Mistake**: Following ICE scores blindly without considering context.

**Fix**:
- ICE is a tool, not a rule
- Consider strategic priorities
- Factor in team morale and learning opportunities
- Sometimes build low-scoring features for strategic reasons

---

## ICE Scoring Template / Mẫu Chấm Điểm ICE

### Quick Scoring Sheet

```markdown
## Feature: [Feature Name]

### Context
[Brief description of the feature and why it's being considered]

### ICE Scoring

**Impact (1-10): __**
- User Value: [How does this help users?]
- Business Value: [Revenue/retention/adoption impact?]
- Strategic Alignment: [Fits product vision?]
- Score Justification: [Why this score?]

**Confidence (1-10): __**
- Evidence Type: [Proven data / Strong evidence / Moderate / Weak / None]
- Evidence Description: [What data/research do you have?]
- Risks/Uncertainties: [What could go wrong?]
- Score Justification: [Why this score?]

**Ease (1-10): __**
- Development Time: [Hours / Days / Weeks / Months]
- Technical Complexity: [Simple / Moderate / Complex]
- Dependencies: [None / Some / Many]
- Testing/Deployment Risk: [Low / Medium / High]
- Score Justification: [Why this score?]

### Final Calculation

**Average Method:**
```
ICE = (Impact + Confidence + Ease) / 3
ICE = (__ + __ + __) / 3 = __
```

**Multiplication Method:**
```
ICE = Impact × Confidence × Ease
ICE = __ × __ × __ = __
```

### Decision
- [ ] Build now (Score: 7+)
- [ ] Build later (Score: 5-7)
- [ ] Backlog (Score: 3-5)
- [ ] Don't build (Score: <3)

### Notes
[Additional context, dependencies, or considerations]
```

---

## Tips for Effective ICE Scoring / Mẹo Chấm Điểm Hiệu Quả

### 1. Score in Batches

Score 5-10 features together for better comparison. Relative ranking matters more than absolute scores.

### 2. Time-Box Your Scoring

Spend 10-15 minutes per feature maximum. ICE is meant to be fast.

### 3. Use Half-Point Scores

If struggling between 7 and 8, use 7.5. Precision helps with close calls.

### 4. Start with Ease

Score Ease first (easiest to estimate), then Confidence, then Impact. Builds momentum.

### 5. Document Your Reasoning

Write 1-2 sentences justifying each score. Helps with future revisits and team alignment.

### 6. Review as a Team

15-minute team review of scores catches bias and builds consensus.

### 7. Focus on the Top 3

After scoring, focus deeply on the top 3 highest-scoring features. Ignore the rest for now.

### 8. Combine with Other Frameworks

Use ICE for quick filtering, then use RICE or Jobs-to-be-Done for deeper analysis of top candidates.

---

## Vietnamese Summary / Tóm Tắt Tiếng Việt

### ICE là gì?

ICE là framework ưu tiên đơn giản dùng 3 yếu tố:
- **Impact (Tác động)**: Giá trị tạo ra (1-10)
- **Confidence (Độ tự tin)**: Chắc chắn mức độ nào (1-10)
- **Ease (Dễ dàng)**: Dễ xây dựng thế nào (1-10)

### Công thức

**Phương pháp Trung bình** (đơn giản):
```
Điểm ICE = (Tác động + Độ tự tin + Dễ dàng) / 3
```

**Phương pháp Nhân** (nâng cao):
```
Điểm ICE = Tác động × Độ tự tin × Dễ dàng
```

### Khi nào dùng ICE?

✅ **Dùng ICE khi:**
- Cần quyết định nhanh
- Không có dữ liệu chi tiết
- Giai đoạn đầu sản phẩm
- Thử nghiệm tăng trưởng
- Công cụ nội bộ

❌ **Dùng RICE khi:**
- Có dữ liệu người dùng
- Quyết định quan trọng
- Cần thuyết phục stakeholder
- Tính Reach được

### Ví dụ thực tế

**Instagram Stories (2016)**:
- Tác động: 10 (Snapchat đang thống trị)
- Độ tự tin: 8 (Có team và tech)
- Dễ dàng: 6 (Cần infrastructure mới)
- **Điểm: 8.0** → Xây dựng → 500M+ người dùng mỗi ngày!

### Lỗi thường gặp

1. Chấm điểm theo sở thích cá nhân
2. Quá tự tin về Confidence
3. Đánh giá thấp độ phức tạp (Ease quá cao)
4. Không hỏi ý kiến team
5. Chấm một lần rồi không cập nhật

### Mẹo quan trọng

- Chấm theo nhóm (5-10 features cùng lúc)
- Giới hạn thời gian (10-15 phút/feature)
- Chấm cùng team (PM + Eng + Design)
- Ghi lý do cho từng điểm
- Cập nhật điểm khi có thêm thông tin

---

## Related Frameworks / Framework Liên Quan

### Prioritization Frameworks

1. **RICE Prioritization**
   - More detailed than ICE (adds Reach)
   - Better for established products
   - Requires more data

2. **MoSCoW Prioritization**
   - Categorization method (Must/Should/Could/Won't)
   - Complementary to ICE
   - Good for release planning

3. **Value vs Effort Matrix**
   - 2x2 matrix visualization
   - Simpler than ICE
   - Good for stakeholder communication

### Growth Frameworks

4. **AARRR (Pirate Metrics)**
   - Acquisition, Activation, Retention, Referral, Revenue
   - Use with ICE for growth experiments
   - Helps define Impact scores

5. **North Star Framework**
   - Defines key metric
   - Helps calibrate Impact scores
   - Strategic alignment tool

### Validation Frameworks

6. **Lean Startup / Build-Measure-Learn**
   - Complements ICE for experiments
   - Helps improve Confidence scores
   - Rapid iteration cycle

---

## Learning Resources / Tài Nguyên Học Tập

### Essential Reading

1. **"The Practical Advantage of the ICE Score"** by Growth Hackers (2017)
   - Original ICE framework explanation
   - Growth hacking context
   - https://blog.growthhackers.com/the-practical-advantage-of-the-ice-score-as-a-test-prioritization-framework-cdd5f0808d64

2. **"ICE vs RICE: Which Framework to Use"** by Userflow (2023)
   - Detailed comparison
   - When to use each
   - https://www.userflow.com/blog/ice-score-vs-rice-score

### Tools

3. **ProductPlan ICE Score Calculator**
   - Free online calculator
   - Template included
   - https://www.productplan.com/glossary/ice-scoring-model/

4. **Airtable ICE Scoring Template**
   - Collaborative scoring
   - Free template

### Books

5. **"Hacking Growth"** by Sean Ellis & Morgan Brown (2017)
   - ICE framework origin
   - Growth experimentation
   - Practical case studies

6. **"Inspired"** by Marty Cagan (2017)
   - Product management fundamentals
   - Prioritization context
   - Complements ICE usage

### Video Resources

7. **"Prioritization Frameworks for PMs"** by Product School
   - ICE explained with examples
   - Comparison with other methods

### Community Resources

8. **GrowthHackers Community**
   - ICE scoring discussions
   - Real-world examples
   - https://growthhackers.com

9. **Product Management Subreddit**
   - PM community discussions
   - Prioritization advice
   - https://reddit.com/r/ProductManagement

---

## Root Integration / Tích Hợp Root

### Using ICE in Root Workflow

**Phase 2: Prioritize & Decide** → Use `/phase2:ice` command

**When to Use in Root:**
- After gathering feature ideas (Phase 1)
- Before detailed planning (Phase 3)
- During backlog grooming
- For growth experiment prioritization

**ICE Complements:**
- **Jobs-to-be-Done**: Use JTBD to define Impact
- **User Story Mapping**: ICE scores help prioritize stories
- **PRD Creation**: High ICE scores justify detailed PRDs

**Root Scoring Examples:**

| Feature | Impact | Confidence | Ease | ICE Score | Priority |
|---------|--------|------------|------|-----------|----------|
| `/phase3:prd` command | 9 | 7 | 8 | 8.0 | High |
| Dark mode | 8 | 9 | 7 | 8.0 | High |
| Command autocomplete | 7 | 6 | 4 | 5.7 | Medium |
| Better error messages | 5 | 8 | 9 | 7.3 | High (Quick win) |
| Update logo | 2 | 10 | 10 | 7.3 | Low (Cosmetic) |

**Note**: "Better error messages" has lower Impact but high Ease, making it a quick win despite moderate overall score.

---

## Quick Reference Card / Thẻ Tham Khảo Nhanh

```
╔════════════════════════════════════════════════════════╗
║                   ICE SCORING CHEAT SHEET              ║
╠════════════════════════════════════════════════════════╣
║ FORMULA:                                               ║
║   Average: (I + C + E) / 3                             ║
║   Multiply: I × C × E                                  ║
╠════════════════════════════════════════════════════════╣
║ IMPACT (1-10): How valuable?                           ║
║   9-10 = Game-changer                                  ║
║   7-8  = High impact                                   ║
║   5-6  = Moderate                                      ║
║   3-4  = Low                                           ║
║   1-2  = Minimal                                       ║
╠════════════════════════════════════════════════════════╣
║ CONFIDENCE (1-10): How sure?                           ║
║   9-10 = Proven data                                   ║
║   7-8  = Good evidence                                 ║
║   5-6  = Some evidence                                 ║
║   3-4  = Weak evidence                                 ║
║   1-2  = No evidence                                   ║
╠════════════════════════════════════════════════════════╣
║ EASE (1-10): How easy?                                 ║
║   9-10 = Hours-days                                    ║
║   7-8  = 1-2 weeks                                     ║
║   5-6  = 1 month                                       ║
║   3-4  = 2-3 months                                    ║
║   1-2  = 3+ months                                     ║
╠════════════════════════════════════════════════════════╣
║ WHEN TO USE ICE:                                       ║
║   ✅ Need quick decisions                              ║
║   ✅ Limited data                                      ║
║   ✅ Early stage                                       ║
║   ✅ Growth experiments                                ║
║                                                        ║
║ WHEN TO USE RICE:                                      ║
║   ✅ Have user data                                    ║
║   ✅ Major decisions                                   ║
║   ✅ Need stakeholder buy-in                           ║
╠════════════════════════════════════════════════════════╣
║ DECISION GUIDE:                                        ║
║   7-10 = Build now                                     ║
║   5-7  = Build later                                   ║
║   3-5  = Backlog                                       ║
║   0-3  = Don't build                                   ║
╚════════════════════════════════════════════════════════╝
```

---

## Changelog / Lịch Sử Thay Đổi

### Version 1.0 (2025-11-20)
- Initial comprehensive ICE Scoring framework document
- Added detailed scoring guides for all three factors
- Included real-world examples (Instagram Stories)
- Added ICE vs RICE comparison
- Added common mistakes and pitfalls
- Added Vietnamese translations
- Added Root integration examples
- Added learning resources

---

**Remember**: ICE is a tool for speed, not precision. Use it to make fast, good-enough decisions. For critical features requiring precision, upgrade to RICE or more detailed analysis.

**Vietnamese**: ICE là công cụ cho tốc độ, không phải độ chính xác. Dùng nó để ra quyết định nhanh, đủ tốt. Với tính năng quan trọng cần độ chính xác cao, nâng cấp lên RICE hoặc phân tích chi tiết hơn.

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
