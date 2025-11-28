---
# Core Metadata
title: "Product Roadmapping"
title_vi: "Lộ Trình Sản Phẩm"
framework_type: "Strategy"
category: ["Product Management", "Strategy", "Planning", "Communication"]

# Origin & Authority
author: "Various (Prodpad, Atlassian, Aha!)"
organization: "Product Management Community"
year_developed: "2000s-2010s"
original_source: "Evolved from Agile movement, popularized by product tools"

# Root Integration
root_phase: ["Phase 3: Document & Plan", "Phase 4: Implement & Execute"]
root_commands: ["/phase3:roadmap", "/phase4:plan"]
when_to_use: "When communicating product strategy, planning features, or aligning stakeholders on direction"

# Difficulty & Time
complexity: "Medium"
estimated_time: "1-2 days for initial roadmap, quarterly updates"
skill_level: "Intermediate"

# Classification
tags: ["roadmap", "planning", "strategy", "communication", "prioritization", "stakeholder-management"]
related_frameworks: ["OKRs", "User Story Mapping", "Product Strategy", "Now-Next-Later"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-21"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Book"
    title: "Product Roadmaps Relaunched"
    author: "C. Todd Lombardo, Bruce McCarthy, et al."
    year: "2017"
  - type: "Article"
    title: "The Product Roadmap is Dead. Long Live the Product Roadmap."
    url: "https://www.prodpad.com/blog/lean-product-roadmap/"
    author: "Janna Bastow (ProdPad)"
    year: "2015"
  - type: "Article"
    title: "How to Build a Product Roadmap"
    url: "https://www.atlassian.com/agile/product-management/product-roadmaps"
    author: "Atlassian"
    year: "2018"
---

# Product Roadmapping / Lộ Trình Sản Phẩm

## Overview / Tổng Quan

**English:**
A product roadmap is a strategic document that outlines the vision, direction, and progress of your product over time. It's the "story" of where your product is going and why.

**Roadmap ≠ Project Plan**
- ❌ Not a promise of specific features by specific dates
- ✅ A strategic guide showing direction and priorities
- ❌ Not a Gantt chart with dependencies
- ✅ A communication tool for alignment

**What a Roadmap Communicates:**
1. **Vision**: Where are we going long-term?
2. **Strategy**: How will we get there?
3. **Priorities**: What matters most right now?
4. **Progress**: What have we done? What's next?

**Why Roadmaps Matter:**
- **Alignment**: Get everyone rowing in same direction
- **Focus**: Say "no" to off-strategy requests
- **Trust**: Show stakeholders you have a plan
- **Communication**: Single source of truth

**Real Example - Spotify (2016):**

**Traditional Roadmap (What They Avoided):**
```
Q1: Launch Discover Weekly
Q2: Build family plan
Q3: Add podcasts
Q4: Launch in 10 new countries
```
Problem: Too specific, feels like commitment

**Spotify's Approach (Outcome-based):**
```
Theme: Personalization
Goal: Help users discover music they'll love
Bets:
  - Algorithmic playlists (Discover Weekly)
  - AI-powered radio
  - Personalized homepage

Theme: Market Expansion
Goal: Reach 1B users
Bets:
  - Family & student plans
  - Emerging markets entry
```
Result: Flexibility to pivot while maintaining strategic focus

**Vietnamese:**
Roadmap sản phẩm là tài liệu chiến lược phác thảo tầm nhìn, hướng đi và tiến độ của sản phẩm theo thời gian.

**Roadmap ≠ Kế hoạch dự án**
- Không phải lời hứa tính năng theo ngày cụ thể
- Là hướng dẫn chiến lược cho thấy ưu tiên

**Roadmap Truyền Đạt:**
1. Tầm nhìn: Đi đâu dài hạn?
2. Chiến lược: Đến đó như thế nào?
3. Ưu tiên: Gì quan trọng nhất?
4. Tiến độ: Đã làm gì? Tiếp theo gì?

---

## Roadmap Types / Các Loại Roadmap

**English:**

### 1. Now-Next-Later Roadmap (Most Flexible)

**Structure:**
```
┌──────────┬──────────┬──────────┐
│   NOW    │   NEXT   │  LATER   │
│ (Doing)  │(Soon)    │(Future)  │
├──────────┼──────────┼──────────┤
│ Feature A│ Feature D│ Feature G│
│ Feature B│ Feature E│ Feature H│
│ Feature C│ Feature F│ Feature I│
└──────────┴──────────┴──────────┘
```

**When to Use:**
- Early-stage products (frequent changes)
- Agile environments
- Want maximum flexibility

**Pros:**
- No commitments to dates
- Easy to shift priorities
- Reduces pressure

**Cons:**
- Vague for stakeholders wanting dates
- Harder for resource planning

**Example - Buffer (Social Media Tool):**
```
NOW (Working on it):
  - Instagram integration
  - Analytics refresh
  - Mobile app bug fixes

NEXT (Up soon):
  - TikTok support
  - Team collaboration features
  - Advanced scheduling

LATER (Future):
  - AI-powered content suggestions
  - Video editing
  - Enterprise features
```

### 2. Theme-Based Roadmap (Strategic Focus)

**Structure: Organized by strategic themes, not features**

```
Theme 1: User Growth (Q1-Q2)
  - Referral program
  - Onboarding optimization
  - Social sharing

Theme 2: Engagement (Q2-Q3)
  - Push notifications
  - Daily challenges
  - Gamification

Theme 3: Monetization (Q3-Q4)
  - Premium tier
  - In-app purchases
  - Ad platform
```

**When to Use:**
- Mature products with clear strategy
- Multiple teams working in parallel
- Need to communicate "why" not just "what"

**Pros:**
- Connects features to strategy
- Easier to prioritize within themes
- Shows bigger picture

**Cons:**
- Less specific on timing
- May confuse stakeholders wanting feature list

**Example - Slack (2019):**
```
Theme: Enterprise Readiness
  - SSO (Single Sign-On)
  - Advanced admin controls
  - Compliance certifications
  - Audit logs

Theme: Developer Experience
  - New API v2
  - Block Kit (UI framework)
  - App directory improvements

Theme: Performance & Scale
  - Message indexing optimization
  - Reduce load times
  - Support for 100K+ user orgs
```

### 3. Timeline Roadmap (Traditional)

**Structure: Features on calendar timeline**

```
Q1 2025        Q2 2025        Q3 2025        Q4 2025
────────────────────────────────────────────────────
[Feature A]    [Feature C]    [Feature E]    [Feature G]
  [Feature B]    [Feature D]    [Feature F]
```

**When to Use:**
- Regulated industries (need dates)
- Hardware products (long lead times)
- Executive/board presentations

**Pros:**
- Clear timelines
- Easy to understand
- Good for planning

**Cons:**
- Feels like commitment
- Inflexible
- Dates often slip (looks bad)

**Best Practice**: Use ranges (Q1, H1) not specific dates (Jan 15)

### 4. Outcome-Based Roadmap (Modern Approach)

**Structure: Focus on goals/outcomes, not outputs**

```
Goal: Increase Activation Rate from 40% to 60%

Hypotheses to Test:
  - Simplified onboarding (reduce steps from 10 to 3)
  - In-app tutorials (video walkthroughs)
  - Empty state improvements (clear CTAs)

Success Metric: Activation rate @ 7 days
Timeline: Q1 2025
```

**When to Use:**
- Data-driven organizations
- Want to empower teams
- Focus on impact over output

**Pros:**
- Aligns with OKRs
- Measures success
- Allows for experimentation

**Cons:**
- Requires mature analytics
- Harder for external stakeholders

**Example - Amplitude (Product Analytics):**
```
Outcome: Reduce time-to-insight for new users

Key Results:
  - 50% of new users run first query in <5 min (currently 30%)
  - 80% create dashboard in week 1 (currently 45%)

Bets:
  - Guided onboarding flow
  - Pre-built chart templates
  - AI-powered query suggestions

Timeline: Q1 2025
Owner: Growth Team
```

**Vietnamese:**

### 4 Loại Roadmap:

**1. Now-Next-Later**: Linh hoạt nhất, không có ngày cụ thể
**2. Theme-Based**: Tổ chức theo chủ đề chiến lược
**3. Timeline**: Truyền thống, có lịch trình
**4. Outcome-Based**: Hiện đại, tập trung vào kết quả

---

## Building Your Roadmap: Playbook / Xây Dựng Roadmap

**English:**

### Step 1: Define Product Vision (Week 1)

**Vision Statement Template:**
"We believe [target users] should be able to [achieve outcome]. Currently, they [current problem]. We will solve this by [solution approach], which will result in [impact]."

**Example - Notion:**
"We believe knowledge workers should have one workspace for all their work. Currently, they juggle 10+ tools. We will solve this by building flexible Lego blocks that replace multiple tools, resulting in seamless workflows."

### Step 2: Set Strategic Themes (Week 1)

**Identify 3-5 Strategic Themes**
- What are your top priorities for next 6-12 months?
- Connect to company OKRs

**Example - Figma (2018):**
1. Performance (large file handling)
2. Collaboration (multiplayer features)
3. Developer handoff (design-to-code)
4. Community (templates, plugins)

### Step 3: Gather Input (Week 2)

**Sources of Input:**
- **Customer feedback**: Support tickets, user interviews, NPS surveys
- **Data**: Analytics, A/B tests, cohort analysis
- **Sales/CS**: What do prospects/customers request?
- **Engineering**: Technical debt, platform improvements
- **Leadership**: Company strategy, market trends
- **Competitive analysis**: What are others building?

**Capture in Opportunity Backlog:**
| Opportunity | Source | Theme | Impact | Effort |
|------------|--------|-------|--------|--------|
| Mobile app | Customers (50 requests) | Growth | High | High |
| Dark mode | Users (forums) | UX | Medium | Low |
| API webhooks | Developers | Platform | High | Medium |

### Step 4: Prioritize (Week 2)

**Use Prioritization Framework:**
- **RICE**: Reach × Impact × Confidence / Effort
- **ICE**: Impact × Confidence × Ease
- **Value vs Effort**: 2×2 matrix

**Plot on Matrix:**
```
High Impact
    ↑
    │   Quick Wins  │  Big Bets
    │   (do now)    │  (plan for)
    ├───────────────┼──────────────
    │   Fill-ins    │  Money Pits
    │   (if time)   │  (avoid)
    ↓
Low Impact
    Low Effort  →  High Effort
```

### Step 5: Sequence Features (Week 3)

**Considerations:**
1. **Dependencies**: What must be built first?
2. **Team capacity**: How many engineers/designers?
3. **Strategic timing**: Market windows, events
4. **Customer promises**: Commitments made?
5. **Technical constraints**: Infrastructure needs?

**Sequence Example:**
```
Q1: Foundation (auth, data model, API)
Q2: Core features (MVP functionality)
Q3: Polish (UX improvements, performance)
Q4: Scale (advanced features, integrations)
```

### Step 6: Create Roadmap Visual (Week 3)

**Choose Format:**
- Now-Next-Later (if high uncertainty)
- Theme-based (if strategic clarity)
- Timeline (if commitments needed)

**Tools:**
- **Spreadsheet**: Google Sheets (simple, collaborative)
- **Slides**: PowerPoint/Google Slides (presentations)
- **Roadmap tools**: Productboard, Aha!, ProductPlan
- **Jira/Linear**: If engineering-focused
- **Figma/Miro**: Custom visual design

**Example Structure (Theme-based):**
```
┌─────────────────────────────────────────────┐
│         PRODUCT ROADMAP - 2025              │
│         Vision: [Your vision]               │
├─────────────────────────────────────────────┤
│ THEME 1: User Growth (Q1-Q2)                │
│   • Referral program                        │
│   • Onboarding v2                           │
│   • Social login                            │
│                                             │
│ THEME 2: Engagement (Q2-Q3)                 │
│   • Push notifications                      │
│   • In-app messaging                        │
│   • Gamification                            │
│                                             │
│ THEME 3: Monetization (Q3-Q4)               │
│   • Premium tier                            │
│   • Team plans                              │
│   • Usage-based pricing                     │
└─────────────────────────────────────────────┘
```

### Step 7: Socialize & Get Buy-in (Week 4)

**Present to Stakeholders:**
1. **Leadership**: Get strategic alignment
2. **Engineering**: Validate feasibility
3. **Sales/CS**: Set expectations
4. **Marketing**: Align campaigns
5. **Entire company**: Transparency and alignment

**Key Slides:**
- Vision & strategy (why)
- Themes & priorities (what)
- Roadmap visual (when)
- Success metrics (how we'll measure)
- What's NOT on roadmap (manage expectations)

### Step 8: Communicate Ongoing (Monthly)

**Regular Updates:**
- **Monthly**: Review progress, adjust priorities
- **Quarterly**: Major roadmap revision
- **Annually**: Strategic planning

**Communication Channels:**
- Public roadmap (for customers)
- Internal wiki (for team)
- All-hands presentation
- Sales/CS enablement sessions

**Vietnamese:**

### Quy Trình 8 Bước:

1. **Định Nghĩa Tầm Nhìn**: Vision statement
2. **Đặt Chủ Đề Chiến Lược**: 3-5 themes
3. **Thu Thập Đầu Vào**: Customers, data, sales, engineering
4. **Ưu Tiên**: RICE, ICE, Value vs Effort
5. **Sắp Xếp Tính Năng**: Dependencies, capacity, timing
6. **Tạo Visual**: Chọn định dạng, tool
7. **Xã Hội Hóa**: Present to stakeholders
8. **Giao Tiếp Liên Tục**: Monthly updates, quarterly revisions

---

## Real Roadmap Examples / Ví Dụ Thực Tế

### Example 1: Linear (Project Management)

**Public Now-Next-Later Roadmap:**

```
NOW (Shipping this cycle):
  ✓ Keyboard shortcuts v2
  ⚡ Custom views
  ⚡ Advanced search

NEXT (Next few cycles):
  • Roadmaps (meta!)
  • Time tracking
  • Dependencies

LATER (Future):
  • Resource planning
  • Portfolio management
  • Mobile apps (iOS, Android)

💡 Note: Not commitments, priorities shift based on feedback
```

**Why It Works:**
- Transparent (public roadmap)
- No dates = flexibility
- Shows progress (checkmarks)

### Example 2: GitHub (2019-2020)

**Theme-Based Approach:**

```
THEME: Actions & CI/CD
Goal: Make GitHub the platform for entire dev workflow
  • GitHub Actions (general availability)
  • Marketplace for actions
  • Self-hosted runners
  • Advanced workflow features

THEME: Security
Goal: Make GitHub the most secure dev platform
  • Code scanning
  • Secret scanning
  • Dependency updates (Dependabot)
  • Security advisories

THEME: Collaboration
Goal: Improve remote team productivity
  • Discussions
  • Improved notifications
  • Draft PRs
  • Auto-merge

THEME: Enterprise
Goal: Support large enterprises at scale
  • Advanced compliance features
  • Audit log streaming
  • SAML improvements
```

**Why It Works:**
- Strategic themes clear
- Goals explain "why"
- Mix of new features + improvements

### Example 3: Superhuman (Email Client)

**Outcome-Based Roadmap (Internal):**

```
Q1 2020:
Outcome: Reduce inbox overwhelm
Metrics: Time to inbox zero, email anxiety score
Bets:
  - Inbox split (important vs other)
  - Remind me later
  - Smart triage

Q2 2020:
Outcome: Increase team adoption
Metrics: % of team using Superhuman
Bets:
  - Team analytics dashboard
  - Shared snippets
  - Team onboarding program

Q3 2020:
Outcome: Expand beyond executives
Metrics: User diversity (roles, industries)
Bets:
  - Gmail import improvements
  - Pricing tiers
  - Expanded onboarding capacity
```

**Why It Works:**
- Tied to outcomes (not just features)
- Measurable success criteria
- Experimentation mindset ("bets")

---

## Common Mistakes / Sai Lầm Thường Gặp

### Mistake 1: Feature Factory Roadmap
**Problem**: Long list of features with no strategy
**Solution**: Start with themes/goals, features are means to end

### Mistake 2: Overly Specific Dates
**Problem**: "Launch X on March 15, 2025"
**Solution**: Use ranges (Q1, H1) or Now-Next-Later

### Mistake 3: Too Much Detail
**Problem**: Every small feature, bug fix, tech debt item
**Solution**: Roadmap = strategic items, backlog = everything else

### Mistake 4: Never Saying No
**Problem**: Adding every request to roadmap
**Solution**: "That's interesting, but doesn't align with our strategy right now"

### Mistake 5: Set and Forget
**Problem**: Create roadmap once, never update
**Solution**: Living document, monthly reviews, quarterly revisions

### Mistake 6: One Roadmap for Everyone
**Problem**: Same roadmap for executives, engineers, customers
**Solution**: Multiple views:
  - **Executives**: Strategic themes, business outcomes
  - **Engineering**: Technical details, dependencies
  - **Customers**: Value propositions, benefits
  - **Sales**: Competitive positioning, timelines

### Mistake 7: Roadmap = Commitment
**Problem**: Stakeholders treat roadmap as promise
**Solution**:
  - Clear disclaimer: "Subject to change"
  - Outcome-focused (not output)
  - Educate on uncertainty

---

## Roadmap Communication / Giao Tiếp Roadmap

**English:**

### Internal Communication

**For Executives:**
- Focus: Strategic themes, business impact, resource allocation
- Format: High-level, visual, ties to OKRs
- Frequency: Monthly reviews, quarterly planning

**For Engineering:**
- Focus: Technical details, dependencies, timelines
- Format: Jira, Linear, detailed specs
- Frequency: Weekly in sprint planning

**For Sales/CS:**
- Focus: Customer benefits, competitive advantages, release dates
- Format: One-pager, FAQ, demo videos
- Frequency: Pre-release training, monthly updates

**For Entire Company:**
- Focus: Vision, progress, celebrate wins
- Format: All-hands presentation
- Frequency: Quarterly

### External Communication (Public Roadmap)

**Should You Have Public Roadmap?**

**Pros:**
- Transparency builds trust
- Reduces support load ("Is X coming?")
- Collects feedback early
- Competitive advantage (if innovative)

**Cons:**
- Competitors see plans
- Customers upset if you change
- Pressure to deliver

**Companies with Public Roadmaps:**
- Linear, GitHub, Notion, Buffer, Trello

**Best Practices:**
- Use Now-Next-Later (not dates)
- Clear disclaimer
- Voting/feedback mechanism
- Regular updates

**Vietnamese:**

### Giao Tiếp Roadmap:

**Nội bộ:**
- Executives: Themes, impact
- Engineering: Details, timeline
- Sales/CS: Benefits, dates
- Company: Vision, progress

**Công khai:**
- Ưu: Minh bạch, giảm support, feedback
- Nhược: Đối thủ thấy, kỳ vọng cao
- Thực hành: Now-Next-Later, disclaimer

---

## Roadmap Tools / Công Cụ

### Dedicated Roadmap Tools
- **Productboard**: Feature voting, prioritization, roadmaps
- **Aha!**: Strategic planning, roadmaps, integrations
- **ProductPlan**: Visual timeline roadmaps
- **Roadmunk**: Timeline and swim-lane roadmaps
- **ProdPad**: Now-Next-Later focused

### General Tools
- **Jira**: Agile/engineering roadmaps
- **Linear**: Modern issue tracking with roadmaps
- **Asana**: Project management with timeline view
- **Notion**: Flexible database for roadmaps
- **Airtable**: Spreadsheet-database hybrid

### Simple/Free Options
- **Google Sheets**: Lightweight, collaborative
- **Google Slides**: For presentations
- **Miro/Figma**: Custom visual roadmaps
- **Trello**: Kanban-style roadmap

**Recommendation**: Start simple (spreadsheet), upgrade as needed

---

## Related Frameworks / Khung Liên Quan

### OKRs (Objectives & Key Results)
**Relationship**: OKRs → Roadmap
- OKRs define what to achieve
- Roadmap shows how (features/initiatives)

### User Story Mapping
**Relationship**: Story Map → Roadmap releases
- Story map = feature breakdown
- Roadmap = when features ship

### Product Strategy
**Relationship**: Strategy → Roadmap
- Strategy = why and where
- Roadmap = what and when

---

## Quick Reference Card / Thẻ Tham Khảo Nhanh

### Roadmap Types
| Type | When to Use | Flexibility |
|------|-------------|-------------|
| Now-Next-Later | Early stage, high uncertainty | Highest |
| Theme-Based | Clear strategy, mature product | High |
| Timeline | Need dates, regulated industry | Low |
| Outcome-Based | Data-driven, OKR culture | High |

### Roadmap Checklist
- [ ] Vision statement clear
- [ ] Strategic themes defined (3-5)
- [ ] Features tied to themes
- [ ] Prioritized (data-driven)
- [ ] Right format for audience
- [ ] Disclaimer added ("subject to change")
- [ ] Success metrics defined
- [ ] Socialized with stakeholders
- [ ] Communication plan in place
- [ ] Review cadence set (monthly/quarterly)

### Red Flags
- ❌ Specific dates months out
- ❌ 50+ items on roadmap
- ❌ No strategic themes
- ❌ Never updated
- ❌ No "why" for items

### Green Lights
- ✅ Outcome-focused
- ✅ Strategic themes clear
- ✅ Right level of detail
- ✅ Living document
- ✅ Aligned with OKRs

---

**Last Updated**: 2025-11-21
**Version**: 1.0
**Root Commands**: `/phase3:roadmap`, `/phase4:plan`
**Next Review**: 2025-12-21

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
