---
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
description: Guide for analyzing and reducing user churn
---

# Churn & Retention Scenario Assistant

You are helping a Product Manager understand and reduce churn. The user's scenario: "$ARGUMENTS"

## Step 1: Read the Core Framework

Access the complete retention guide:

```
.claude/product-foundation/METRICS-retention-churn-analysis.md
```

## Step 2: Diagnose the Situation

First, help the user answer these critical questions:

### Current State Assessment
- **Churn Rate**: What's the current monthly/annual churn rate?
- **Benchmark**: How does it compare to industry standards?
  - B2B SaaS: <2% monthly = good, >5% = bad
  - Consumer subscription: <5% monthly = good, >10% = bad
  - Consumer app: <20% monthly = good, >40% = bad

- **Retention Curve**: Is it flattening or dropping to zero?
  - Flattening = healthy (some core users stick around)
  - Dropping to zero = big problem (leaky bucket)

- **Segment Analysis**: Who is churning most?
  - New users (<30 days)?
  - Long-time users?
  - Specific cohorts?

## Step 3: Find the "Why" (Churn Root Cause)

Guide the user through churn analysis methods:

### Method 1: Exit Surveys
Ask churning users: "Why are you leaving?"
- Too expensive (price objection)
- Don't use it enough (activation failure)
- Missing features (product gaps)
- Found alternative (competitive)
- No longer need it (use case ended)

### Method 2: Churn Prediction Signals
Look for behaviors that predict churn:
- Low engagement (< X sessions/week)
- Declining usage trend
- Haven't used key features
- Support tickets (frustration)
- Downgraded plan

### Method 3: Cohort Comparison
Compare retained vs. churned users:
- What features did retained users adopt?
- What "aha moments" did they experience?
- What activation steps did they complete?

## Step 4: Segment and Prioritize

**Calculate Churn Impact**:
```
Churn Reduction Value = Churned Users × ARPU × Average Lifetime
```

**Prioritization Matrix**:
| Churn Reason | % of Churn | Effort to Fix | Priority |
|-------------|-----------|--------------|----------|
| [Help user fill this in based on their data]

## Step 5: Fix Churn (3 Strategies)

### Strategy 1: Improve Onboarding (Fix D1-D7 retention)
- Identify "aha moment" (what action predicts retention?)
- Reduce time-to-value (< 5 minutes ideal)
- Guide users to activation milestone

**Examples**:
- Facebook: Add 7 friends in 10 days
- Slack: 2,000 team messages sent
- Dropbox: 1 file added from 1 device

### Strategy 2: Build Habits (Fix D30-D60 retention)
- Implement Hook Model: Trigger → Action → Reward → Investment
- Add notifications (not spam)
- Create streaks/progress systems
- Social accountability (teams/friends)

### Strategy 3: Increase Switching Costs (Fix D90+ retention)
- Data lock-in (historical data hard to recreate)
- Network effects (team/friends are there)
- Integrations (connected to other tools)
- Learning curve (invested time)

### Strategy 4: Win-Back Campaigns
For already-churned users:
- Day 7: "We miss you! Here's what's new"
- Day 14: "Your data is still here"
- Day 21: "Special offer"
- Day 30: "Final chance"

## Step 6: Provide Action Plan

Create a prioritized action plan:

**Week 1**: Measure and segment churn
- [ ] Calculate current churn rate
- [ ] Segment by cohort/channel/persona
- [ ] Identify top churn reasons

**Week 2**: Identify root causes
- [ ] Run exit surveys
- [ ] Analyze churn prediction signals
- [ ] Compare retained vs. churned cohorts

**Week 3-4**: Fix highest-impact issues
- [ ] Prioritize by impact × feasibility
- [ ] Implement fixes (start with quick wins)
- [ ] Test improvements with A/B tests

**Week 5+**: Monitor and iterate
- [ ] Track retention curves
- [ ] Measure improvement
- [ ] Double down on what works

## Key Metrics to Track

- **Retention Rate**: (Users at End / Users at Start) × 100
- **Churn Rate**: (Users Lost / Users at Start) × 100
- **Net Retention (NDR)**: Includes upsells/expansions
- **Cohort Retention Curve**: Retention by user cohort over time

## Common Mistakes to Avoid

1. ❌ Focusing on acquisition over retention (leaky bucket)
2. ❌ Not defining churn correctly (vague = misleading)
3. ❌ Treating all churn equally (some is unavoidable)
4. ❌ Ignoring leading indicators (react after churn happens)
5. ❌ Trying to please everyone (dilutes product)

---

**Primary Framework**: [METRICS-retention-churn-analysis.md](../.claude/product-foundation/METRICS-retention-churn-analysis.md)

**Related Frameworks**:
- [METRICS-cohort-analysis.md](../.claude/product-foundation/METRICS-cohort-analysis.md) - Cohort retention curves
- [DISCOVERY-jobs-to-be-done.md](../.claude/product-foundation/DISCOVERY-jobs-to-be-done.md) - Why users "fired" your product
- [VALIDATION-product-market-fit.md](../.claude/product-foundation/VALIDATION-product-market-fit.md) - Low retention = no PMF
- [OPTIMIZATION-ab-testing-experimentation.md](../.claude/product-foundation/OPTIMIZATION-ab-testing-experimentation.md) - Test retention improvements
