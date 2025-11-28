---
# Core Metadata
title: "Kano Model"
title_vi: "Mô Hình Kano"
framework_type: "Prioritization"
category: ["Product Management", "Prioritization", "User Satisfaction"]

# Origin & Authority
author: "Dr. Noriaki Kano"
organization: "Tokyo University of Science"
year_developed: "1984"
original_source: "Attractive Quality and Must-Be Quality"

# Root Integration
root_phase: ["Phase 2: Prioritize & Decide"]
root_commands: ["/phase2:kano"]
when_to_use: "When cross-functional teams disagree on feature priority, or need to balance must-haves vs delighters"

# Difficulty & Time
complexity: "Medium"
estimated_time: "1-2 weeks (survey + analysis)"
skill_level: "Intermediate"

# Classification
tags: ["prioritization", "customer-satisfaction", "feature-classification", "cross-functional", "survey"]
related_frameworks: ["RICE Prioritization", "Value Proposition Canvas", "Balanced Trade-Off Matrix"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-20"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Original Paper"
    title: "Attractive Quality and Must-Be Quality (May require account)"
    url: "https://www.scirp.org/reference/referencespapers?referenceid=1836954"
    author: "Noriaki Kano"
    year: "1984"
  - type: "Article"
    title: "The Kano Model: A Tool to Prioritize Features"
    url: "https://www.productplan.com/glossary/kano-model/"
    author: "ProductPlan"
    year: "2024"
  - type: "Article"
    title: "Kano Model in Product Management"
    url: "https://productschool.com/resources/glossary/kano-model"
    author: "Product School"
    year: "2024"
  - type: "Tutorial"
    title: "How to Use the Kano Model"
    url: "https://www.userpilot.com/blog/kano-model/"
    author: "Userpilot"
    year: "2024"
---

# Kano Model / Mô Hình Kano

## Overview

**English:**
The Kano Model, developed by Dr. Noriaki Kano in 1984, classifies product features based on how they affect customer satisfaction. It's incredibly powerful for handling cross-functional conflicts because it provides objective criteria for feature debates.

**When to use it:**
- Cross-functional teams disagree on feature priority
- Need to balance "must-haves" vs "delighters"
- Limited resources and must choose which features to cut
- Stakeholders want different things (UX wants delight, Ops wants stability)

**Vietnamese:**
Mô hình Kano, phát triển bởi Tiến sĩ Noriaki Kano năm 1984, phân loại tính năng sản phẩm dựa trên cách chúng ảnh hưởng đến sự hài lòng của khách hàng. Cực kỳ mạnh mẽ để xử lý xung đột giữa các phòng ban vì nó cung cấp tiêu chí khách quan cho các cuộc tranh luận về tính năng.

---

## The 5 Feature Categories

```
Customer
Satisfaction
    ↑
    |     Delighters (Excitement)
    |        /
    |       /
    |------/-------------- Performance
    |     /       /
    |    /       /
    |   /       /
----+--/-------/----------→ Feature Implementation
    | /       /
    |/       /  Basic (Must-Be)
    |       /
    |      /
    |     /
    ↓
```

### 1. Basic Features (Must-Be) - Nền Tảng Cơ Bản

**Definition**: Features that customers expect. Their absence causes major dissatisfaction, but their presence doesn't increase satisfaction.

**Characteristics:**
- Customers assume you have these
- Absence = deal breaker
- Presence = "Of course you have this"
- Example: Hotels must have clean sheets

**Root Examples:**
- `/phase1:idea` command must save the idea (if it doesn't, users leave)
- Search must return results
- Data must not be lost

**Questions to Identify:**
- "What would make you immediately stop using this product?"
- "What's the bare minimum this must do?"

---

### 2. Performance Features (Satisfiers) - Tính Năng Hiệu Suất

**Definition**: Features where more is better. Satisfaction increases linearly with implementation quality.

**Characteristics:**
- Better performance = higher satisfaction
- Poor performance = dissatisfaction
- Customers explicitly request these
- Competitive differentiator

**Root Examples:**
- RICE scoring speed: Faster = better
- PRD quality: More detailed = better satisfaction
- AI response time: Faster = better

**Questions to Identify:**
- "What would make you choose us over competitors?"
- "What do you wish worked better/faster/easier?"

---

### 3. Excitement Features (Delighters) - Tính Năng Gây Bất Ngờ

**Definition**: Features customers don't expect but love when they discover them. Creates "wow" moments.

**Characteristics:**
- Customers don't know to ask for these
- Absence doesn't hurt (users don't expect it)
- Presence creates delight and word-of-mouth
- Turns users into advocates

**Real-World Examples:**
- **Spotify Wrapped**: Nobody asked for it, everyone loves it
- **Gmail's "Undo Send"**: Didn't exist anywhere, now a favorite feature
- **Slack's emoji reactions**: Not in requirements, became iconic

**Root Examples:**
- AI auto-detects when you're prioritizing and suggests best framework
- Celebrates when you complete your first launch
- Learns your PM style and adapts recommendations

**Questions to Identify:**
- "What would make you tell your friends about us?"
- "What would unexpectedly delight you?"

---

### 4. Indifferent Features - Tính Năng Không Quan Trọng

**Definition**: Features that don't affect satisfaction either way.

**Characteristics:**
- Users don't care if you have it or not
- Waste of development resources
- Often requested by ONE loud customer
- Should be deprioritized

**Examples:**
- Dark mode for a tool used only during business hours
- Export to 15 different formats when users only need 2
- Customizable fonts in a B2B analytics tool

**Warning Sign:**
When only one stakeholder wants it, and no customers have requested it, it's probably indifferent.

---

### 5. Reverse Features - Tính Năng Ngược

**Definition**: Features that actually DECREASE satisfaction despite good intentions.

**Characteristics:**
- More functionality = less satisfaction
- Often adds complexity
- Annoys more users than it helps

**Real-World Examples:**
- **Microsoft Clippy**: "Looks like you're writing a letter!" (users hated it)
- **Auto-play videos**: Intended to increase engagement, actually annoyed users
- **Gamification in serious B2B tools**: Frivolous for enterprise users

**How to detect:**
User says: "Can you turn off [feature]?" or "This is getting in my way"

---

## How to Use the Kano Model: 6-Step Process

### Step 1: List All Potential Features

Create a comprehensive list of features under consideration.

**Example for Root v2.0:**
1. Instant PRD generation
2. Dark mode
3. Slack integration for notifications
4. AI auto-categorizes features
5. Custom templates
6. Collaboration (multiple users)
7. Version history
8. Mobile app
9. Export to Jira
10. Analytics dashboard

---

### Step 2: Create Kano Survey Questions

For EACH feature, ask TWO questions:

**Functional Question** (feature present):
"How would you feel if [feature] were present?"

**Dysfunctional Question** (feature absent):
"How would you feel if [feature] were absent?"

**Answer Options** (for both questions):
1. I like it
2. I expect it
3. I'm neutral
4. I can tolerate it
5. I dislike it

---

**Example for "Dark Mode" feature:**

**Functional**: "How would you feel if Root had dark mode?"
- User answers: "I like it" (nice to have)

**Dysfunctional**: "How would you feel if Root did NOT have dark mode?"
- User answers: "I'm neutral" (doesn't matter)

**Result**: Dark mode is a **Delighter** (nice but not critical)

---

**Example for "Data doesn't get lost" feature:**

**Functional**: "How would you feel if your PRDs and ideas were always saved and never lost?"
- User answers: "I expect it" (must have)

**Dysfunctional**: "How would you feel if Root sometimes lost your data?"
- User answers: "I dislike it" (deal breaker)

**Result**: Data persistence is a **Basic** feature (must-have)

---

### Step 3: Classify Each Feature

Use the Kano Evaluation Table:

| Dysfunctional → <br> Functional ↓ | Like | Expect | Neutral | Tolerate | Dislike |
|-----------------------------------|------|--------|---------|----------|---------|
| **Like** | Q | E | E | E | P |
| **Expect** | R | I | I | I | B |
| **Neutral** | R | I | I | I | B |
| **Tolerate** | R | I | I | I | B |
| **Dislike** | R | R | R | R | Q |

**Legend:**
- **B** = Basic (Must-be)
- **P** = Performance
- **E** = Excitement (Delighter)
- **I** = Indifferent
- **R** = Reverse
- **Q** = Questionable (user didn't understand question)

---

### Step 4: Survey Your Users

**Survey Size:**
- **B2C products**: 50-100 users minimum
- **B2B products**: 20-30 users (smaller user base)
- **Internal tools**: 10-15 users

**Pro Tip**: Segment by user type
- New users vs. power users often categorize features differently
- Enterprise vs. SMB have different must-haves

---

### Step 5: Calculate Results

Count how many users classified each feature in each category.

**Example Results for "Collaboration (multi-user)" feature:**

| Category | Count | Percentage |
|----------|-------|------------|
| Basic | 2 | 10% |
| Performance | 5 | 25% |
| Excitement | 8 | 40% |
| Indifferent | 4 | 20% |
| Reverse | 1 | 5% |

**Winner**: Excitement (40%) - It's a delighter!

---

### Step 6: Prioritize Using Kano + Effort Matrix

**Priority Framework:**

```
High Impact on Satisfaction
        ↑
        |  [Basic - Build First]    [Delighters - Build After Basics]
        |
        |  ─────────────────────────────────────────
        |
        |  [Performance - Build Next] [Indifferent - Skip]
        |
        └──────────────────────────────────────────→ Low Effort → High Effort
```

**Decision Rules:**

1. **Build ALL Basic features first** (regardless of effort)
   - If you don't have these, customers leave

2. **Build Performance features next** (prioritize by effort)
   - Low-effort performance features = quick wins
   - High-effort performance features = roadmap for later

3. **Build Excitement features if resources allow**
   - Start with low-effort delighters
   - Save high-effort delighters for when you have breathing room

4. **Skip Indifferent features**
   - Waste of resources

5. **Remove Reverse features**
   - They're hurting you

---

## Complete Example: Instant Refund Feature (Cross-Functional Conflict)

**Scenario**: Business Operations requests instant refund capability.

### The Conflict:
- **UX Team**: "Customers will love instant refunds! Must-build!"
- **Finance Team**: "Cashflow nightmare! This will destroy reconciliation!"
- **Product Team**: "Sounds complex and expensive..."
- **Operations Team**: "Current process takes 2-4 weeks, customers complain"

**Traditional Approach** (leads to endless meetings):
- Month 1: Finance says no
- Month 2: UX escalates to VP
- Month 3: Compromise on half-solution that satisfies nobody

---

### Kano Approach:

#### Step 1: Survey Customers

Ask 30 customers the Kano questions:

**Functional**: "How would you feel if refunds were instant (within 5 minutes)?"
**Dysfunctional**: "How would you feel if refunds took 2-4 weeks like today?"

**Results:**
- 70% said instant refunds are **Performance** feature
- 20% said it's **Basic** (must-have)
- 10% said **Indifferent**

**Interpretation**:
- Current 2-4 week wait is causing dissatisfaction
- Instant refunds would significantly increase satisfaction
- **This is important to customers**

---

#### Step 2: Assess Implementation Complexity

**Option A: Full Instant Digital Wallet**
- **Effort**: 6 months, 3 engineers
- **Risk**: High (cashflow, reconciliation, fraud)
- **Finance Impact**: Company fronts refund money before bank refunds

**Option B: Instant Credit/Store Balance**
- **Effort**: 1 month, 1 engineer
- **Risk**: Low (no cashflow risk)
- **Finance Impact**: Neutral (money stays in ecosystem)

**Option C: Expedited Refund (24-48 hours)**
- **Effort**: 2 weeks, process change
- **Risk**: Very low
- **Finance Impact**: Minimal

---

#### Step 3: Test with Kano + Customer Validation

Survey customers again with the 3 options:

| Option | Satisfaction Impact | Effort | Risk |
|--------|---------------------|--------|------|
| **Option A**: Instant wallet | +85% satisfaction | 6 months | High |
| **Option B**: Store credit | +60% satisfaction | 1 month | Low |
| **Option C**: 24-48hr refund | +45% satisfaction | 2 weeks | Very Low |

**Question**: "Which would you prefer?"
- 55% chose Option B (store credit)
- 30% chose Option A (instant wallet)
- 15% chose Option C (expedited)

**Key Finding**: Customers prefer Option B (store credit) because:
- "I'll probably buy again anyway"
- "I just don't want to wait 2-4 weeks"
- "Store credit is instant, that's what matters"

---

#### Step 4: Make Data-Driven Decision

**Recommendation to Leadership:**

"Based on Kano analysis + customer validation:
- **Phase 1** (Ship in 1 month): Instant store credit (Option B)
  - Satisfies 60% of dissatisfaction
  - Low risk, low effort
  - Finance team approves

- **Phase 2** (Roadmap for Q3): Instant wallet (Option A)
  - For customers who don't want store credit
  - More complex, but tackles remaining 40%"

**Result:**
- ✅ Finance happy: No cashflow risk in Phase 1
- ✅ UX happy: Customers get instant refunds
- ✅ Operations happy: Process simplified
- ✅ Product happy: Shipped in 1 month instead of 6
- ✅ Customers happy: 2-4 weeks → instant

**Everyone wins because Kano provided objective data instead of opinions.**

---

## Common Mistakes

| Mistake | Why It's Bad | Better Approach |
|---------|-------------|-----------------|
| **Building Delighters before Basics** | Customers leave before experiencing the delight | Always build Basic features first |
| **Assuming your opinion = customer opinion** | What YOU think is a must-have might be indifferent to users | Always survey real users |
| **Surveying only one user segment** | Enterprise users ≠ SMB users | Segment your survey by user type |
| **Ignoring effort** | Some basics are 3-month projects | Basic features with low effort = priority 1 |
| **Not re-running Kano periodically** | Delighters become Basics over time (e.g., mobile apps were delighters in 2010, basics in 2025) | Re-survey every 12-18 months |

---

## Vietnamese Summary

**Tóm Tắt:**

Mô hình Kano phân loại tính năng thành 5 loại:
- **Cơ bản**: Bắt buộc phải có (VD: dữ liệu không bị mất)
- **Hiệu suất**: Càng tốt càng hài lòng (VD: tốc độ phản hồi)
- **Gây bất ngờ**: Không mong đợi nhưng thích (VD: Spotify Wrapped)
- **Không quan trọng**: Người dùng không quan tâm
- **Ngược**: Làm giảm hài lòng (VD: Clippy của Microsoft)

Quy trình: Khảo sát người dùng với 2 câu hỏi (có/không có tính năng), phân loại, ưu tiên xây dựng Cơ bản trước, sau đó Hiệu suất, cuối cùng Gây bất ngờ.

---

## Related Frameworks

The Kano Model works particularly well when combined with other prioritization and validation frameworks:

### 1. RICE Prioritization
**File**: `/.claude/product-foundation/rice-prioritization.md`

**When to use together:**
- Kano tells you WHICH features matter to customers (Basic/Performance/Excitement)
- RICE tells you WHEN to build them (Reach, Impact, Confidence, Effort)

**Example workflow:**
1. Use Kano to categorize features (Basic/Performance/Excitement)
2. Use RICE to prioritize within each category
3. Result: Build high-RICE Basic features first, then high-RICE Performance, then high-RICE Excitement

---

### 2. Value Proposition Canvas
**File**: `/.claude/product-foundation/value-proposition-canvas.md`

**When to use together:**
- Value Proposition Canvas identifies customer pains and gains
- Kano validates which solutions create the most satisfaction

**Example workflow:**
1. Use Value Proposition Canvas to identify customer pains (e.g., "refunds take too long")
2. Brainstorm solutions (instant wallet, store credit, expedited)
3. Use Kano to validate which solution customers prefer
4. Result: Customer-validated solution that addresses real pains

---

### 3. Balanced Trade-Off Matrix
**File**: `/.claude/product-foundation/balanced-tradeoff-matrix.md`

**When to use together:**
- Kano shows customer satisfaction impact
- Balanced Trade-Off Matrix shows cross-functional constraints (Finance, Eng, Legal)

**Example workflow:**
1. Use Kano to identify must-have features (Basic)
2. Use Balanced Trade-Off Matrix to assess feasibility across teams
3. Result: Features that satisfy customers AND are feasible to build

**Real example from Instant Refund case:**
- Kano showed customers want instant refunds (Performance feature)
- Balanced Trade-Off Matrix revealed Finance constraints
- Solution: Store credit (satisfies Kano + passes Trade-Off Matrix)

---

## Learn More

### Books
- **"Attractive Quality and Must-Be Quality"** by Noriaki Kano (1984)
  - Original research paper introducing the Kano Model
  - Available on ResearchGate

- **"The Kano Model: A Manager's Guide to Understanding Customer Needs"** by Lou Cohen (1995)
  - Practical guide to implementing Kano in product development
  - Includes survey templates and case studies

- **"Inspired: How to Create Tech Products Customers Love"** by Marty Cagan (2017)
  - Chapter on customer validation mentions Kano Model
  - Context on when to use different prioritization methods

### Articles & Tutorials
- **ProductPlan**: "The Kano Model - A Tool to Prioritize Features"
  - URL: https://www.productplan.com/glossary/kano-model/
  - Beginner-friendly overview with visual examples

- **Product School**: "Kano Model in Product Management"
  - URL: https://productschool.com/resources/glossary/kano-model
  - Practical tips for PMs implementing Kano

- **Userpilot**: "How to Use the Kano Model"
  - URL: https://www.userpilot.com/blog/kano-model/
  - Step-by-step tutorial with templates

- **Mind the Product**: "Using the Kano Model to Prioritize Product Development"
  - Real-world case studies from product teams

- **Silicon Valley Product Group**: "Customer Discovery vs Feature Prioritization"
  - When to use Kano vs other methods

### Tools & Templates
- **Typeform**: Kano Model Survey Template
  - URL: https://www.typeform.com/templates/t/kano-model/
  - Pre-built survey with Kano questions

- **Google Forms**: Free Kano Survey Template
  - Customizable template for running Kano surveys

- **Excel/Sheets**: Kano Analysis Calculator
  - Spreadsheet templates for calculating Kano results
  - Available on ProductPlan and other PM resources

- **Miro**: Kano Model Workshop Template
  - Collaborative board for remote Kano workshops
  - Includes evaluation table and prioritization matrix

### Videos & Courses
- **YouTube - Product School**: "What is the Kano Model?" (10 mins)
  - Quick overview with visual examples

- **Udemy**: "Product Management: Prioritization Frameworks"
  - Module on Kano Model with real case studies
  - Includes survey design best practices

- **Coursera - University of Virginia**: "Digital Product Management"
  - Week 4 covers Kano Model in depth
  - Academic perspective with research backing

### Research Papers
- **Original Paper**: "Attractive Quality and Must-Be Quality" (Kano et al., 1984)
  - URL: https://www.researchgate.net/publication/232937942_Attractive_quality_and_must-be_quality
  - The foundational research introducing the model

- **"The Evolution of Customer Needs"** (Kano, 2001)
  - How features transition from Excitement to Performance to Basic over time
  - Explains why you need to re-run Kano surveys periodically

### Community Resources
- **Product Management Slack Communities**
  - #prioritization channel often discusses Kano
  - Mind the Product, Product School communities

- **Reddit**: r/ProductManagement
  - Search "Kano Model" for real PM experiences
  - Templates and tips shared by community

---

## Quick Reference Card

### When to Use Kano
✅ Cross-functional disagreements on priority
✅ Need to balance must-haves vs nice-to-haves
✅ Limited resources, must cut features
✅ Validating customer satisfaction impact

### When NOT to Use Kano
❌ Technical debt prioritization (use engineering-led frameworks)
❌ Time-sensitive decisions (Kano takes 1-2 weeks)
❌ Very small user base (<10 users)
❌ Features are obvious basics (e.g., "app must load")

### Kano in 60 Seconds
1. List features
2. Survey users: "How would you feel if we HAD this?" + "How would you feel if we DIDN'T have this?"
3. Classify: Basic/Performance/Excitement/Indifferent/Reverse
4. Prioritize: Build Basics first → Performance → Excitement
5. Win: Data-driven decisions, no more opinion battles

---

**Last Updated**: November 20, 2025
**Framework Version**: 1.0
**Root Phase**: Phase 2: Prioritize & Decide
**Root Command**: `/phase2:kano`

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
