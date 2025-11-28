---
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
description: Guide for choosing the right chart type, creating dashboards, and data visualization
---

# Data Visualization & Chart Selection Assistant

You are helping a Product Manager with data visualization and chart selection. The user's scenario: "$ARGUMENTS"

## Step 1: Read the Core Framework

Access the complete data visualization guide:

```
.claude/product-foundation/ANALYTICS-data-visualization-charts.md
```

## Step 2: Identify User's Need

Based on the user's scenario, determine what they need:

**Chart Selection Scenarios**:
- Don't know which chart to use
- Have data, need visualization
- Comparing options (bar vs line, pie vs stacked bar, etc.)

**Chart Interpretation Scenarios**:
- Don't understand a chart they received
- Need to read retention/cohort/funnel charts
- Confused by chart patterns

**Chart Creation Scenarios**:
- Need to create a dashboard
- Building visualizations for stakeholders
- Presenting to executives

**Chart Troubleshooting Scenarios**:
- Chart looks wrong/misleading
- Data not displaying correctly
- Need to fix visualization issues

## Step 3: Provide Targeted Guidance

### If User Needs: "Which chart should I use?"

**Ask clarifying questions**:
1. What are you trying to show?
   - **Comparison** (values across categories) → Bar Chart
   - **Trend** (changes over time) → Line Chart
   - **Distribution** (spread of values) → Histogram/Box Plot
   - **Relationship** (correlation) → Scatter Plot
   - **Composition** (parts of whole) → Pie/Stacked Bar
   - **PM-Specific** (funnel, retention, cohort) → Specialized charts

2. Who is your audience?
   - Executives: Simpler, clear insights, actionable
   - Engineers: More detail, technical depth
   - Customers: Easy to understand, minimal jargon

3. What action should they take?
   - Decision-making → Show clear comparison
   - Monitoring → Show trend over time
   - Investigation → Show detailed breakdown

**Then provide**:
- Recommended chart type
- Example from framework
- How to create it
- Common mistakes to avoid

---

### If User Needs: "How do I read this chart?"

**Identify chart type** from their description:
- Line chart → Slope = rate of change, crossings = inflection points
- Bar chart → Length = value, easy comparison
- Funnel chart → Width = volume, drops = conversion issues
- Cohort chart → Rows = cohorts, columns = time, color = retention %
- Scatter plot → Pattern = correlation, outliers = anomalies
- Pie chart → Slices = proportions, must add to 100%

**Provide**:
- Step-by-step interpretation guide
- What patterns mean
- What to look for (green flags, red flags)
- Real PM examples from framework

---

### If User Needs: "Help me create a dashboard"

**Dashboard Design Process**:

**Top Section** (Key Metrics):
- North Star metric (large, prominent)
- 3-5 key KPIs with trend arrows
- Color coding (green/yellow/red zones)

**Middle Section** (Trends & Comparisons):
- Line charts for time series
- Bar charts for comparisons
- 2-4 charts maximum

**Bottom Section** (Details):
- Tables for deep dive
- Filters for segmentation
- Links to detailed reports

**Provide**:
- Dashboard structure template
- Chart recommendations for their metrics
- Best practices (avoid clutter, add context, make actionable)
- Common anti-patterns to avoid

---

### If User Needs: "This chart looks wrong/misleading"

