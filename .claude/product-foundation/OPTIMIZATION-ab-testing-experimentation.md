---
# Core Metadata
title: "A/B Testing & Experimentation Framework"
title_vi: "Khung Kiểm Thử A/B & Thử Nghiệm"
framework_type: "Optimization"
category: ["Product Management", "Optimization", "Analytics", "Data-Driven"]

# Origin & Authority
author: "Ronald Fisher, Google, Optimizely"
organization: "Various (Statistical methods 1920s, Digital 2000s)"
year_developed: "1920s (Statistics), 2000s (Digital)"
original_source: "The Design of Experiments (Fisher, 1935), Google's experimentation platform"

# Root Integration
root_phase: ["Phase 4: Implement & Execute", "Phase 5: Track Progress"]
root_commands: ["/phase4:experiment", "/phase5:optimize"]
when_to_use: "When optimizing features, testing hypotheses, or making data-driven product decisions"

# Difficulty & Time
complexity: "Medium-High"
estimated_time: "1-4 weeks per experiment (depends on traffic)"
skill_level: "Intermediate"

# Classification
tags: ["ab-testing", "experimentation", "optimization", "data-driven", "hypothesis-testing", "statistics"]
related_frameworks: ["North Star Framework", "AARRR Pirate Metrics", "Feature Adoption", "Product Analytics"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-21"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Book"
    title: "Trustworthy Online Controlled Experiments"
    author: "Ron Kohavi, Diane Tang, Ya Xu"
    year: "2020"
  - type: "Article"
    title: "The Surprising Power of Online Experiments"
    url: "https://hbr.org/2017/09/the-surprising-power-of-online-experiments"
    author: "Ron Kohavi, Stefan Thomke"
    year: "2017"
  - type: "Article"
    title: "How to Run an A/B Test That Actually Works"
    url: "https://www.reforge.com/blog/how-to-run-ab-tests"
    author: "Reforge"
    year: "2019"
---

# A/B Testing & Experimentation Framework / Khung Kiểm Thử A/B & Thử Nghiệm

## Overview / Tổng Quan

**English:**
A/B testing (also called split testing) is a method of comparing two versions of something to determine which performs better. It's the scientific method applied to product development.

**How A/B Testing Works:**
1. Create two versions: A (control) and B (variant)
2. Randomly split users into two groups
3. Show Version A to one group, Version B to the other
4. Measure which version performs better on your goal metric
5. If statistically significant, ship the winner

**Why A/B Testing Matters:**
- **Data > Opinions**: Stop arguing, start testing
- **Small Changes = Big Impact**: Changing button color from blue to green increased Bing's revenue by $80M/year
- **Avoid Mistakes**: Test before full rollout prevents disasters
- **Compound Growth**: 1% improvements add up (1.01^365 = 37.8x improvement)

**Real Example - Booking.com:**
- **Experiment**: Added "Only 1 room left!" urgency message
- **Hypothesis**: Urgency increases conversions
- **Result**: +10% booking rate
- **Impact**: $100M+ annual revenue increase
- **Scale**: Runs 25,000+ experiments per year

**Vietnamese:**
Kiểm thử A/B là phương pháp so sánh hai phiên bản để xác định cái nào hoạt động tốt hơn.

**Tại Sao Kiểm Thử A/B Quan Trọng:**
- Dữ liệu > Ý kiến cá nhân
- Thay đổi nhỏ = Tác động lớn
- Tránh sai lầm trước khi triển khai toàn diện
- Tăng trưởng tích lũy

**Ví Dụ - Booking.com:**
- Thêm thông báo "Chỉ còn 1 phòng!"
- Kết quả: +10% tỷ lệ đặt phòng
- Tác động: $100M+ doanh thu hàng năm
- Quy mô: 25,000+ thử nghiệm/năm

---

## The Experimentation Process / Quy Trình Thử Nghiệm

**English:**

### Step 1: Form a Hypothesis
**Format**: "If [we make this change], then [this metric] will [increase/decrease] because [reason]."

**Good Hypothesis Examples:**
- ✅ "If we add social proof (showing 5-star reviews), then signup conversion will increase by 10% because users trust peer validation"
- ✅ "If we reduce form fields from 10 to 5, then completion rate will increase by 20% because friction decreases"
- ✅ "If we change CTA button from 'Submit' to 'Get Started', then click-through rate will increase by 5% because it's more action-oriented"

**Bad Hypothesis Examples:**
- ❌ "If we make the button bigger, users will click more" (no specific metric, no reasoning)
- ❌ "Let's test red vs blue button" (no hypothesis, just testing colors randomly)

### Step 2: Choose Metrics

**Primary Metric (North Star):**
- The ONE metric you're trying to move
- Must be measurable, actionable, meaningful
- Example: Conversion rate, revenue per user, retention

**Secondary Metrics (Guardrails):**
- Metrics to ensure you're not breaking things
- Example: If testing faster checkout, ensure refund rate doesn't increase

**Counter Metrics:**
- Metrics that might move in opposite direction
- Example: If increasing free trial length, ensure paid conversions don't drop

**Example - Netflix:**
- **Primary**: Hours watched (engagement)
- **Secondary**: Account cancellation rate (don't increase churn)
- **Counter**: Content discovery (don't make it harder to find shows)

### Step 3: Determine Sample Size

**Key Concepts:**
- **Statistical Significance**: Confidence that result is real (not luck)
- **Power**: Probability of detecting a real effect
- **Minimum Detectable Effect (MDE)**: Smallest change you care about

**Standard Settings:**
- **Significance Level (α)**: 95% (p-value < 0.05)
- **Statistical Power (β)**: 80%
- **MDE**: Depends on current conversion rate

**Sample Size Calculator Formula:**
```
n = (Z_α/2 + Z_β)² × 2p(1-p) / (MDE)²

Where:
- Z_α/2 = 1.96 (for 95% confidence)
- Z_β = 0.84 (for 80% power)
- p = baseline conversion rate
- MDE = minimum detectable effect (e.g., 0.05 for 5%)
```

**Quick Reference:**
| Baseline Rate | MDE | Sample Size per Variant |
|--------------|-----|------------------------|
| 5% | 10% (0.5%) | 50,000 |
| 5% | 20% (1%) | 12,500 |
| 10% | 10% (1%) | 25,000 |
| 10% | 20% (2%) | 6,250 |

**Rule of Thumb**: Need ~2,500-10,000 users per variant for most tests

### Step 4: Run the Test

**Duration Guidelines:**
- **Minimum**: 1-2 weeks (capture weekly patterns)
- **Full business cycle**: Include weekends if behavior differs
- **Until significance**: Don't stop early (causes false positives)

**Common Durations:**
- **High traffic**: 1-2 weeks
- **Medium traffic**: 2-4 weeks
- **Low traffic**: 4-8 weeks

**Randomization:**
- Use proper randomization (user ID hash, not session)
- Ensure consistent experience (same user always sees same variant)
- 50/50 split for most tests

### Step 5: Analyze Results

**What to Check:**
1. **Statistical Significance**: Is p-value < 0.05?
2. **Practical Significance**: Is the lift worth shipping?
3. **Segment Analysis**: Does it work for all user groups?
4. **Temporal Stability**: Is effect consistent over time?

**Interpreting P-Values:**
- **p < 0.01**: Highly significant (< 1% chance of luck)
- **p < 0.05**: Significant (< 5% chance of luck)
- **p > 0.05**: Not significant (could be random)

**Example Result:**
```
Control (A):    5.2% conversion (10,000 users)
Variant (B):    6.0% conversion (10,000 users)
Lift:           +15.4%
P-value:        0.003 (significant)
95% CI:         [+5%, +26%]
Decision:       Ship it! ✅
```

### Step 6: Make a Decision

**Decision Framework:**
| Scenario | Action |
|----------|--------|
| Significant win (p < 0.05, positive lift) | Ship variant |
| Significant loss (p < 0.05, negative lift) | Keep control |
| Not significant (p > 0.05) | Keep control (or test longer) |
| Mixed results (segments differ) | Ship to winning segments only |

**Vietnamese:**

### Quy Trình 6 Bước:
1. **Đặt Giả Thuyết**: "Nếu [thay đổi], thì [chỉ số] sẽ [tăng/giảm] vì [lý do]"
2. **Chọn Chỉ Số**: Primary (mục tiêu), Secondary (bảo vệ), Counter (đối lập)
3. **Xác Định Mẫu**: Cần ~2,500-10,000 người/biến thể
4. **Chạy Thử Nghiệm**: 1-4 tuần, đảm bảo ngẫu nhiên
5. **Phân Tích**: Kiểm tra p-value < 0.05, phân tích phân khúc
6. **Quyết Định**: Ship nếu thắng có ý nghĩa thống kê

---

## Types of Experiments / Các Loại Thử Nghiệm

**English:**

### 1. A/B Test (Classic)
**What**: Test 2 versions (A vs B)
**When**: Simple changes (button color, copy, layout)
**Example**: Old headline vs new headline

### 2. A/B/n Test (Multi-variant)
**What**: Test 3+ versions (A vs B vs C vs D)
**When**: Multiple options to test
**Example**: Testing 4 different pricing pages
**Caution**: Need more traffic (split across more variants)

### 3. Multivariate Test (MVT)
**What**: Test multiple elements simultaneously
**When**: Want to understand interaction effects
**Example**: Testing headline × image × CTA button (2 × 3 × 2 = 12 combinations)
**Caution**: Need LOTS of traffic

### 4. Sequential Testing
**What**: Analyze data continuously, stop when confident
**When**: High traffic, need faster results
**Tool**: Bayesian methods, SPRT (Sequential Probability Ratio Test)

### 5. Bandit Algorithm
**What**: Dynamically allocate traffic to winning variant
**When**: Minimizing regret (lost conversions during test)
**Example**: Email subject line testing (quickly shift to winner)

**Vietnamese:**

### Các Loại:
1. **A/B**: 2 phiên bản
2. **A/B/n**: 3+ phiên bản
3. **Multivariate**: Nhiều yếu tố cùng lúc
4. **Sequential**: Phân tích liên tục
5. **Bandit**: Phân bổ động sang bên thắng

---

## Real Experimentation Examples / Ví Dụ Thực Tế

### Example 1: Google - 41 Shades of Blue
**Test**: Tested 41 shades of blue for link color
**Hypothesis**: Optimal blue increases click-through rate
**Result**: Found best blue, increased revenue by $200M/year
**Lesson**: Small details matter at scale

### Example 2: Airbnb - Professional Photography
**Test**: Offered free professional photos to hosts
**Hypothesis**: Better photos → higher booking rate
**Result**: +2.5x booking rate for listings with pro photos
**Decision**: Invested $10M in photographer network
**Impact**: $1B+ revenue increase

### Example 3: Netflix - Artwork Testing
**Test**: Different thumbnail images for same show
**Hypothesis**: Personalized artwork increases play rate
**Result**: +20-30% higher engagement with personalized thumbnails
**Scale**: Tests artwork for every title, every user

### Example 4: HubSpot - Homepage CTA
**Test**: "Get Started Free" vs "Start Free Trial"
**Hypothesis**: "Get Started" feels less committal
**Result**: +24% click-through rate
**Lesson**: Word choice matters

### Example 5: Obama Campaign 2008
**Test**: 4 media (images/video) × 6 CTAs = 24 combinations
**Result**: Best combo increased signups by 40.6%
**Impact**: 2.8M more signups, $60M additional donations
**Lesson**: Experimentation wins elections

---

## Common Pitfalls & How to Avoid / Sai Lầm Thường Gặp

### Pitfall 1: Peeking (Checking Results Too Early)
**Problem**: Stopping test as soon as you see significance
**Why It's Wrong**: Increases false positive rate (Type I error)
**Solution**:
- Decide sample size upfront
- Only check results at predetermined milestones
- Use sequential testing methods if you must peek

### Pitfall 2: Testing Too Many Things at Once
**Problem**: Running 10 experiments simultaneously on same page
**Why It's Wrong**: Experiments interact, pollute each other's results
**Solution**:
- Test one primary element at a time
- Use experimentation calendar to avoid collisions
- If must overlap, ensure tests target different pages/flows

### Pitfall 3: Insufficient Sample Size
**Problem**: Declaring winner with 100 users per variant
**Why It's Wrong**: High variance, likely false positive
**Solution**:
- Calculate required sample size before starting
- Rule of thumb: minimum 2,500-5,000 per variant
- For small changes, need even more

### Pitfall 4: Ignoring Novelty Effect
**Problem**: New design performs better initially, then regresses
**Why It's Wrong**: Users attracted to change, not actual improvement
**Solution**:
- Run test for at least 2-4 weeks
- Analyze cohorts separately (new users vs returning)
- Look for sustained lift over time

### Pitfall 5: Local Maximum Trap
**Problem**: Incrementally optimizing to local peak, missing bigger opportunity
**Example**: Testing button colors when entire flow is broken
**Solution**:
- Balance exploitation (A/B tests) with exploration (bigger bets)
- Occasionally test radical redesigns
- Use qualitative research alongside A/B tests

### Pitfall 6: Shipping Non-Significant Results
**Problem**: "Well, it looks promising even though p = 0.15..."
**Why It's Wrong**: Likely due to random chance
**Solution**:
- Stick to p < 0.05 threshold
- If borderline, run test longer
- Don't lower bar post-hoc

### Pitfall 7: Ignoring Practical Significance
**Problem**: "We got 0.01% lift and it's statistically significant!"
**Why It's Wrong**: Not worth engineering effort
**Solution**:
- Define MDE (Minimum Detectable Effect) upfront
- Consider cost-benefit (dev time vs impact)
- Only ship if practically meaningful

---

## Advanced Topics / Chủ Đề Nâng Cao

### Segmentation Analysis
Don't just look at overall results—analyze by segment:
- **New vs Returning Users**: New users might react differently
- **Geography**: US vs Europe vs Asia
- **Device**: Mobile vs Desktop
- **User Type**: Free vs Paid, Power users vs Casual

**Example - Pinterest:**
Tested new layout, overall neutral result. But:
- New users: +10% (liked simplified interface)
- Power users: -5% (lost productivity)
- Decision: Ship to new users only

### Network Effects
Be careful with tests that affect user interactions:
- Example: If you test "invite friends" feature, control group doesn't benefit from invited friends
- Solution: Cluster randomization (entire networks in same group)

### Long-term Effects
Some changes have delayed impact:
- Example: Aggressive notification might increase short-term engagement but long-term churn
- Solution: Track long-term metrics (30-day, 90-day retention)

---

## Experimentation Tools / Công Cụ

### A/B Testing Platforms
- **Optimizely**: Enterprise platform, visual editor
- **VWO**: Easy setup, good for marketing tests
- **Google Optimize**: Free, integrates with Analytics
- **LaunchDarkly**: Feature flags + experimentation
- **Split.io**: Developer-focused feature flagging

### Statistical Tools
- **Evan's Awesome A/B Tools**: Sample size calculator
- **AB Test Calculator**: Significance testing
- **Python statsmodels**: For custom analysis
- **R**: Advanced statistical analysis

### Analytics Platforms
- **Amplitude Experiment**: Built into product analytics
- **Mixpanel**: Experimentation + analytics
- **Heap**: Auto-capture + testing

---

## When to Use A/B Testing / Khi Nào Sử Dụng

### Use A/B Testing When:
- ✅ You have sufficient traffic (>10K visitors/month)
- ✅ Testing incremental improvements
- ✅ Need data-driven decision between options
- ✅ Change is reversible
- ✅ You can measure impact within weeks

### Don't Use A/B Testing When:
- ❌ Insufficient traffic (<1K visitors/month) - use analytics/qualitative
- ❌ Testing radical redesign (use phased rollout instead)
- ❌ Impact is long-term (>3 months to see results)
- ❌ Change is irreversible (e.g., pricing change for existing customers)
- ❌ Ethical concerns (don't test harmful experiences)

---

## Related Frameworks / Khung Liên Quan

### North Star Framework
**Relationship**: A/B testing optimizes North Star metric
- North Star defines WHAT to optimize
- A/B testing determines HOW to optimize it

### AARRR Pirate Metrics
**Relationship**: Test improvements across funnel
- Use A/B tests to improve each AARRR stage
- Acquisition, Activation, Retention, Referral, Revenue

### Feature Adoption Framework
**Relationship**: Test feature rollout strategies
- A/B test onboarding flows
- Test feature discoverability

---

## Quick Reference Card / Thẻ Tham Khảo Nhanh

### Experiment Checklist
- [ ] Hypothesis formed (If X, then Y, because Z)
- [ ] Primary metric defined
- [ ] Secondary/counter metrics identified
- [ ] Sample size calculated
- [ ] Randomization strategy decided
- [ ] Test duration planned (1-4 weeks)
- [ ] Tracking implemented correctly
- [ ] Analysis plan documented
- [ ] Decision criteria defined (what constitutes success?)

### Key Formulas
**Statistical Significance**: p < 0.05 (95% confidence)
**Conversion Lift**: (B - A) / A × 100%
**Required Sample Size**: Use calculator for your baseline + MDE

### Decision Matrix
| P-value | Lift | Decision |
|---------|------|----------|
| < 0.05 | Positive | Ship it |
| < 0.05 | Negative | Keep control |
| > 0.05 | Any | Keep control or test longer |

### Common Sample Sizes
- **High impact test** (10-20% expected lift): 2,500-5,000 per variant
- **Medium impact** (5-10% lift): 5,000-10,000 per variant
- **Small impact** (<5% lift): 10,000-50,000 per variant

---

**Last Updated**: 2025-11-21
**Version**: 1.0
**Root Commands**: `/phase4:experiment`, `/phase5:optimize`
**Next Review**: 2025-12-21

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
