---
# Core Metadata
title: "Feature Adoption Framework"
title_vi: "Khung Chấp Nhận Tính Năng"
framework_type: "Metrics"
category: ["Product Management", "Metrics", "Features", "Analytics"]

# Origin & Authority
author: "Amplitude, Mixpanel, Product Analytics Community"
organization: "Product Analytics Industry"
year_developed: "2010s"
original_source: "Product analytics best practices"

# Root Integration
root_phase: ["Phase 5: Track Progress"]
root_commands: ["/phase5:adoption", "/phase5:features"]
when_to_use: "After launching features, to measure usage, identify adoption barriers, and optimize engagement"

# Difficulty & Time
complexity: "Medium"
estimated_time: "Ongoing tracking (1-2 weeks for initial setup)"
skill_level: "Intermediate"

# Classification
tags: ["feature-adoption", "metrics", "analytics", "product-analytics", "engagement"]
related_frameworks: ["AARRR Pirate Metrics", "Retention & Churn", "A/B Testing", "Product Metrics"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-21"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Guide"
    title: "The Complete Guide to Feature Adoption"
    url: "https://amplitude.com/blog/feature-adoption"
    author: "Amplitude"
    year: "2022"
  - type: "Article"
    title: "Measuring Feature Success"
    url: "https://mixpanel.com/blog/measuring-feature-success/"
    author: "Mixpanel"
    year: "2021"
---

# Feature Adoption Framework / Khung Chấp Nhận Tính Năng

## Overview / Tổng Quan

**English:**
Feature Adoption measures how many users discover, try, and regularly use new features. It's critical for understanding if your feature investments are paying off.

**The Feature Adoption Paradox:**
- You spend 80% of development time on features
- But 80% of features are rarely or never used
- **Solution**: Measure adoption to prioritize what matters

**Real Example - Facebook Stories:**
- **2017 Launch**: 20% adoption in 6 months
- **2018**: Improved discovery (added to top of feed)
- **2019**: 50% adoption
- **2020**: 500M daily active users
- **Key**: Measured adoption → identified barriers → optimized placement

**Vietnamese:**
Feature Adoption đo lường có bao nhiêu người dùng khám phá, thử và sử dụng thường xuyên các tính năng mới.

**Nghịch Lý Tính Năng:**
- Bạn dành 80% thời gian phát triển cho tính năng
- Nhưng 80% tính năng ít khi hoặc không bao giờ được dùng

---

## The 3 Stages of Adoption / 3 Giai Đoạn Chấp Nhận

**English:**

### Stage 1: Awareness (Discovery)
**Question**: Do users know the feature exists?
**Metric**: % of eligible users who saw the feature

### Stage 2: Trial (First Use)
**Question**: Do users try it?
**Metric**: % who performed the action at least once

### Stage 3: Regular Usage (Habit)
**Question**: Do users make it a habit?
**Metric**: % who use it repeatedly (e.g., 3+ times/month)

**Adoption Funnel:**
```
100% Total Users
  ↓
80% Awareness (saw the feature)
  ↓
40% Trial (tried it once)
  ↓
15% Regular Usage (use it 3+ times/month)
```

**Example - Gmail's Smart Compose:**
- **Awareness**: 90% (shown inline while typing)
- **Trial**: 45% (used at least once)
- **Regular Usage**: 20% (use weekly)
- **Insight**: Good awareness & trial, but only 20% find it useful

---

## Key Metrics / Chỉ Số Chính

**English:**

### 1. Feature Adoption Rate
**Formula**: (Users Who Used Feature / Total Active Users) × 100

**Example - Spotify's Discover Weekly:**
- Active users: 200M
- Used Discover Weekly: 60M
- **Adoption Rate = 30%**

### 2. Time to Adoption
**What**: How long until users try the feature?
**Good**: <7 days for most features
**Bad**: >30 days (users might not discover it)

### 3. Adoption Depth
**What**: How deeply do users engage?
**Levels**:
- **Shallow**: Used once, never again
- **Medium**: Used occasionally (monthly)
- **Deep**: Used regularly (weekly/daily)

**Example - LinkedIn's Feed:**
- **Shallow** (scroll only): 60% of users
- **Medium** (like/comment monthly): 25%
- **Deep** (post weekly): 5%

### 4. Feature Retention
**What**: Do users keep using it?
**Formula**: % of users who tried feature and still use it after 30/60/90 days

**Example - Instagram Reels:**
- Tried once: 80%
- Still using after 30 days: 50%
- **Feature Retention = 62.5%**

### 5. Stickiness (DAU/MAU)
**What**: Daily Active / Monthly Active for specific feature
**Good**: >20% for most features
**Excellent**: >40%

**Vietnamese:**

### Chỉ Số Chính:
1. **Tỷ Lệ Chấp Nhận**: % người dùng đã dùng tính năng
2. **Thời Gian Đến Chấp Nhận**: Bao lâu để thử?
3. **Độ Sâu Chấp Nhận**: Họ sử dụng sâu đến mức nào?
4. **Giữ Chân Tính Năng**: Họ có tiếp tục dùng không?
5. **Stickiness**: DAU/MAU của tính năng

---

## Measuring Adoption: Step-by-Step / Đo Lường Từng Bước

**English:**

### Step 1: Define Success Metrics BEFORE Launch
**Questions to Answer:**
- What counts as "using" the feature?
- What adoption rate = success?
- What timeline (30/60/90 days)?

**Example - Notion's Comments Feature:**
- **Success Metric**: 20% of teams use comments weekly
- **Timeline**: Within 60 days of launch
- **Measurement**: % of workspaces with ≥3 comments/week

### Step 2: Set Up Tracking
**Events to Track:**
1. **Exposure**: User saw the feature (impression)
2. **Interaction**: User clicked/engaged
3. **Completion**: User completed the action
4. **Repeat**: User did it again

**Example - Slack's Huddles Tracking:**
```javascript
// Exposure
track('huddle_button_viewed', {location: 'dm_header'})

// Interaction
track('huddle_started', {participants: 2})

// Completion
track('huddle_ended', {duration: 300}) // 5 mins

// Repeat
track('huddle_started', {is_repeat_user: true})
```

### Step 3: Segment Users
**Who's adopting vs. not adopting?**
- By persona (power users vs. casual)
- By plan (free vs. paid)
- By cohort (when they signed up)
- By behavior (engagement level)

**Example - Figma's Auto Layout:**
- **Designers** (core persona): 60% adoption
- **Developers** (secondary): 15% adoption
- **Insight**: Optimize for designers, not developers

### Step 4: Identify Barriers
**Why aren't users adopting?**
- **Awareness**: They don't know it exists
- **Discovery**: They can't find it
- **Understanding**: They don't get what it does
- **Value**: They don't see why they need it
- **Friction**: It's too hard to use

**How to Find Barriers:**
1. **Analytics**: Where do users drop off?
2. **User Interviews**: Ask non-adopters why
3. **Session Recordings**: Watch user behavior
4. **Surveys**: "Why haven't you tried X?"

### Step 5: Optimize Adoption
**Tactics by Barrier:**

| Barrier | Solution | Example |
|---------|----------|---------|
| **Low Awareness** | Announcements, in-app tooltips, emails | Notion's "What's New" modal |
| **Hard to Find** | Improve navigation, onboarding callouts | Gmail's prominent Smart Compose |
| **Don't Understand** | Educational content, demos, tutorials | Figma's YouTube tutorials |
| **No Perceived Value** | Show benefits, social proof, use cases | LinkedIn: "People who X get Y% more views" |
| **Too Much Friction** | Simplify UX, reduce steps | Dropbox's one-click sharing |

**Vietnamese:**

### Quy Trình Đo Lường:
1. **Xác Định Chỉ Số** trước khi ra mắt
2. **Thiết Lập Tracking**: Exposure → Interaction → Completion → Repeat
3. **Phân Khúc**: Ai đang chấp nhận? Ai không?
4. **Tìm Rào Cản**: Tại sao họ không dùng?
5. **Tối Ưu**: Giải quyết từng rào cản

---

## The Adoption Curve / Đường Cong Chấp Nhận

**English:**

**Rogers' Diffusion of Innovation (1962):**
```
        /‾‾‾‾‾‾‾‾\
       /          \
      /            \___
     /
    /
  Innovators Early   Early    Late      Laggards
   (2.5%)  Adopters Majority Majority   (16%)
           (13.5%)   (34%)    (34%)
```

**Feature Adoption Strategy by Segment:**

### 1. Innovators (2.5%)
- **Who**: Power users, tech enthusiasts
- **Strategy**: Beta access, early preview
- **Example**: GitHub Copilot X (invite-only beta)

### 2. Early Adopters (13.5%)
- **Who**: Opinion leaders, influencers
- **Strategy**: Exclusive launch, referral program
- **Example**: Clubhouse (invite-only initially)

### 3. Early Majority (34%)
- **Who**: Pragmatic users, need social proof
- **Strategy**: Case studies, testimonials, tutorials
- **Example**: Notion's public templates

### 4. Late Majority (34%)
- **Who**: Skeptical, need hand-holding
- **Strategy**: Simplify, customer support, incentives
- **Example**: Zoom's one-click join (no account needed)

### 5. Laggards (16%)
- **Who**: Resistant to change, use basics only
- **Strategy**: Don't force it, let them opt-in eventually
- **Example**: Gmail's new UI (optional for years)

**Vietnamese:**

### Đường Cong Chấp Nhận (Rogers):
1. **Người Đổi Mới** (2.5%): Power users
2. **Người Chấp Nhận Sớm** (13.5%): Opinion leaders
3. **Đa Số Sớm** (34%): Thực dụng, cần bằng chứng xã hội
4. **Đa Số Muộn** (34%): Hoài nghi, cần hướng dẫn
5. **Người Chậm Chân** (16%): Kháng cự thay đổi

---

## Adoption Tactics Library / Thư Viện Chiến Thuật

**English:**

### Tactic 1: In-App Announcements
**When**: Feature launches
**Format**: Modal, banner, tooltip
**Example**: Notion's "What's New" modal (appears once per user)

### Tactic 2: Progressive Disclosure
**What**: Show feature when contextually relevant
**Example**: Gmail's "Undo Send" appears after sending email

### Tactic 3: Empty States
**What**: Prompt feature use when area is empty
**Example**: Spotify's "Liked Songs" empty state → "Heart a song to see it here"

### Tactic 4: Gamification
**What**: Reward feature usage
**Example**: LinkedIn's "Complete your profile" (progress bar)

### Tactic 5: Social Proof
**What**: Show others using it
**Example**: Loom: "10 teammates watched your video"

### Tactic 6: Onboarding Integration
**What**: Include in new user onboarding
**Example**: Slack's guided tour includes Huddles

### Tactic 7: Email Campaigns
**When**: 7 days post-launch (users who haven't tried)
**Format**: "Have you tried X? Here's why it's useful"

### Tactic 8: Default-On
**What**: Enable by default, let users opt-out
**Example**: Gmail's Smart Reply (on by default)

**Vietnamese:**

### Chiến Thuật Tăng Adoption:
1. **Thông Báo Trong App**: Modal, banner, tooltip
2. **Progressive Disclosure**: Hiện khi phù hợp ngữ cảnh
3. **Empty States**: Gợi ý khi vùng trống
4. **Gamification**: Phần thưởng cho việc sử dụng
5. **Social Proof**: Hiển thị người khác đang dùng
6. **Tích Hợp Onboarding**: Bao gồm trong hướng dẫn
7. **Email Campaigns**: Nhắc nhở người chưa thử
8. **Default-On**: Bật mặc định, để opt-out

---

## Common Mistakes / Sai Lầm Thường Gặp

### Mistake 1: Building Without Adoption Plan
**Problem**: Launch feature, hope users find it
**Result**: Low adoption, wasted effort

**Solution**: Plan adoption strategy BEFORE building
- How will users discover it?
- What's the onboarding flow?
- How will we measure success?

### Mistake 2: Forcing Features on Users
**Problem**: Make feature mandatory, users revolt
**Example**: Instagram removing chronological feed → backlash

**Solution**: Gradual rollout, optional initially

### Mistake 3: Not Measuring Depth
**Problem**: Celebrating "90% tried it once" when only 5% use it regularly

**Solution**: Track regular usage, not just first use

### Mistake 4: Ignoring Non-Adopters
**Problem**: Only talking to fans, missing why others don't use it

**Solution**: Interview non-adopters
- "Why haven't you tried X?"
- "What would make you try it?"

### Mistake 5: No Iteration Post-Launch
**Problem**: Launch and move on to next feature

**Solution**: Monitor adoption for 90 days, iterate based on data

---

## Quick Reference / Tham Khảo Nhanh

### The 3 Stages
1. **Awareness**: Do they know it exists?
2. **Trial**: Do they try it?
3. **Regular Usage**: Do they keep using it?

### Key Metrics
- **Adoption Rate**: (Users Who Used / Total Users) × 100
- **Time to Adoption**: Days until first use
- **Feature Retention**: % still using after 30/60/90 days
- **Stickiness**: DAU/MAU for feature

### Adoption Benchmarks
- **Good**: 20-30% adoption within 90 days
- **Great**: 40%+ adoption
- **Sticky**: DAU/MAU > 20%

### Barriers to Adoption
1. Awareness (don't know it exists)
2. Discovery (can't find it)
3. Understanding (don't get it)
4. Value (don't see why)
5. Friction (too hard)

### Boosting Adoption
- In-app announcements
- Progressive disclosure
- Empty states
- Gamification
- Social proof
- Email campaigns
- Default-on (opt-out)

---

**Last Updated**: 2025-11-21
**Version**: 1.0
**Root Commands**: `/phase5:adoption`, `/phase5:features`
**Next Review**: 2025-12-21

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