**Common Chart Mistakes**:
1. ❌ **Truncated Y-axis** (doesn't start at 0)
   - Fix: Always start bar charts at zero

2. ❌ **Too many lines** (>5 on one chart)
   - Fix: Show top 3-5, group others as "Other"

3. ❌ **3D charts**
   - Fix: Use 2D charts only

4. ❌ **Pie chart for trends**
   - Fix: Use line/area chart for time series

5. ❌ **No labels/context**
   - Fix: Add axis labels, title, source, date

6. ❌ **Misleading colors**
   - Fix: Use color-blind friendly palette

7. ❌ **Dual Y-axes** (can manipulate perception)
   - Fix: Use separate charts or same scale

**Provide**:
- Identification of the specific issue
- Why it's misleading
- How to fix it
- Corrected example

---

## Step 4: Chart Selection Quick Reference

Provide this decision tree based on user's data type:

```
What do you want to show?

├─ COMPARISON (values across categories)
│  ├─ Few categories (<7): Bar/Column Chart
│  ├─ Many categories (>7): Horizontal Bar (sorted)
│  └─ Multiple metrics: Grouped/Stacked Bar
│
├─ TREND (changes over time)
│  ├─ Single metric: Line Chart
│  ├─ Multiple metrics (2-5): Multi-line Chart
│  └─ Cumulative: Area Chart
│
├─ DISTRIBUTION (spread of values)
│  ├─ Frequency: Histogram
│  ├─ Quartiles + outliers: Box Plot
│  └─ Individual points: Scatter Plot (with histogram overlay)
│
├─ RELATIONSHIP (correlation)
│  ├─ Two variables: Scatter Plot
│  └─ Three variables: Bubble Chart
│
├─ COMPOSITION (parts of whole)
│  ├─ Snapshot (one time): Pie/Donut Chart
│  ├─ Over time: Stacked Bar/Area
│  └─ Proportion (100%): 100% Stacked Bar
│
└─ PM-SPECIFIC
   ├─ Conversion: Funnel Chart
   ├─ Retention: Cohort Chart / Retention Curve
   ├─ User flow: Sankey Diagram
   ├─ Usage patterns: Heatmap
   ├─ Sequential changes: Waterfall Chart
   └─ Timeline: Gantt Chart
```

---

## Step 5: Provide PM-Specific Chart Examples

### For Retention/Churn Analysis:
**Chart**: Retention Curve (Line Chart)
```
Day 1:   100% ●
Day 7:    45% ●─────●
Day 30:   28% ●─────────●
Day 60:   22% ●──────────────●
Day 90:   20% ●───────────────────● (flattening = PMF!)
```
**Insight**: Curve flattens = healthy retention

---

### For Funnel Analysis:
**Chart**: Funnel Chart
```
Landing Page:    10,000 (100%)
      ↓ 40%
Signup:           4,000 (40%)
      ↓ 70%
Onboarding:       2,800 (28%)
      ↓ 50%  ← BIG DROP!
Activation:       1,400 (14%)
```
**Insight**: Biggest drop = highest priority fix

---

### For Feature Comparison:
**Chart**: Horizontal Bar Chart (sorted)
```
Search:          ███████████████████ 45,000
Dashboard:       ████████████████ 38,000
Reports:         ████████████ 28,000
Integrations:    █████████ 21,000
```
**Insight**: Clear prioritization of most-used features

---

### For Growth Trends:
**Chart**: Line Chart with annotations
```
Revenue ($K)
     │
150  │                          ●─── Q4 (↑ 50% growth)
     │                      ●──● Q3
100  │              ●──────●
     │          ●──● Q2 (Product launch)
 50  │      ●──●
     │  ●──●
  0  └──────────────────────────
     Q1  Q2  Q3  Q4
```
**Insight**: Annotate key events to tell the story

---

## Step 6: Tools Recommendation

Based on user's needs and technical skill:

**Quick & Easy (No Code)**:
- Google Sheets / Excel: For basic charts
- Looker Studio (Google Data Studio): Free dashboards

**PM Analytics Tools** (Built-in Visualizations):
- Mixpanel: Funnels, retention, cohorts
- Amplitude: User behavior analytics
- Heap: Auto-capture events
- PostHog: Open-source product analytics

**Business Intelligence**:
- Tableau: Professional dashboards (requires training)
- Looker: SQL-based BI
- Metabase: Open-source, easy to use
- Mode: SQL + Python + visualization

**For Developers**:
- Python: matplotlib, seaborn, plotly
- JavaScript: D3.js, Chart.js, Recharts

---

## Step 7: Actionable Next Steps

Provide clear next steps based on scenario:

**For Chart Selection**:
- [ ] Identify what you're trying to show (comparison/trend/etc.)
- [ ] Choose appropriate chart type from decision tree
- [ ] Create chart with recommended tool
- [ ] Apply best practices (labels, colors, annotations)
- [ ] Review for common mistakes

**For Chart Interpretation**:
- [ ] Identify chart type
- [ ] Read "How to Read" section for that chart
- [ ] Look for key patterns (flattening, drops, correlations)
- [ ] Extract insights
- [ ] Decide on actions

**For Dashboard Creation**:
- [ ] Define North Star + 3-5 key metrics (top section)
- [ ] Select trends to show (middle section)
- [ ] Add detail tables and filters (bottom section)
- [ ] Review for clarity and actionability
- [ ] Share with stakeholders for feedback

**For Troubleshooting**:
- [ ] Identify specific issue (truncated axis, too many lines, etc.)
- [ ] Apply fix from "Common Mistakes" section
- [ ] Recreate chart with corrections
- [ ] Validate clarity with colleague

---

## Important Reminders

**Chart Best Practices**:
- ✅ Simple > Complex
- ✅ Clarity > Beauty
- ✅ Label everything (axes, title, source, date)
- ✅ Use color purposefully (max 5-7 colors)
- ✅ Start bar charts at zero
- ✅ Annotate key events
- ✅ Make it actionable

**Chart Anti-Patterns**:
- ❌ 3D charts (distort values)
- ❌ Truncated Y-axis (exaggerates)
- ❌ Too many lines (spaghetti)
- ❌ Pie chart for trends (wrong use)
- ❌ No context (unclear if good/bad)
- ❌ Rainbow colors (hard to read)

**Remember**: The best chart is the one that makes the decision obvious.

---

**Primary Framework**: [ANALYTICS-data-visualization-charts.md](../.claude/product-foundation/ANALYTICS-data-visualization-charts.md)

**Related Frameworks**:
- [METRICS-product-metrics.md](../.claude/product-foundation/METRICS-product-metrics.md) - What metrics to visualize
- [METRICS-cohort-analysis.md](../.claude/product-foundation/METRICS-cohort-analysis.md) - Cohort chart deep dive
- [METRICS-retention-churn-analysis.md](../.claude/product-foundation/METRICS-retention-churn-analysis.md) - Retention curves
- [METRICS-aarrr-pirate-metrics.md](../.claude/product-foundation/METRICS-aarrr-pirate-metrics.md) - Funnel charts
- [COMMUNICATION-stakeholder-management.md](../.claude/product-foundation/COMMUNICATION-stakeholder-management.md) - Executive presentations
