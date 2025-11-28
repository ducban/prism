---
# Core Metadata
title: "Data Visualization & Chart Selection Framework"
title_vi: "Khung Trực Quan Hóa Dữ Liệu & Chọn Biểu Đồ"
framework_type: "Analytics"
category: ["Analytics", "Data Visualization", "Business Intelligence", "Metrics"]

# Origin & Authority
author: "Edward Tufte, Stephen Few, Cole Nussbaumer Knaflic"
organization: "Industry best practices"
year_developed: "1980s-2015"
original_source: "The Visual Display of Quantitative Information (Tufte, 1983), Storytelling with Data (Knaflic, 2015)"

# Root Integration
root_phase: ["Phase 5: Track Progress", "Phase 6: Launch & Measure"]
root_commands: ["/scenario:chart", "/scenario:dashboard", "/scenario:metrics"]
when_to_use: "When you need to visualize data, create dashboards, present metrics, or communicate insights to stakeholders"

# Difficulty & Time
complexity: "Medium"
estimated_time: "30 min - 2 hours (depending on chart complexity)"
skill_level: "Beginner-Intermediate"

# Classification
tags: ["data-visualization", "charts", "dashboards", "analytics", "metrics", "communication"]
related_frameworks: ["Product Metrics", "Cohort Analysis", "AARRR Pirate Metrics", "North Star Framework", "Retention & Churn Analysis"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-23"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Book"
    title: "The Visual Display of Quantitative Information"
    author: "Edward Tufte"
    year: "1983"
  - type: "Book"
    title: "Storytelling with Data"
    author: "Cole Nussbaumer Knaflic"
    year: "2015"
  - type: "Book"
    title: "Information Dashboard Design"
    author: "Stephen Few"
    year: "2006"
  - type: "Tool"
    title: "Chart Chooser by Juice Analytics"
    url: "https://www.juiceanalytics.com/chartchooser"
---

# Data Visualization & Chart Selection Framework / Khung Trực Quan Hóa Dữ Liệu

## Overview / Tổng Quan

**English:**
Choosing the wrong chart type can hide insights, confuse stakeholders, or lead to wrong decisions. This framework helps Product Managers select the right visualization for their data story.

**The Problem with Charts:**
- 📊 **Wrong chart type** → Insights get lost
- 📉 **Too complex** → Stakeholders confused
- 📈 **Misleading scales** → Wrong conclusions
- 🎨 **Poor design** → Data ignored

**The Goal:**
Answer 3 questions before creating any chart:
1. **What am I trying to show?** (Comparison, trend, distribution, relationship, composition?)
2. **Who is my audience?** (Executives, engineers, customers, investors?)
3. **What action should they take?** (Approve budget, fix bug, change strategy?)

**Vietnamese:**
Chọn sai loại biểu đồ có thể che giấu insights, làm stakeholder bối rối, hoặc dẫn đến quyết định sai.

**Mục Tiêu:**
Trả lời 3 câu hỏi trước khi tạo bất kỳ biểu đồ nào:
1. Tôi muốn thể hiện điều gì? (So sánh, xu hướng, phân phối, mối quan hệ, cấu trúc?)
2. Ai là đối tượng? (Executives, kỹ sư, khách hàng, nhà đầu tư?)
3. Họ nên hành động gì? (Phê duyệt ngân sách, sửa lỗi, đổi chiến lược?)

---

## The Chart Selection Matrix / Ma Trận Chọn Biểu Đồ

### 1. COMPARISON Charts (So Sánh)
**Goal**: Compare values across categories

#### Bar Chart (Biểu Đồ Cột)
**When to Use**:
- ✅ Comparing values across categories (e.g., revenue by product)
- ✅ Showing rankings (e.g., top 10 features by usage)
- ✅ Comparing time periods (e.g., Q1 vs Q2 vs Q3)
- ✅ Negative values present

**How to Read**:
- Longer bar = higher value
- Easy to compare exact values
- Horizontal bars work better for long category names

**How to Create**:
```
Tools: Excel, Google Sheets, Tableau, Looker, Amplitude
Steps:
1. Organize data: Category | Value
2. Sort by value (descending usually)
3. Use horizontal bars if >5 categories
4. Label bars directly (avoid legends when possible)
5. Start Y-axis at zero (never truncate!)
```

**Example - PM Use Case**:
```
Feature Usage (Monthly Active Users)
Search:          ███████████████████ 45,000
Dashboard:       ████████████████ 38,000
Reports:         ████████████ 28,000
Integrations:    █████████ 21,000
API Access:      ██████ 15,000
```

**Common Mistakes**:
- ❌ Starting Y-axis at non-zero (exaggerates differences)
- ❌ Using 3D bars (harder to read)
- ❌ Too many categories (>10 becomes cluttered)

---

#### Column Chart (Biểu Đồ Cột Dọc)
**When to Use**:
- ✅ Time series comparison (e.g., monthly revenue)
- ✅ Few categories (<7)
- ✅ Showing trends over time

**Different from Bar Chart**: Vertical orientation, better for time series

**Example - PM Use Case**:
Monthly Sign-ups comparison across 6 months

---

#### Grouped/Stacked Bar Chart (Biểu Đồ Cột Nhóm/Xếp Chồng)
**When to Use**:
- ✅ Comparing multiple metrics per category
- ✅ Showing parts of a whole (stacked)
- ✅ Comparing subgroups (grouped)

**How to Choose**:
- **Grouped**: When comparing each subgroup's absolute values
- **Stacked**: When showing total + composition

**Example - PM Use Case**:
```
Grouped: Compare Free vs Paid users per feature
Stacked: Show total users + breakdown by plan type
```

---

### 2. TREND Charts (Xu Hướng)

#### Line Chart (Biểu Đồ Đường)
**When to Use**:
- ✅ Showing trends over time
- ✅ Continuous data (time series)
- ✅ Multiple metrics comparison (up to 5 lines)
- ✅ Highlighting patterns (seasonality, growth, decline)

**How to Read**:
- Slope = rate of change (steeper = faster)
- Up = growth, Down = decline, Flat = stable
- Crossing lines = inflection points (important!)

**How to Create**:
```
Tools: Excel, Google Sheets, Mixpanel, Amplitude, Looker
Best Practices:
1. Use clear line colors (max 5 lines)
2. Label lines directly (not just legend)
3. Highlight the most important line
4. Add annotations for key events
5. Use consistent time intervals
```

**Example - PM Use Case (Retention Curve)**:
```
Day 1:   100% ●
Day 7:    45% ●─────●
Day 30:   28% ●─────────●
Day 60:   22% ●──────────────●
Day 90:   20% ●───────────────────● (flattening = good!)
```

**Real Example - Slack Retention:**
```
Slack's retention curve:
Week 1:  100%
Week 2:   93%  (strong!)
Week 4:   88%
Week 8:   85%  (curve flattens = PMF signal)
```

**Common Mistakes**:
- ❌ Too many lines (>5 = spaghetti chart)
- ❌ Inconsistent time intervals (weekly + monthly mixed)
- ❌ Not starting at zero when comparing magnitudes

---

#### Area Chart (Biểu Đồ Vùng)
**When to Use**:
- ✅ Showing cumulative totals over time
- ✅ Emphasizing magnitude of change
- ✅ Stacked area: showing composition changes over time

**Example - PM Use Case**:
Cumulative feature adoption over time

---

### 3. DISTRIBUTION Charts (Phân Phối)

#### Histogram (Biểu Đồ Tần Suất)
**When to Use**:
- ✅ Showing distribution of continuous data
- ✅ Understanding data spread (normal, skewed, bimodal)
- ✅ Finding outliers

**How to Read**:
- X-axis = ranges (bins)
- Y-axis = frequency (count or %)
- Shape tells the story: normal bell curve, right-skewed, left-skewed

**How to Create**:
```
Tools: Excel (Data Analysis ToolPak), Python (matplotlib), Tableau
Steps:
1. Define bins (ranges)
2. Count occurrences in each bin
3. Plot as bars (no gaps between bars!)
4. Analyze shape and outliers
```

**Example - PM Use Case**:
```
Session Duration Distribution
0-1 min:    ████████████████████ 2,400 users (poor engagement)
1-5 min:    ██████████████████████████████ 3,800 users
5-10 min:   ████████████████ 2,100 users
10-30 min:  ██████████ 1,200 users
30+ min:    ████ 500 users (power users!)

Insight: Bimodal distribution = 2 user segments (bouncing vs engaged)
```

**Common Mistakes**:
- ❌ Too few bins (lose detail)
- ❌ Too many bins (too noisy)
- ❌ Gaps between bars (makes it look like bar chart)

---

#### Box Plot (Biểu Đồ Hộp)
**When to Use**:
- ✅ Showing median, quartiles, and outliers
- ✅ Comparing distributions across groups
- ✅ Identifying outliers

**How to Read**:
```
    |        ┌─────────────┐
    |    ────┤      │      ├────  ← Whiskers (min/max or 1.5×IQR)
    |        │  ●   │   ●  │
    |        └──────┼──────┘
    |          Q1  Median  Q3
```

**Example - PM Use Case**:
Compare response times across different API endpoints

---

### 4. RELATIONSHIP Charts (Mối Quan Hệ)

#### Scatter Plot (Biểu Đồ Phân Tán)
**When to Use**:
- ✅ Showing correlation between two variables
- ✅ Finding patterns or clusters
- ✅ Identifying outliers

**How to Read**:
- Positive correlation: points go up-right ↗
- Negative correlation: points go down-right ↘
- No correlation: random scatter

**How to Create**:
```
Tools: Excel, Google Sheets, Tableau, Python (matplotlib, seaborn)
Best Practices:
1. Each point = one data point
2. Add trend line if correlation exists
3. Label interesting outliers
4. Use color/size for 3rd dimension
```

**Example - PM Use Case (RICE Prioritization)**:
```
           │
 High   10 │        ● Feature A (High Impact, Low Effort = DO THIS!)
           │
 Impact  5 │  ● Feature C        ● Feature B
           │
 Low     0 │    ● Feature D
           └─────────────────────
             Low → High
                Effort
```

**Real Example - Intercom Feature Prioritization:**
```
Scatter plot of all feature requests:
X-axis: Effort (person-weeks)
Y-axis: Expected Impact (RICE score)
Color: Customer segment (Enterprise vs SMB)
Result: Identified 3 "quick wins" in top-left quadrant
```

**Common Mistakes**:
- ❌ Too many points (>100 becomes blob)
- ❌ Not labeling outliers
- ❌ Assuming correlation = causation

---

#### Bubble Chart (Biểu Đồ Bong Bóng)
**When to Use**:
- ✅ Showing 3 dimensions (X, Y, bubble size)
- ✅ Comparing items on multiple metrics

**Example - PM Use Case**:
- X-axis: Customer count
- Y-axis: Revenue per customer
- Bubble size: Churn rate
- Color: Market segment

---

### 5. COMPOSITION Charts (Cấu Trúc/Thành Phần)

#### Pie Chart (Biểu Đồ Tròn)
**When to Use**:
- ✅ Showing parts of a whole (must add to 100%)
- ✅ Maximum 5-7 slices
- ✅ One slice is dominant (>50%)

**When NOT to Use**:
- ❌ Comparing similar-sized slices (use bar chart instead)
- ❌ Showing trends over time (use line chart)
- ❌ More than 7 categories (too cluttered)

**How to Read**:
- Bigger slice = larger proportion
- All slices = 100%
- Start at 12 o'clock, go clockwise

**How to Create**:
```
Tools: Excel, Google Sheets, Tableau
Best Practices:
1. Order slices by size (largest first)
2. Limit to 5-7 slices max
3. Label with percentages AND values
4. Use contrasting colors
5. Pull out important slice for emphasis
```

**Example - PM Use Case**:
```
User Acquisition Channels (November 2025)
────────────────────────────────
Organic Search:    42% (4,200 users)
Direct:            28% (2,800 users)
Paid Ads:          18% (1,800 users)
Referral:          12% (1,200 users)

Total: 10,000 new users
```

**Real Example - Dropbox Traffic Sources (2010):**
```
Referral Program:  60% (viral growth!)
Direct:            25%
Paid:              15%

Insight: Referral program is the growth engine → invest more
```

**Common Mistakes**:
- ❌ Using for trends (pie charts are snapshots, not time series)
- ❌ Too many slices (>7)
- ❌ 3D pie charts (distort proportions)
- ❌ Not ordering by size

---

#### Donut Chart (Biểu Đồ Vòng)
**When to Use**:
- Same as pie chart, but with central space for key metric
- ✅ Better for multiple donut comparison

**Example - PM Use Case**:
Show user distribution by plan type, with total ARR in center

---

#### Stacked Bar/Column Chart (Biểu Đồ Cột Xếp Chồng)
**When to Use**:
- ✅ Showing composition changes over time
- ✅ Comparing totals AND parts
- ✅ 100% stacked: for proportion comparison

**Example - PM Use Case**:
```
Monthly Revenue by Plan Type
Jan: [Free: 20% | Pro: 45% | Enterprise: 35%] = $100K
Feb: [Free: 18% | Pro: 42% | Enterprise: 40%] = $120K (↑ Enterprise!)
Mar: [Free: 15% | Pro: 40% | Enterprise: 45%] = $140K
```

---

### 6. PM-SPECIFIC Charts (Biểu Đồ Chuyên Dụng PM)

#### Funnel Chart (Biểu Đồ Phễu)
**When to Use**:
- ✅ Showing conversion through stages
- ✅ Identifying drop-off points
- ✅ A/B testing results

**How to Read**:
- Width = number/percentage at each stage
- Narrowing = expected (some drop-off)
- Sudden drop = problem to investigate!

**How to Create**:
```
Tools: Mixpanel, Amplitude, Google Analytics, Excel
Key Metrics:
- Conversion rate per stage
- Overall conversion rate
- Drop-off rate per stage
```

**Example - PM Use Case (SaaS Onboarding)**:
```
Visited Landing Page:    10,000 (100%)
      ↓ 40% conversion
Signed Up:                4,000 (40%)
      ↓ 70% conversion
Completed Onboarding:     2,800 (28%)
      ↓ 50% conversion  ← BIG DROP! Investigate!
Activated (used key feature): 1,400 (14%)
      ↓ 60% conversion
Converted to Paid:          840 (8.4%)
```

**Real Example - LinkedIn Sign-up Funnel:**
```
Stage 1: Visit homepage         100%
Stage 2: Click "Join Now"        45%  (55% drop)
Stage 3: Enter email             38%  (7% drop - low friction form ✓)
Stage 4: Verify email            32%  (6% drop)
Stage 5: Complete profile        28%  (4% drop)
Stage 6: Add 5+ connections      22%  (6% drop)

Biggest opportunity: Stage 1→2 (improve homepage CTA)
```

**Common Mistakes**:
- ❌ Too many stages (>7)
- ❌ Not labeling conversion rates
- ❌ Ignoring time windows (1-day vs 7-day funnel)

---

#### Cohort Retention Chart (Biểu Đồ Retention Cohort)
**When to Use**:
- ✅ Measuring product stickiness
- ✅ Comparing retention across cohorts
- ✅ Validating product-market fit

**How to Read**:
```
Cohort: Users who signed up in same time period
Columns: Retention % at Day/Week/Month intervals
Color: Darker = higher retention
```

**How to Create**:
```
Tools: Mixpanel, Amplitude, SQL + Tableau
Structure:
         Day 0  Day 1  Day 7  Day 30  Day 90
Week 1:  100%   45%    28%    20%     18%
Week 2:  100%   48%    32%    24%     21%  ← Improving!
Week 3:  100%   52%    38%    28%     25%  ← Even better!
```

**Example - PM Use Case**:
```
Monthly Cohort Retention (Mobile App)

Cohort     M0   M1   M2   M3   M4   M5   M6
────────────────────────────────────────────
Jan 2025: 100%  45%  32%  25%  22%  20%  20% ← Flattening at 20%
Feb 2025: 100%  48%  35%  28%  25%  23%  22% ← Improving!
Mar 2025: 100%  52%  40%  33%  30%  28%  --

Insight: New onboarding flow (launched Feb) improved retention by 5-10%
```

**Real Example - Facebook (2010):**
```
Cohort retention by "Days to 7 Friends" milestone:
- Users who added 7 friends in 10 days: 90% retained at Day 30
- Users who added 7 friends in 30 days: 60% retained at Day 30
- Users who never added 7 friends: 20% retained at Day 30

Insight: "7 friends in 10 days" became activation metric
```

**Common Mistakes**:
- ❌ Not defining cohort clearly (signup date vs first action)
- ❌ Mixing cohort sizes (1,000 users vs 10 users)
- ❌ Ignoring seasonality

---

#### Sankey Diagram (Biểu Đồ Dòng Chảy)
**When to Use**:
- ✅ Showing flow between states
- ✅ User journey mapping
- ✅ Attribution analysis

**How to Read**:
- Width of flow = magnitude
- Flows can split or merge

**Example - PM Use Case**:
```
Traffic Source → Landing Page → Conversion

Organic (60%) ──────────┐
                         ├──→ Homepage (45%) ───→ Signup (12%)
Paid Ads (20%) ─────────┤
                         └──→ Product Page (35%) → Signup (8%)
Referral (20%) ──────────────→ Dashboard (20%) ──→ Signup (15%)

Insight: Referral traffic converts best (15% vs 12% vs 8%)
```

---

#### Heatmap (Biểu Đồ Nhiệt)
**When to Use**:
- ✅ Showing patterns across two dimensions
- ✅ Correlation matrices
- ✅ Usage patterns (hour × day)

**Example - PM Use Case**:
```
Feature Usage Heatmap (Hour × Day of Week)

         Mon   Tue   Wed   Thu   Fri   Sat   Sun
6-9am:   🟦    🟦    🟦    🟦    🟦    ⬜    ⬜
9-12pm:  🟩    🟩    🟩    🟩    🟦    🟦    ⬜
12-3pm:  🟨    🟨    🟨    🟨    🟨    🟦    ⬜
3-6pm:   🟧    🟧    🟧    🟧    🟦    🟦    ⬜
6-9pm:   🟦    🟦    🟦    🟦    🟦    🟦    🟦

Legend: ⬜ Low → 🟦 → 🟩 → 🟨 → 🟧 High

Insight: Peak usage = weekday afternoons (plan maintenance for weekends)
```

---

#### Waterfall Chart (Biểu Đồ Thác Nước)
**When to Use**:
- ✅ Showing cumulative effect of sequential changes
- ✅ Revenue/profit breakdown
- ✅ Funnel analysis with values

**How to Read**:
- Starting value (anchor)
- Incremental changes (floating bars)
- Final value (anchor)

**Example - PM Use Case**:
```
Monthly Recurring Revenue (MRR) Changes

Start MRR:        $100,000 ███████████████████
+ New MRR:         +$25,000 ↑↑↑↑↑
+ Expansion MRR:   +$10,000 ↑↑
- Churned MRR:     -$15,000 ↓↓↓
- Contraction MRR:  -$5,000 ↓
End MRR:          $115,000 ████████████████████████

Net Change: +$15,000 (+15%)
```

---

#### Gantt Chart (Biểu Đồ Gantt)
**When to Use**:
- ✅ Project timeline visualization
- ✅ Roadmap communication
- ✅ Dependency tracking

**Example - PM Use Case**:
```
Q4 2025 Product Roadmap

Feature A:  ████████░░░░░░░░ (Oct 1 - Nov 15)
Feature B:          ████████ (Nov 1 - Dec 15)
Feature C:              ██████ (Nov 15 - Dec 31)
Launch:                        ● (Dec 31)
         Oct        Nov        Dec
```

---

### 7. BUSINESS ANALYTICS Charts

#### Revenue/Profit Chart (Line + Bar Combo)
**When to Use**:
- ✅ Showing revenue trends + profit margins
- ✅ Comparing actuals vs targets

**Example**:
```
Bars: Monthly revenue
Line: Profit margin %
```

---

#### Burn Rate Chart (Runway Visualization)
**When to Use**:
- ✅ Showing cash position over time
- ✅ Forecasting runway

**Example - PM Use Case**:
```
Cash Balance:
$1,000K ●
         ╲
$800K     ●
           ╲
$600K       ●  ← Current ($600K)
             ╲
$400K         ●
               ╲ Projected
$200K           ●
                 ╲
$0K               ● ← Runway ends: June 2026 (6 months)

Burn Rate: -$100K/month
Action: Need funding or profitability in 6 months
```

---

#### Customer Segmentation Chart (2×2 Matrix)
**When to Use**:
- ✅ Showing customer segments
- ✅ Portfolio analysis

**Example - PM Use Case**:
```
         High Value
              │
   Champions  │  High Potential
       ●  ●   │    ●  ●
       ● ●●   │   ●
──────────────┼───────────────
       ●      │  ●  ●  ●
        ●     │ ●  ●
   At Risk    │  Low Priority
              │
         Low Value
```

---

## Chart Creation Tools / Công Cụ Tạo Biểu Đồ

### For Product Managers

**Quick & Easy (No code)**:
- **Google Sheets / Excel**: Basic charts, accessible to everyone
- **Looker Studio (Google Data Studio)**: Free dashboards
- **Notion**: Embedded charts from databases

**PM Analytics Tools**:
- **Mixpanel**: Funnels, retention, cohorts (built-in)
- **Amplitude**: User behavior analytics
- **Heap**: Auto-capture event tracking
- **PostHog**: Open-source product analytics

**Business Intelligence**:
- **Tableau**: Professional dashboards (steep learning curve)
- **Looker**: SQL-based BI tool
- **Metabase**: Open-source, easy BI
- **Mode**: SQL + Python + visualization

**For Developers**:
- **Python**: matplotlib, seaborn, plotly
- **JavaScript**: D3.js, Chart.js, Recharts
- **R**: ggplot2

---

## How to Choose the Right Chart / Cách Chọn Biểu Đồ Đúng

### Decision Tree

```
What do you want to show?

├─ COMPARISON (compare values across categories)
│  ├─ Few categories (<7): Column/Bar Chart
│  ├─ Many categories (>7): Horizontal Bar Chart (sorted)
│  └─ Multiple metrics per category: Grouped/Stacked Bar
│
├─ TREND (changes over time)
│  ├─ Single metric: Line Chart
│  ├─ Multiple metrics (2-5): Multi-line Chart
│  └─ Cumulative total: Area Chart
│
├─ DISTRIBUTION (spread of values)
│  ├─ Frequency distribution: Histogram
│  ├─ Quartiles + outliers: Box Plot
│  └─ Show individual points: Scatter Plot
│
├─ RELATIONSHIP (correlation between variables)
│  ├─ Two variables: Scatter Plot
│  └─ Three variables: Bubble Chart
│
├─ COMPOSITION (parts of a whole)
│  ├─ Snapshot (one time period): Pie/Donut Chart
│  ├─ Over time: Stacked Bar/Area Chart
│  └─ Proportion (100%): 100% Stacked Bar
│
└─ PM-SPECIFIC
   ├─ Conversion: Funnel Chart
   ├─ Retention: Cohort Chart / Line Chart
   ├─ User flow: Sankey Diagram
   ├─ Usage patterns: Heatmap
   ├─ Sequential changes: Waterfall Chart
   └─ Timeline: Gantt Chart
```

---

## Chart Best Practices / Nguyên Tắc Thiết Kế

### 1. **Clarity Over Aesthetics**
- Simple > Complex
- Remove chart junk (3D effects, unnecessary gridlines, decorations)
- High data-to-ink ratio

### 2. **Label Everything**
- Chart title: What + So What
- Axis labels with units
- Direct labels (avoid legends when possible)
- Source and date

### 3. **Use Color Purposefully**
- Max 5-7 colors
- Color-blind friendly palettes
- Use color to highlight, not decorate
- Consistent colors across dashboards

### 4. **Scale Matters**
- Always start bar/column charts at zero
- Use consistent scales for comparison
- Show breaks if axis is truncated
- Log scale for exponential data

### 5. **Tell a Story**
- Annotate key events (product launch, bug fix, etc.)
- Add trend lines for clarity
- Highlight important data points
- Include context (benchmarks, targets)

### 6. **Make it Actionable**
- Include recommendations
- Show thresholds (green/yellow/red zones)
- Compare to goals/benchmarks
- Clear next steps

---

## Common Chart Mistakes & Fixes / Lỗi Phổ Biến

| Mistake | Why It's Bad | Fix |
|---------|-------------|-----|
| **Truncated Y-axis** (doesn't start at 0) | Exaggerates differences | Always start at zero for bar charts |
| **Too many lines** (>5) | Spaghetti chart, unreadable | Show top 3-5, group others as "Other" |
| **Pie chart for trends** | Pies are snapshots, not time series | Use line/area chart |
| **3D charts** | Distorts values, hard to read | Use 2D charts only |
| **No labels** | Audience has to guess | Label axes, data points, and add title |
| **Rainbow colors** | Hard to distinguish | Max 5-7 colors, use color-blind palette |
| **Dual Y-axes** | Can be misleading | Use separate charts or same scale |
| **Unlabeled legend** | "What's the blue line?" | Direct labels or clear legend |
| **No context** | "Is this good or bad?" | Add benchmarks, targets, or comparisons |

---

## PM Chart Library - Quick Reference / Thư Viện Nhanh

### Most Common PM Charts (80% of use cases)

1. **Line Chart** - Retention curve, DAU/MAU trends, MRR growth
2. **Bar Chart** - Feature usage, revenue by segment, NPS by cohort
3. **Funnel Chart** - Conversion funnels, onboarding drop-off
4. **Cohort Chart** - Retention by cohort, feature adoption
5. **Scatter Plot** - Prioritization (RICE), A/B test results
6. **Stacked Bar** - Revenue mix, user composition over time

### When Stakeholders Ask for Specific Charts

**"Show me our growth"**
→ Line chart (MRR, users, revenue over time)

**"Which feature is most used?"**
→ Horizontal bar chart (sorted by usage)

**"How's our retention?"**
→ Cohort retention chart or retention curve (line chart)

**"Where do users drop off?"**
→ Funnel chart with conversion rates

**"How do segments compare?"**
→ Grouped bar chart or small multiples

**"What should we prioritize?"**
→ Scatter plot (effort vs impact) or RICE table

**"How's our revenue mix changing?"**
→ Stacked area chart or 100% stacked bar

---

## Real PM Examples / Ví Dụ Thực Tế

### Example 1: Spotify - Retention Curve
**Chart Type**: Line Chart
**Insight**: Retention curve flattened at 40% after Day 30 → PMF confirmed
**Action**: Focus on activation (getting users to Day 30)

### Example 2: Airbnb - Funnel Analysis
**Chart Type**: Funnel Chart
**Insight**: 60% drop-off between "Search" → "View Listing"
**Action**: Improved search algorithm → increased conversion by 15%

### Example 3: Netflix - Cohort Analysis
**Chart Type**: Cohort Retention Heatmap
**Insight**: Cohorts who watched 3+ titles in Week 1 had 90% retention
**Action**: Onboarding flow optimized to get users to 3 titles faster

### Example 4: Slack - Feature Adoption
**Chart Type**: Stacked Area Chart
**Insight**: Integrations adoption grew from 10% → 45% of teams
**Action**: Integrations became a core value prop

### Example 5: LinkedIn - A/B Test Results
**Chart Type**: Bar Chart with Error Bars
**Insight**: New feed algorithm increased time on site by 12% (p < 0.01)
**Action**: Rolled out to 100% of users

---

## Dashboard Design Principles / Nguyên Tắc Dashboard

### Good Dashboard Structure

**Top Section**: Key Metrics (North Star + 3-5 KPIs)
- Large numbers with trend arrows
- Color coding (green/yellow/red)

**Middle Section**: Trends & Comparisons
- Line charts for time series
- Bar charts for comparisons

**Bottom Section**: Details & Breakdowns
- Tables for deep dive
- Filters for segmentation

### Dashboard Anti-Patterns

❌ **Too many metrics** (analysis paralysis)
✅ Focus on 5-7 key metrics

❌ **No hierarchy** (everything looks equally important)
✅ Visual hierarchy (size, color, position)

❌ **Static snapshots** (outdated data)
✅ Real-time or auto-refresh

❌ **No context** (is 10% churn good or bad?)
✅ Add benchmarks and targets

---

## Practice Exercise / Bài Tập Thực Hành

**Scenario**: You're a PM at a SaaS company. CEO asks:
*"How's our product performing? I need to present to the board next week."*

**Your Task**: Choose the right charts and explain why.

**Data Available**:
- Monthly Recurring Revenue (12 months)
- User growth (12 months)
- Retention by cohort (6 cohorts)
- Top 10 features by usage
- Customer segments (Enterprise, SMB, Self-serve)
- Churn reasons (5 categories)

**Solution**:
1. **MRR Trend**: Line chart (show growth trajectory)
2. **User Growth**: Line chart (overlay with MRR to show unit economics)
3. **Retention**: Cohort retention chart (show stickiness improving)
4. **Feature Usage**: Horizontal bar chart (sorted, top 10)
5. **Revenue Mix**: Stacked bar chart (composition change over time)
6. **Churn Reasons**: Horizontal bar chart (sorted by frequency)

**Pro Tip**: Create a 1-page executive dashboard with these 6 charts

---

## Resources / Tài Nguyên

### Books
- **"Storytelling with Data"** by Cole Nussbaumer Knaflic (2015) - Best book for PMs
- **"The Visual Display of Quantitative Information"** by Edward Tufte (1983) - Classic
- **"Information Dashboard Design"** by Stephen Few (2006) - Dashboard best practices

### Tools
- **Chart Chooser** (Juice Analytics): Interactive chart selection tool
- **Color Brewer**: Color-blind friendly palettes
- **Figma/Sketch**: Mockup dashboards before building

### Online Courses
- **Google Analytics Academy**: Free courses on data visualization
- **Tableau Public**: Free tool + gallery of examples

---

## Summary / Tóm Tắt

**Before creating any chart, ask**:
1. **What's the question?** (What am I trying to answer?)
2. **What's the data type?** (Categorical, time series, distribution, relationship?)
3. **Who's the audience?** (Technical, executive, customer?)
4. **What's the action?** (What should they do with this information?)

**The Chart Selection Matrix**:
- **Comparison** → Bar Chart
- **Trend** → Line Chart
- **Distribution** → Histogram / Box Plot
- **Relationship** → Scatter Plot
- **Composition** → Pie / Stacked Bar
- **PM-Specific** → Funnel / Cohort / Sankey

**Remember**:
- Simple > Complex
- Clarity > Beauty
- Action > Information

**The best chart is the one that makes the decision obvious.**

---

## Quick Decision Guide / Hướng Dẫn Nhanh

| PM Question | Chart Type | Example |
|------------|-----------|---------|
| How's our growth? | Line chart | MRR over time |
| Which feature wins? | Bar chart | Feature usage (sorted) |
| Where do users drop? | Funnel chart | Signup → Activation |
| Is retention improving? | Cohort chart | Monthly cohorts |
| What should we build? | Scatter plot | Effort vs Impact |
| How's revenue mix changing? | Stacked area | Revenue by plan type |
| Where does traffic come from? | Pie chart | Channels (if <7) |
| When should we launch? | Gantt chart | Roadmap timeline |
| What's the pattern? | Heatmap | Usage by hour × day |
| How did we get here? | Waterfall | MRR bridge |

---

**Next Steps**:
1. ✅ Bookmark this framework
2. ✅ Use the decision tree for your next chart
3. ✅ Review your current dashboards (fix common mistakes)
4. ✅ Practice with real data
5. ✅ Share charts with stakeholders and get feedback

**Remember**: The goal isn't to create beautiful charts. The goal is to make decisions obvious.

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
