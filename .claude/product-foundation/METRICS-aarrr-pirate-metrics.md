---
# Core Metadata
title: "AARRR (Pirate Metrics)"
title_vi: "Chỉ Số Cướp Biển AARRR"
framework_type: "Metrics"
category: ["Product Management", "Growth", "Metrics", "Analytics"]

# Origin & Authority
author: "Dave McClure"
organization: "500 Startups"
year_developed: "2007"
original_source: "Startup Metrics for Pirates"

# Root Integration
root_phase: ["Phase 5: Track Progress", "Phase 6: Launch & Release"]
root_commands: ["/phase5:metrics", "/phase6:analytics"]
when_to_use: "When measuring product growth funnel, or optimizing user lifecycle"

# Difficulty & Time
complexity: "Medium"
estimated_time: "Ongoing tracking"
skill_level: "Intermediate"

# Classification
tags: ["metrics", "growth", "analytics", "funnel", "lifecycle"]
related_frameworks: ["ICE Scoring", "Cohort Analysis", "Hook Model"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-20"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Presentation"
    title: "Startup Metrics for Pirates (AARRR)"
    url: "https://www.slideshare.net/dmc500hats/startup-metrics-for-pirates-long-version"
    author: "Dave McClure"
    year: "2007"
  - type: "Article"
    title: "AARRR Framework: Metrics That Let Your StartUp Sound Like A Pirate Ship"
    url: "https://www.productplan.com/glossary/aarrr-framework/"
    author: "ProductPlan"
    year: "2024"
  - type: "Guide"
    title: "Understanding AARRR Pirate Metrics"
    url: "https://www.productplan.com/glossary/aarrr-framework/"
    author: "ProductPlan"
    year: "2024"
---

# AARRR (Pirate Metrics) / Chỉ Số Cướp Biển AARRR

## Overview / Tổng Quan

### English

AARRR is a framework for measuring product growth and user journey. It breaks down the user lifecycle into 5 stages, helping product teams identify where users are dropping off and where to focus optimization efforts.

**AARRR stands for:**
- **A**cquisition: How do users find you?
- **A**ctivation: Do they have a great first experience?
- **R**etention: Do they come back?
- **R**evenue: Do they pay?
- **R**eferral: Do they tell others?

### Vietnamese

AARRR là framework đo lường tăng trưởng sản phẩm và hành trình người dùng. Nó chia vòng đời người dùng thành 5 giai đoạn, giúp đội sản phẩm xác định nơi người dùng rời bỏ và nơi cần tập trung tối ưu hóa.

**AARRR là viết tắt của:**
- **A**cquisition (Thu hút): Người dùng tìm thấy bạn như thế nào?
- **A**ctivation (Kích hoạt): Họ có trải nghiệm đầu tiên tốt không?
- **R**etention (Giữ chân): Họ có quay lại không?
- **R**evenue (Doanh thu): Họ có trả tiền không?
- **R**eferral (Giới thiệu): Họ có nói với người khác không?

---

## Real Example - Dropbox's AARRR

**How Dropbox Applied AARRR:**
- **Acquisition**: SEO, ads, word of mouth → 100K visitors/month
- **Activation**: Upload first file within 5 minutes → 60% activation rate
- **Retention**: Use weekly for 3 months → 40% retention
- **Revenue**: Convert to paid plan → 4% conversion
- **Referral**: Invite friends for storage → 35% referral rate

---

## 📋 AARRR Framework Playbook for Root

### Stage 1: Acquisition (Thu Hút)

#### Definition

**English:** How do potential users discover Root?

**Vietnamese:** Người dùng tiềm năng tìm thấy Root như thế nào?

#### Key Questions

- Where are users coming from?
- Which channels work best?
- What's the cost per acquisition?

#### Metrics to Track

| Metric | Definition | Target for Root |
|--------|------------|----------------------|
| **Traffic sources** | GitHub, search, social, direct | Diversified channels |
| **Visitors** | Unique visitors per month | 5,000/month by Q2 |
| **Cost per visitor** | Marketing spend / visitors | <$2 (mostly organic) |
| **Channel conversion** | Visitors who install | 10-15% |

#### How to Measure for Root

```
Acquisition Rate = (New Users / Total Visitors) × 100%

Example:
- 1,000 visitors from GitHub
- 120 install Root
- Acquisition Rate = (120 / 1,000) × 100% = 12%
```

#### Optimization Tactics

- ✅ Improve GitHub README with clear value proposition
- ✅ Create demo videos showing capabilities
- ✅ Write blog posts about PM techniques
- ✅ Share on Product Hunt, Hacker News
- ✅ SEO optimization for "PM slash commands"

#### Common Mistakes

- ❌ Tracking only total traffic (need to track sources)
- ❌ Ignoring quality of traffic (bot vs real users)
- ❌ Not measuring time-to-install from first visit

#### Vietnamese Summary

**Định nghĩa truyền thống:** Làm thế nào người dùng tìm thấy bạn?

**Định nghĩa cho AI/Root:** Tương tự. Kênh marketing, word-of-mouth, tìm kiếm tự nhiên.

---

### Stage 2: Activation (Kích Hoạt)

#### Definition

**English:** Does the user have a great first experience and reach their "aha moment"?

**Vietnamese:** Người dùng có trải nghiệm đầu tiên tuyệt vời và đạt đến "khoảnh khắc aha" không?

#### Key Questions

- What's the first value users should experience?
- How long until they reach it?
- What percentage reaches the "aha moment"?

#### Activation Moments for Root

| Action | Why It Matters | Target Time |
|--------|---------------|-------------|
| **Install & setup** | Can they get started? | <5 minutes |
| **First command used** | Do they try it? | Within 10 minutes |
| **First PRD generated** | Do they see value? | Within 1 hour |
| **Use 3+ commands** | Are they exploring? | Within first session |

#### How to Define Activation for Root

**Activation = User successfully generates their first PRD or completes RICE scoring**

**Why?** Because that's when they think: "Wow, this actually saves me time!"

#### How to Measure

```
Activation Rate = (Users Who Reach Aha Moment / Total Sign-ups) × 100%

Example:
- 120 users install Root
- 72 users generate their first PRD within 24 hours
- Activation Rate = (72 / 120) × 100% = 60%
```

#### Optimization Tactics

- ✅ Add onboarding flow: "/start" command
- ✅ Provide examples: "Try /phase3:prd 'Dark mode feature'"
- ✅ Quick wins: Highlight easiest commands first
- ✅ Templates: Pre-filled examples for common use cases
- ✅ Time to value: Reduce steps to first success

#### Common Mistakes

- ❌ Defining activation too late (should be first value, not full adoption)
- ❌ Measuring installs instead of active usage
- ❌ Not tracking time to activation

#### Vietnamese Summary

**Định nghĩa truyền thống:** Người dùng trải nghiệm giá trị cốt lõi lần đầu (ví dụ: tạo một dự án).

**Định nghĩa cho AI/Root:** **Cuộc hội thoại thành công đầu tiên.** Người dùng đặt một câu hỏi có ý nghĩa và nhận được một câu trả lời hữu ích, khiến họ nghĩ "À, cái này hay đấy". Ví dụ: Người dùng hỏi "Tóm tắt chi tiêu tuần trước" và nhận được một bản tóm tắt hữu ích.

---

### Stage 3: Retention (Giữ Chân)

#### Definition

**English:** Do users come back and use Root regularly?

**Vietnamese:** Người dùng có quay lại và sử dụng Root thường xuyên không?

#### Key Questions

- How often do users return?
- When do they churn?
- What makes them stick?

#### Retention Cohorts

| Time Period | Good Retention | Target for Root |
|-------------|---------------|----------------------|
| **Day 1** | 40-60% | 50% |
| **Day 7** | 20-30% | 25% |
| **Day 30** | 10-15% | 15% |
| **Day 90** | 5-10% | 10% |

#### How to Measure

```
Retention Rate = (Users Active in Period / Users from Cohort) × 100%

Example (Day 7 retention):
- 100 users installed on March 1
- 28 users were active on March 8
- Day 7 Retention = (28 / 100) × 100% = 28%
```

#### Retention Curve Analysis

- **Flattening curve** = Good (users staying)
- **Steep decline** = Bad (users churning)
- **Uptick** = Great (users returning)

#### How to Improve Retention for Root

**1. Create Habits (Daily/Weekly Triggers):**
   - Weekly prioritization routine: "Every Monday, run /phase2:rice"
   - Daily standups: "Update status with /phase5:status"
   - Monthly retros: "Run /phase7:retro"

**2. Add Sticky Features:**
   - Personal templates (users customize)
   - History (users reference past PRDs)
   - Shortcuts (users build muscle memory)

**3. Re-engagement:**
   - Reminder: "You haven't prioritized in 2 weeks"
   - New features: "Try the new /phase6:checklist command"
   - Value reinforcement: "You've saved 15 hours this month"

#### Common Mistakes

- ❌ Not tracking cohorts (need to see if newer users retain better)
- ❌ Celebrating DAU growth without checking retention
- ❌ Not understanding why users churn

#### Vietnamese Summary

**Định nghĩa truyền thống:** Người dùng quay lại sử dụng sản phẩm (ví dụ: đăng nhập hàng ngày).

**Định nghĩa cho AI/Root:** **Sự tin tưởng và phụ thuộc.** Người dùng chủ động quay lại để đặt một câu hỏi _mới_, vì cuộc hội thoại trước đó đã giải quyết được vấn đề của họ. Đo lường tần suất các phiên hội thoại có giá trị, không phải số lần đăng nhập.

**Ví dụ thực tế:** Sau 2 tuần, người dùng quay lại hỏi "Làm thế nào để tôi lập ngân sách?".

---

### Stage 4: Revenue (Doanh Thu)

#### Definition

**English:** How do you monetize the product?

**Vietnamese:** Làm thế nào để kiếm tiền từ sản phẩm?

#### Key Questions

- What's the pricing model?
- What's the conversion rate?
- What's the lifetime value (LTV)?

#### Revenue Models for Root (Hypothetical)

| Model | Description | Example Pricing |
|-------|-------------|----------------|
| **Freemium** | Free basic, paid premium | Free for 50 items, $10/mo unlimited |
| **Usage-based** | Pay per command / item | $0.10 per PRD generated |
| **Team plan** | Per-seat pricing | $15/user/month |
| **Enterprise** | Custom pricing for large teams | $500/mo for 50 users |

#### Key Revenue Metrics

```
Conversion Rate = (Paid Users / Total Users) × 100%

Average Revenue Per User (ARPU) = Total Revenue / Total Users

Lifetime Value (LTV) = ARPU × Average Lifetime (months)

Example:
- 1,000 active users
- 40 paid users (4% conversion)
- $10/month ARPU
- 24-month average lifetime
- LTV = $10 × 24 = $240 per user
```

#### Pricing Strategy for Root

**Recommendation**: Value-based pricing
- Users save 5 hours/week on documentation
- If PM costs $50/hour → $250/week value
- Charge $20/month (8% of value) = Easy decision

#### How to Increase Revenue

1. **Improve conversion**: Better free-to-paid flow
2. **Increase ARPU**: Upsell premium features
3. **Reduce churn**: Keep paid users happy
4. **Expand use cases**: Team plans, enterprise

#### Common Mistakes

- ❌ Pricing too low (undervaluing your product)
- ❌ Not testing pricing (fear of changing prices)
- ❌ Charging before proving value (activate first, monetize second)

#### Vietnamese Summary

**Định nghĩa truyền thống:** Người dùng trả tiền.

**Định nghĩa cho AI/Root:** Có thể là đăng ký trả phí, hoặc là một phần của một nền tảng lớn hơn (ví dụ: trợ lý AI trong một ngân hàng giúp giữ chân khách hàng và giảm chi phí hỗ trợ).

---

### Stage 5: Referral (Giới Thiệu)

#### Definition

**English:** Do users recommend Root to others?

**Vietnamese:** Người dùng có giới thiệu Root cho người khác không?

#### Key Questions

- Do users tell colleagues?
- What's the viral coefficient?
- How do we incentivize referrals?

#### Referral Metrics

```
Viral Coefficient (K) = (Invites Sent / User) × (Conversion Rate of Invites)

Example:
- Each user invites 2 colleagues on average
- 30% of invites convert to users
- K = 2 × 0.30 = 0.6

If K > 1 → Viral growth (exponential)
If K < 1 → Need other acquisition channels
```

#### Referral Tactics for Root

**1. Built-in Sharing:**
   - Share PRD: "Export and share with team"
   - Collaboration: "Invite team to use Root"
   - Templates: "Share your custom templates"

**2. Incentive Programs:**
   - "Invite 3 colleagues → Get premium features free"
   - "Team discount: 20% off for 5+ users"

**3. Make It Remarkable:**
   - PRDs so good people ask "How did you create this?"
   - Time savings so obvious people notice
   - Features that spark conversations

**4. Social Proof:**
   - "Used by PMs at Google, Amazon, Netflix"
   - Testimonials from power users
   - Case studies showing ROI

#### How to Measure

```
Referral Rate = (New Users from Referrals / Total Users) × 100%

Example:
- 100 active users
- 15 new users came from referrals
- Referral Rate = (15 / 100) × 100% = 15%
```

#### Common Mistakes

- ❌ Building referral program before product is good
- ❌ Asking for referrals too early (need happy users first)
- ❌ Not tracking referral source

#### Vietnamese Summary

**Định nghĩa truyền thống:** Người dùng mời bạn bè.

**Định nghĩa cho AI/Root:** Người dùng nói với bạn bè: "Bạn nên hỏi [sản phẩm] về [vấn đề], nó đã giúp tôi rất nhiều." Giới thiệu dựa trên kết quả, không phải dựa trên phần thưởng.

**Ví dụ thực tế:** Người dùng đăng một câu trả lời thông minh của sản phẩm lên mạng xã hội.

---

## 🎯 AARRR Funnel Analysis for Root

### Complete Funnel Example

```
100,000 Website Visitors (Acquisition)
    ↓ 12% install
12,000 Installs (Acquisition)
    ↓ 60% activate
7,200 Activated Users (Activation)
    ↓ 25% retained Day 7
1,800 Active Users Week 1 (Retention)
    ↓ 15% retained Day 30
1,080 Active Users Month 1 (Retention)
    ↓ 4% convert to paid
43 Paid Users (Revenue)
    ↓ 15% refer colleagues
6 New Users from Referrals (Referral)
```

### Where to Focus

1. **Biggest drop-off** = Biggest opportunity
2. In example above: **Activation** (12K → 7.2K = 40% loss)
3. Fix: Improve onboarding, reduce time to first value

### How to Use AARRR for Root

1. Set baseline metrics for each stage
2. Measure weekly/monthly
3. Identify worst-performing stage
4. Run experiments to improve that stage
5. Move to next weakest stage

---

## 🎓 How to Apply AARRR

### Step-by-Step Implementation

**Step 1: Define Your Metrics**
- For each AARRR stage, define what "success" looks like
- Set realistic targets based on industry benchmarks
- Create tracking mechanisms (analytics, dashboards)

**Step 2: Measure Baseline**
- Run for 2-4 weeks to get baseline data
- Identify current conversion rates at each stage
- Calculate drop-off rates between stages

**Step 3: Identify Bottleneck**
- Find the stage with worst performance
- Understand why users are dropping off
- Talk to users, analyze behavior data

**Step 4: Run Experiments**
- Design experiments to improve bottleneck stage
- Test one change at a time
- Measure impact over 2-4 weeks

**Step 5: Iterate**
- If experiment works, keep it and move to next bottleneck
- If it doesn't work, try a different approach
- Continuously optimize weakest stage

---

## ⚠️ Common Mistakes to Avoid

### 1. Optimizing for Wrong Metrics

**Problem:** Optimizing for DAU (daily active users) may lead to encouraging meaningless questions just to inflate numbers.

**Solution:** Focus on **quality** of interactions, not just quantity.

### 2. Not Tracking Cohorts

**Problem:** You can't tell if newer users are retaining better than older users.

**Solution:** Always analyze retention by cohort (users who joined in same week/month).

### 3. Charging Before Proving Value

**Problem:** Asking for payment before users experience value leads to low conversion.

**Solution:** Activate first, monetize second. Let users experience the "aha moment" before asking for payment.

### 4. Building Referral Programs Too Early

**Problem:** Users won't refer if the product isn't good yet.

**Solution:** First make product remarkable, then add referral mechanics.

### 5. Ignoring Foundation Projects

**Problem:** AARRR may give low scores to infrastructure projects that are crucial for long-term success.

**Solution:** Have a separate "bucket" for platform investments that may not show immediate AARRR impact.

---

## 🔗 Related Frameworks

### Integration with Other PM Techniques

**1. Hook Model + AARRR**
- Hook Model focuses on creating habits (relevant to Retention)
- Use Hook Model to improve Day 7, Day 30 retention
- AARRR measures if the habit is actually forming

**2. ICE/RICE Scoring + AARRR**
- Use AARRR to identify which stage needs improvement
- Use RICE to prioritize experiments for that stage
- Example: If Activation is weak, score experiments to improve onboarding

**3. Cohort Analysis + AARRR**
- Break down AARRR by cohort (week/month)
- See if retention is improving over time
- Identify which cohorts are most valuable

**4. Customer Journey Mapping + AARRR**
- Journey Map shows qualitative user experience
- AARRR quantifies each stage of the journey
- Use both to understand "why" and "how many"

**5. Jobs to Be Done + AARRR**
- JTBD explains why users "hire" your product
- AARRR measures if you're delivering on that job
- Example: If job is "save time on documentation", track time saved in Activation

---

## 📊 AARRR Dashboard Template

### Recommended Metrics to Track

```
┌─────────────────────────────────────────────────────────────┐
│ AARRR Dashboard for Root                              │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│ ACQUISITION                                                  │
│ • Total Visitors: 5,000/month         Target: 5,000         │
│ • Install Rate: 12%                   Target: 10-15%        │
│ • Top Channel: GitHub (60%)                                 │
│                                                              │
│ ACTIVATION                                                   │
│ • Activation Rate: 60%                Target: 60%           │
│ • Time to First PRD: 45 min           Target: <1 hour       │
│ • Commands Used: 3.2                  Target: 3+            │
│                                                              │
│ RETENTION                                                    │
│ • Day 1: 50%                          Target: 50%           │
│ • Day 7: 28%                          Target: 25%           │
│ • Day 30: 15%                         Target: 15%           │
│                                                              │
│ REVENUE                                                      │
│ • Conversion Rate: 4%                 Target: 4%            │
│ • ARPU: $10/month                                           │
│ • LTV: $240                                                 │
│                                                              │
│ REFERRAL                                                     │
│ • Referral Rate: 15%                  Target: 10%           │
│ • Viral Coefficient: 0.6              Target: >0.5          │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

---

## 🌏 Vietnamese Summary / Tóm Tắt Tiếng Việt

### Triết Lý AARRR cho Phát Triển AI

Đo lường hành vi người dùng qua 5 giai đoạn. Đối với AI, định nghĩa của các giai đoạn này phải được điều chỉnh để phản ánh giá trị của một mối quan hệ, không phải là một công cụ.

### 5 Giai Đoạn AARRR

**A - Acquisition (Thu hút)**
- Làm thế nào người dùng tìm thấy bạn?
- Kênh marketing, word-of-mouth, tìm kiếm tự nhiên

**A - Activation (Kích hoạt)**
- Cuộc hội thoại thành công đầu tiên
- Người dùng đặt câu hỏi có ý nghĩa và nhận được câu trả lời hữu ích

**R - Retention (Giữ chân)**
- Sự tin tưởng và phụ thuộc
- Người dùng chủ động quay lại để đặt câu hỏi mới
- Đo lường tần suất các phiên hội thoại có giá trị

**R - Revenue (Doanh thu)**
- Người dùng trả tiền
- Có thể là đăng ký trả phí hoặc một phần của nền tảng lớn hơn

**R - Referral (Giới thiệu)**
- Người dùng nói với bạn bè về sản phẩm
- Giới thiệu dựa trên kết quả, không phải phần thưởng

### Những Sai Lầm Cần Tránh

1. **Tối ưu hóa cho sai chỉ số**: Tối ưu hóa cho DAU có thể dẫn đến việc khuyến khích các câu hỏi vô nghĩa. Tập trung vào **chất lượng** của sự tương tác.

2. **Không theo dõi cohort**: Cần xem liệu người dùng mới có giữ chân tốt hơn người dùng cũ không.

3. **Thu phí trước khi chứng minh giá trị**: Kích hoạt trước, kiếm tiền sau.

4. **Xây dựng chương trình giới thiệu quá sớm**: Sản phẩm phải tốt trước khi người dùng muốn giới thiệu.

5. **Bỏ qua các dự án nền tảng**: Các dự án cải thiện mô hình cốt lõi có thể có điểm AARRR thấp trong ngắn hạn nhưng cực kỳ quan trọng cho sự thành công lâu dài.

---

## 📚 Learning Resources

### Essential Reading

1. **Original Presentation**
   - [Startup Metrics for Pirates (AARRR)](https://www.slideshare.net/dmc500hats/startup-metrics-for-pirates-long-version)
   - Dave McClure, 500 Startups (2007)
   - The original deck that started it all

2. **ProductPlan Guide**
   - [AARRR Framework: Metrics That Let Your StartUp Sound Like A Pirate Ship](https://www.productplan.com/glossary/aarrr-framework/)
   - Comprehensive guide with modern examples

3. **Medium Deep Dive**
   - [The Pirate Metrics Framework (AARRR)](https://medium.com/@ms.mbalke/aarrr-framework-metrics-that-let-your-startup-sound-like-a-pirate-ship-e91d4082994b)
   - Practical implementation guide

### Video Resources

- **Dave McClure's Original Talk**: Search "Startup Metrics for Pirates Dave McClure" on YouTube
- **Modern AARRR Examples**: Look for case studies from successful startups

### Tools for Tracking AARRR

- **Analytics**: Google Analytics, Mixpanel, Amplitude
- **Cohort Analysis**: Mixpanel, Amplitude
- **Dashboards**: Looker, Tableau, Metabase
- **A/B Testing**: Optimizely, VWO

---

## 🚀 Quick Start Checklist

Use this checklist to implement AARRR for your product:

- [ ] Define success metrics for each AARRR stage
- [ ] Set up analytics tracking for all 5 stages
- [ ] Measure baseline for 2-4 weeks
- [ ] Create AARRR dashboard
- [ ] Identify biggest drop-off stage
- [ ] Talk to users to understand why they're dropping off
- [ ] Design 3 experiments to improve bottleneck stage
- [ ] Run experiments for 2-4 weeks
- [ ] Measure impact and iterate
- [ ] Move to next weakest stage

---

## 💡 Key Takeaways

1. **AARRR measures the complete user lifecycle** from discovery to referral
2. **Focus on the biggest drop-off** - that's your biggest opportunity
3. **Activation is often the most important stage** - if users don't see value fast, they churn
4. **Retention is the foundation of growth** - without retention, acquisition is wasted
5. **For AI products, focus on quality of interactions** over quantity of usage
6. **Measure cohorts, not just aggregates** - understand if you're improving over time
7. **Use AARRR with other frameworks** - combine with RICE, JTBD, Hook Model for better decisions

---

## Related Files

- [ICE Scoring](./ice-scoring.md) - Prioritize experiments to improve AARRR stages
- [RICE Scoring](./rice-scoring.md) - Score feature ideas based on AARRR impact
- [Hook Model](./hook-model.md) - Build habits to improve Retention
- [Customer Journey Mapping](./customer-journey-mapping.md) - Understand qualitative experience at each AARRR stage
- [Jobs to Be Done](./jobs-to-be-done.md) - Understand why users "hire" your product (impacts all AARRR stages)

---

**Last Updated**: 2025-11-20
**Version**: 1.0
**Maintained by**: Root Team

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
