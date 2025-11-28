---
allowed-tools: Read, Grep
description: Guide for validating product-market fit
---

# Product-Market Fit Validation Assistant

You are helping a Product Manager validate product-market fit. The user's scenario: "$ARGUMENTS"

## Step 1: Read the Framework

```
.claude/product-foundation/VALIDATION-product-market-fit.md
```

## Step 2: Run the Sean Ellis Test

This is the GOLD STANDARD for PMF measurement.

### The PMF Question:
Ask your users: **"How would you feel if you could no longer use this product?"**

**Options**:
- Very disappointed
- Somewhat disappointed
- Not disappointed (it isn't really that useful)
- N/A - I no longer use it

### The PMF Threshold:
- **≥40% "Very disappointed"** = You have PMF ✅
- **25-40%** = Getting close, needs work 🟡
- **<25%** = No PMF yet ❌

### Survey Setup:
- **Who**: Active users who've used product ≥3 times
- **Sample size**: Minimum 40 responses (ideally 100+)
- **Timing**: After users experience core value (e.g., 1 week of use)
- **Tool**: Typeform, Google Forms, or in-app survey

## Step 3: Check Alternative PMF Signals

Beyond the Sean Ellis test, look for:

### 1. Retention Cohorts
- **PMF Signal**: Retention curve flattens (not dropping to zero)
- **Example**: WhatsApp has 70% Day-30 retention

### 2. Organic Growth Rate
- **PMF Signal**: >20% month-over-month organic growth (not paid)
- **Example**: Dropbox grew 3900% in 15 months (mostly referrals)

### 3. Net Promoter Score (NPS)
- **PMF Signal**: NPS > 50
- **Formula**: % Promoters (9-10) - % Detractors (0-6)

### 4. Customer Acquisition Cost (CAC) Payback
- **PMF Signal**: <12 months payback
- **Formula**: CAC / Monthly Revenue per Customer

### 5. Engagement (DAU/MAU)
- **PMF Signal**:
  - Social products: >20%
  - SaaS products: >40%
  - Consumer apps: >60%

### 6. Churn Rate
- **PMF Signal**:
  - Consumer: <5% monthly churn
  - B2B: <2% monthly churn

## Step 4: Interpret Results

### Scenario A: High PMF Score (≥40%)
✅ **You have PMF!**

**Next Steps**:
- Scale through marketing and sales
- Double down on what works
- Don't break what users love

**Related Framework**: [LAUNCH-go-to-market-strategy.md](../.claude/product-foundation/LAUNCH-go-to-market-strategy.md)

### Scenario B: Medium PMF Score (25-40%)
🟡 **Close but not there yet**

**Next Steps**:
1. Segment users by PMF score
2. Analyze "very disappointed" users:
   - Who are they? (Role, industry, use case)
   - What do they love? (Main benefit)
   - Find common patterns
3. **Double down on that segment**
4. Build for them, ignore others temporarily
5. Re-survey in 3 months

**Case Study**: Superhuman went from 22% → 58% in 12 months using this approach

### Scenario C: Low PMF Score (<25%)
❌ **No PMF yet**

**Next Steps**:
1. **Don't scale GTM!** (Will burn money)
2. Talk to users - understand why (use survey Q3 & Q4)
3. Options:
   - **Iterate**: Fix value proposition based on feedback
   - **Pivot**: Try different customer segment or use case
   - **Persist**: Sometimes 25% → 40% is just a few improvements away

**WARNING**: Don't pivot too early. If 25-40%, dig deeper first.

## Step 5: The PMF Pyramid

If you don't have PMF, work through Dan Olsen's pyramid:

```
     ┌─────────────────┐
     │   UX (Layer 5)  │
     ├─────────────────┤
     │ Feature Set (4) │
     ├─────────────────┤
     │ Value Prop (3)  │
     ├─────────────────┤
     │ Underserved (2) │
     ├─────────────────┤
     │Target Customer 1│
     └─────────────────┘
```

Fix from bottom up:
1. **Layer 1**: Right target customer?
2. **Layer 2**: Solving underserved needs?
3. **Layer 3**: Clear value proposition?
4. **Layer 4**: Right features?
5. **Layer 5**: Delightful UX?

## Common PMF Mistakes

1. ❌ **Confusing PMF with growth**: You can grow without PMF (paid ads), but it's unsustainable
2. ❌ **Declaring PMF too early**: 40% with 50 users ≠ PMF (sample too small)
3. ❌ **Scaling before PMF**: GTM without PMF = leaky bucket
4. ❌ **Ignoring retention**: High signups but low retention = no PMF
5. ❌ **Stopping after achieving PMF**: PMF can be lost, keep measuring

## PMF Action Plan

**Week 1-2**: Measure
- [ ] Run Sean Ellis survey (40+ responses)
- [ ] Check retention cohorts
- [ ] Calculate DAU/MAU, NPS, churn

**Week 3-4**: Analyze
- [ ] Interpret PMF score
- [ ] Segment by user type
- [ ] Identify patterns in "very disappointed" users

**Week 5+**: Act
- [ ] If PMF (≥40%): Scale GTM
- [ ] If close (25-40%): Double down on core segment
- [ ] If no PMF (<25%): Iterate or pivot

---

**Primary Framework**: [VALIDATION-product-market-fit.md](../.claude/product-foundation/VALIDATION-product-market-fit.md)

**Related Frameworks**:
- [METRICS-retention-churn-analysis.md](../.claude/product-foundation/METRICS-retention-churn-analysis.md) - Retention signals
- [DISCOVERY-value-proposition-canvas.md](../.claude/product-foundation/DISCOVERY-value-proposition-canvas.md) - Fix value prop
- [LAUNCH-go-to-market-strategy.md](../.claude/product-foundation/LAUNCH-go-to-market-strategy.md) - Scale after PMF
