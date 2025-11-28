---
# Core Metadata
title: "Retention & Churn Analysis"
title_vi: "Phân Tích Giữ Chân & Rời Bỏ"
framework_type: "Metrics"
category: ["Product Management", "Metrics", "Growth", "Analytics"]

# Origin & Authority
author: "Brian Balfour, Lenny Rachitsky, Various"
organization: "Reforge, Growth practitioners"
year_developed: "2010s"
original_source: "Reforge Growth Series, industry best practices"

# Root Integration
root_phase: ["Phase 5: Track Progress"]
root_commands: ["/phase5:retention", "/phase5:churn", "/phase5:metrics"]
when_to_use: "When analyzing why users leave, predicting churn, or improving long-term retention"

# Difficulty & Time
complexity: "Medium-High"
estimated_time: "Ongoing analysis (2-4 weeks for initial setup)"
skill_level: "Intermediate-Advanced"

# Classification
tags: ["retention", "churn", "metrics", "analytics", "cohort", "growth"]
related_frameworks: ["Cohort Analysis", "Product-Market Fit", "AARRR Pirate Metrics", "North Star Framework"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-21"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Article"
    title: "Retention is the Silent Killer"
    url: "https://brianbalfour.com/essays/retention-is-the-silent-killer"
    author: "Brian Balfour"
    year: "2015"
  - type: "Guide"
    title: "How to Improve User Retention"
    url: "https://www.lennysnewsletter.com/p/how-to-improve-retention"
    author: "Lenny Rachitsky"
    year: "2021"
  - type: "Book"
    title: "The Lean Analytics"
    author: "Alistair Croll & Benjamin Yoskovitz"
    year: "2013"
---

# Retention & Churn Analysis / Phân Tích Giữ Chân & Rời Bỏ

## Overview / Tổng Quan

**English:**
Retention measures how many users continue using your product over time. Churn is the opposite - users who stop using your product. These are the most important metrics for sustainable growth.

**Why Retention Matters More Than Acquisition:**
- Acquiring new users is 5-25x more expensive than retaining existing ones
- A 5% increase in retention can increase profits by 25-95%
- High retention = Product-Market Fit
- Low retention = Leaky bucket (no amount of growth will save you)

**The Leaky Bucket Analogy:**
```
New Users (pouring water in) → Your Product (bucket) → Churned Users (water leaking out)

If the leak is bigger than the pour, the bucket never fills!
```

**Real Example - Netflix:**
- **Monthly Churn**: ~2.5% (97.5% retention)
- **Annual Retention**: ~70%
- **Key**: They obsess over retention (recommendation algorithm, original content, smooth UX)
- **Result**: 230M subscribers, $30B revenue

**Vietnamese:**
Retention đo lường có bao nhiêu người dùng tiếp tục sử dụng sản phẩm của bạn theo thời gian. Churn là ngược lại - người dùng ngừng sử dụng.

**Tại Sao Retention Quan Trọng Hơn Acquisition:**
- Thu hút người dùng mới đắt hơn 5-25 lần so với giữ chân
- Tăng 5% retention có thể tăng 25-95% lợi nhuận
- Retention cao = Product-Market Fit
- Retention thấp = Thùng thủng lỗ (tăng trưởng không thể cứu)

---

## Key Metrics / Chỉ Số Chính

**English:**

### 1. Retention Rate
**Formula**: (Users at End of Period / Users at Start) × 100

**Example**:
- Jan 1: 1,000 users signed up
- Feb 1: 700 still active
- **30-Day Retention = 70%**

**Retention Benchmarks by Industry:**
| Industry | Day 1 | Day 7 | Day 30 | Day 90 |
|----------|-------|-------|--------|--------|
| **Social Media** | 65% | 45% | 30% | 20% |
| **E-commerce** | 40% | 25% | 15% | 10% |
| **SaaS B2B** | 80% | 75% | 70% | 65% |
| **Gaming** | 50% | 25% | 10% | 5% |
| **Finance** | 85% | 80% | 75% | 70% |

### 2. Churn Rate
**Formula**: (Users Lost / Total Users at Start) × 100

**Example**:
- Jan 1: 1,000 users
- Jan 31: 50 users churned
- **Monthly Churn = 5%**

**Good vs. Bad Churn:**
| Product Type | Good Churn | Acceptable | Bad |
|-------------|------------|------------|-----|
| **B2B SaaS** | <2%/month | 2-5%/month | >5%/month |
| **Consumer Subscription** | <5%/month | 5-10%/month | >10%/month |
| **Consumer App** | <20%/month | 20-40%/month | >40%/month |

### 3. Net Retention (NDR/NRR)
**Formula**: (Revenue at End - Churned Revenue + Expansion) / Revenue at Start × 100

**Why It's Better Than Churn**: Accounts for upsells and expansions

**Example - Snowflake:**
- Start: $100K MRR from cohort
- Churned: -$10K
- Upsells: +$50K
- **Net Retention = ($100K - $10K + $50K) / $100K = 140%**

**Benchmarks:**
- **>120% = Excellent** (best-in-class SaaS)
- **100-120% = Good**
- **<100% = Problematic**

### 4. Cohort Retention Curve
**What**: Track retention by user cohort over time

**Example:**
```
Week 0: 100% (all new users)
Week 1: 40% still active
Week 2: 30%
Week 4: 25%
Week 8: 22%
Week 12: 20% ← Retention curve flattens (good sign!)
```

**Healthy Retention Curve**: Flattens (asymptotes to baseline)
**Unhealthy Curve**: Continues dropping to zero

**Vietnamese:**

### Chỉ Số Chính:
1. **Tỷ Lệ Giữ Chân** (Retention Rate): % người dùng còn lại
2. **Tỷ Lệ Rời Bỏ** (Churn Rate): % người dùng rời đi
3. **Giữ Chân Ròng** (Net Retention): Tính cả mở rộng và nâng cấp
4. **Đường Cong Cohort**: Retention theo thời gian

---

## The 3 Types of Retention / 3 Loại Retention

**English:**

### Type 1: Short-term Retention (Day 1, Day 7)
**What**: Did users come back after first use?
**Measures**: Activation quality, "aha moment" effectiveness
**Fix If Low**: Improve onboarding, reduce time-to-value

**Example - Duolingo:**
- D1 retention goal: 55%
- Fix: Gamification, streak system, push notifications
- Result: Improved D1 retention by 10%

### Type 2: Medium-term Retention (Day 30, Day 60)
**What**: Did users form a habit?
**Measures**: Product stickiness, habit formation
**Fix If Low**: Increase engagement triggers, add habit loops

**Example - Spotify:**
- D30 retention goal: 70%
- Fix: Personalized playlists (Discover Weekly), sharing features
- Result: Became daily habit for millions

### Type 3: Long-term Retention (Day 90+, Month 6+)
**What**: Is this a lasting solution?
**Measures**: Product-Market Fit, switching costs
**Fix If Low**: Add network effects, increase switching costs, continuous innovation

**Example - Slack:**
- M6 retention: 93%
- Reason: Team-wide adoption, integrations, searchable history = high switching cost

**Vietnamese:**

### 3 Loại Retention:
1. **Ngắn hạn** (Ngày 1, 7): Người dùng có quay lại không?
2. **Trung hạn** (Ngày 30, 60): Người dùng có hình thành thói quen không?
3. **Dài hạn** (Ngày 90+): Đây có phải giải pháp lâu dài không?

---

## Churn Analysis Framework / Khung Phân Tích Churn

**English:**

### Step 1: Measure Churn
**Define "Churned"**: When is a user considered churned?
- **B2B SaaS**: Canceled subscription or didn't renew
- **Consumer Subscription**: Canceled paid plan
- **Free Product**: No activity for 30/60/90 days (varies by product)

**Example - Instagram:**
- Churned = No login for 30 days
- They send re-engagement emails at day 7, 14, 21

### Step 2: Segment Churn
**Who is churning?** Break down by:
- **Cohort**: When did they sign up?
- **Acquisition Channel**: Where did they come from?
- **User Persona**: What type of user?
- **Feature Usage**: Which features did they (not) use?
- **Price Tier**: Free vs. paid?

**Example - Netflix Churn Segments:**
| Segment | Churn Rate | Insight |
|---------|-----------|---------|
| New users (< 1 month) | 8%/month | Poor onboarding |
| Light users (< 5 hrs/month) | 6%/month | Low engagement |
| Heavy users (> 20 hrs/month) | 1%/month | Highly engaged |
| Family plan | 1.5%/month | Higher value |
| Basic plan | 4%/month | More price-sensitive |

### Step 3: Identify Churn Reasons
**How to Find Why Users Churn:**

**Method 1: Exit Surveys**
Ask when users cancel: "Why are you leaving?"
- Too expensive (price objection)
- Don't use it enough (activation failure)
- Missing features (product gaps)
- Found alternative (competitive)
- No longer need it (use case ended)

**Method 2: Churn Prediction Model**
Identify behaviors that predict churn:
- Low engagement (< X sessions/week)
- Declining usage trend
- Haven't used key features
- Support tickets (frustration signals)
- Downgraded plan

**Example - Spotify Churn Signals:**
- User hasn't created a playlist (low investment)
- Declining listening hours
- Hasn't used mobile app (channel mismatch)
- Skips most recommendations (personalization failure)

**Method 3: Cohort Analysis**
Compare retained vs. churned users:
- What features did retained users adopt?
- What "aha moments" did they experience?
- What activation steps did they complete?

### Step 4: Prioritize Churn Reduction
**Calculate Impact:**
```
Churn Reduction Value = Churned Users × ARPU × Average Lifetime
```

**Example:**
- 100 users churning/month
- ARPU = $20/month
- Average lifetime = 12 months
- **Value of Reducing Churn by 10%** = 10 users × $20 × 12 = $2,400/month

**Prioritization Matrix:**
| Churn Reason | % of Churn | Effort to Fix | Priority |
|-------------|-----------|--------------|----------|
| Poor onboarding | 30% | Medium | HIGH |
| Missing features | 25% | High | MEDIUM |
| Too expensive | 20% | Low (packaging) | HIGH |
| Found competitor | 15% | High | LOW |
| Use case ended | 10% | N/A | N/A |

**Vietnamese:**

### Quy Trình Phân Tích Churn:
1. **Đo Churn**: Định nghĩa "churned" là gì
2. **Phân Khúc**: Ai đang churn?
3. **Tìm Nguyên Nhân**: Tại sao họ rời bỏ?
4. **Ưu Tiên**: Giải quyết nguyên nhân nào trước

---

## Retention Improvement Playbook / Hướng Dẫn Cải Thiện

**English:**

### Strategy 1: Improve Onboarding (Fix Short-term Retention)

**The "Aha Moment":**
- **Facebook**: Add 7 friends in 10 days
- **Slack**: 2,000 team messages sent
- **Dropbox**: 1 file added from 1 device
- **Twitter**: Follow 30 accounts

**Onboarding Checklist:**
- [ ] Identify your "aha moment" (what action predicts retention?)
- [ ] Reduce time-to-value (< 5 minutes ideal)
- [ ] Progressive disclosure (don't overwhelm)
- [ ] Personalize experience (ask about use case)
- [ ] Celebrate milestones (dopamine hits)

**Example - Duolingo Onboarding:**
1. Quick 5-minute lesson (immediate value)
2. Streak system explained (habit formation)
3. Personalized goal setting
4. Daily reminder setup
5. **Result**: 55% D1 retention (vs. 40% before)

### Strategy 2: Build Habits (Fix Medium-term Retention)

**The Hook Model (Nir Eyal):**
```
Trigger → Action → Variable Reward → Investment → (Repeat)
```

**Examples:**
| Product | Trigger | Action | Reward | Investment |
|---------|---------|--------|--------|------------|
| **Instagram** | Notification | Open app | New likes | Post photo |
| **Duolingo** | Daily reminder | Do lesson | XP + streak | Progress saved |
| **Slack** | @ mention | Reply | Conversation | Messages in history |

**Habit-Forming Tactics:**
- **Notifications**: Re-engage at right time (not spam)
- **Streaks**: Visualize consistency (Duolingo, Snapchat)
- **Social**: Add friends/teams (accountability)
- **Progress**: Show advancement (LinkedIn profile strength)
- **Personalization**: Content that improves over time

### Strategy 3: Increase Switching Costs (Fix Long-term Retention)

**Switching Cost Types:**
1. **Data**: Historical data hard to recreate (Evernote notes, Gmail history)
2. **Network**: Team/friends are there (Slack, WhatsApp)
3. **Integration**: Connected to other tools (Zapier, Salesforce)
4. **Learning**: Invested time learning (Photoshop, Excel)
5. **Financial**: Upfront costs or contracts (enterprise software)

**Example - Notion:**
- **Data**: Years of notes, wikis, databases
- **Network**: Team workspaces, shared docs
- **Integration**: Embedded content, API connections
- **Learning**: Custom templates, workflows
- **Result**: Very low churn once adopted

### Strategy 4: Win-Back Campaigns

**Re-engagement Email Sequence:**
- **Day 7**: "We miss you! Here's what's new"
- **Day 14**: "Your data is still here" (remind of investment)
- **Day 21**: "Special offer" (discount or feature unlock)
- **Day 30**: "Final chance" (create urgency)

**Example - Spotify Win-Back:**
- Email: "Your playlists miss you"
- Offer: 3 months for $9.99 (vs. normal $9.99/month)
- **Result**: 20% of lapsed users reactivated

**Vietnamese:**

### Chiến Lược Cải Thiện Retention:
1. **Cải Thiện Onboarding**: Giảm time-to-value, tìm "aha moment"
2. **Xây Dựng Thói Quen**: Hook Model, triggers, streaks
3. **Tăng Chi Phí Chuyển Đổi**: Dữ liệu, mạng lưới, tích hợp
4. **Chiến Dịch Win-Back**: Email re-engagement, ưu đãi

---

## Common Mistakes / Sai Lầm Thường Gặp

### Mistake 1: Focusing on Acquisition Over Retention
**Problem**: Adding users to a leaky bucket

**Example**: Startup spends $100K on ads, gains 10K users, but 90% churn in 30 days

**Solution**: Fix retention FIRST, then scale acquisition
- Rule of thumb: Don't scale until retention curve flattens

### Mistake 2: Not Defining Churn Correctly
**Problem**: Vague definition leads to misleading metrics

**Wrong**: "User hasn't logged in recently"
**Right**: "User hasn't performed core action in X days" (where X depends on product)

**Solution**: Define churn based on product usage pattern
- Daily product: 7 days inactive
- Weekly product: 30 days inactive
- Monthly product: 60 days inactive

### Mistake 3: Treating All Churn Equally
**Problem**: Not all churn is bad or preventable

**Types of Churn:**
- **Involuntary**: Credit card expired, payment failed (fixable!)
- **Voluntary - Use case ended**: Graduated, moved, etc. (unavoidable)
- **Voluntary - Product issue**: Missing features, too expensive (fixable!)

**Solution**: Segment and prioritize fixable churn

### Mistake 4: Ignoring Leading Indicators
**Problem**: Reacting to churn after it happens

**Better**: Predict churn and intervene early

**Leading Indicators:**
- Declining engagement
- Support tickets
- Feature abandonment
- Negative feedback

**Example - Intercom:**
- Tracks "health score" per account
- Alerts when score drops
- Customer success reaches out proactively
- **Result**: Reduced churn by 15%

---

## Quick Reference / Tham Khảo Nhanh

### Key Formulas
```
Retention Rate = (Users at End / Users at Start) × 100
Churn Rate = (Users Lost / Users at Start) × 100
Net Retention = (Revenue at End - Churn + Expansion) / Revenue at Start × 100
```

### Retention Benchmarks
- **B2B SaaS**: M1 = 90%+, M12 = 70%+
- **Consumer Subscription**: M1 = 60%+, M12 = 40%+
- **Social Apps**: D1 = 40%+, D30 = 20%+

### The Retention Curve
- **Healthy**: Flattens to baseline (asymptote)
- **Unhealthy**: Continues dropping to zero

### Churn Reduction Priority
1. Fix involuntary churn (payment issues)
2. Improve onboarding (aha moment)
3. Build habits (triggers + rewards)
4. Increase switching costs (data, network, integrations)
5. Win-back campaigns (re-engage churned users)

---

**Last Updated**: 2025-11-21
**Version**: 1.0
**Root Commands**: `/phase5:retention`, `/phase5:churn`
**Next Review**: 2025-12-21

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
