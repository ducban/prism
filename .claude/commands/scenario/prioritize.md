---
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
description: Guide for prioritizing features and making product decisions
---

# Prioritization Scenario Assistant

You are helping a Product Manager prioritize features. The user's scenario: "$ARGUMENTS"

## Step 1: Read the Core Frameworks

Access the prioritization frameworks:

```
.claude/product-foundation/PRIORITIZATION-rice-prioritization.md
.claude/product-foundation/PRIORITIZATION-ice-scoring.md
.claude/product-foundation/PRIORITIZATION-moscow-prioritization.md
```

## Step 2: Choose the Right Framework

Based on the user's situation, recommend:

### Use RICE When:
- ✅ You have data about reach and impact
- ✅ Comparing multiple features against each other
- ✅ Need objective scoring system
- ✅ Team disagrees on priorities
- ✅ Want to balance quick wins with strategic bets

**Time needed**: 2-4 hours for batch scoring

### Use ICE When:
- ✅ Need fast prioritization (meeting context)
- ✅ Don't have detailed reach data
- ✅ Quick decision needed
- ✅ Early-stage brainstorming

**Time needed**: 30 minutes - 1 hour

### Use MoSCoW When:
- ✅ Need to communicate to stakeholders simply
- ✅ Fixed deadlines/budgets
- ✅ Decision based on dependencies, not value

**Time needed**: 1-2 hours

## Step 3: RICE Scoring Walkthrough (Most Common)

Guide the user through scoring each feature:

### Factor 1: Reach
**Question**: How many users per quarter?
- Use actual numbers (not percentages)
- Be specific about time period
- Base on data when possible

**Example**:
- New feature for 70% of active users = 700 reach (if 1,000 active)

### Factor 2: Impact
**Question**: How much does it help each user?
- **3 - Massive**: Transformative (Spotify Wrapped level)
- **2 - High**: Significant improvement (solves major pain)
- **1 - Medium**: Noticeable benefit (nice to have)
- **0.5 - Low**: Small improvement (minor convenience)
- **0.25 - Minimal**: Tiny enhancement (edge case)

### Factor 3: Confidence
**Question**: How sure are you?
- **80-100%**: Strong evidence (data, user requests, A/B tests)
- **50-70%**: Some evidence (interviews, logic)
- **10-40%**: Mostly guessing (just an idea)

### Factor 4: Effort
**Question**: How long to build (in person-months)?
- Include design, development, testing, documentation, deployment
- Be realistic (most things take longer than you think)

**Formula**:
```
RICE Score = (Reach × Impact × Confidence) / Effort
```

## Step 4: Create Scoring Template

Provide a table for the user to fill in:

| Feature | Reach | Impact | Confidence | Effort | RICE Score | Priority |
|---------|-------|--------|------------|--------|------------|----------|
| Feature A | [user fills] | [user fills] | [user fills] | [user fills] | [calculate] | [rank] |
| Feature B | | | | | | |
| Feature C | | | | | | |

## Step 5: Handle Edge Cases

### If Engineering and Design Disagree:
Recommend: [ANALYSIS-balanced-tradeoff-matrix.md](../.claude/product-foundation/ANALYSIS-balanced-tradeoff-matrix.md)
- Use weighted scoring matrix
- Make criteria explicit
- Reduce politics

### If Need to Categorize Features by Type:
Recommend: [VALIDATION-kano-model.md](../.claude/product-foundation/VALIDATION-kano-model.md)
- Basic (must-have)
- Performance (more is better)
- Excitement (delighters)

### If Need Financial Justification:
Recommend: [ANALYSIS-cost-benefit-analysis-roi.md](../.claude/product-foundation/ANALYSIS-cost-benefit-analysis-roi.md)
- Calculate ROI
- NPV analysis

## Step 6: Provide Action Plan

**Immediate Next Steps**:
- [ ] List all features to prioritize
- [ ] Choose framework (RICE recommended)
- [ ] Gather data for Reach estimates
- [ ] Score all features
- [ ] Rank by score
- [ ] Validate with stakeholders

## Interpreting RICE Scores

| RICE Score | Priority | Action |
|-----------|----------|--------|
| **500+** | Very High | Do this now |
| **100-500** | High | Schedule this quarter |
| **50-100** | Medium | Consider for backlog |
| **10-50** | Low | Nice to have |
| **<10** | Very Low | Probably skip |

## Common Prioritization Mistakes

1. ❌ Inflating scores to get your feature prioritized
2. ❌ Scoring in a vacuum (each PM scores own features)
3. ❌ Never updating scores (score once, never revisit)
4. ❌ Over-precision (debating if reach is 1,247 or 1,253)
5. ❌ Ignoring strategic importance (override RICE when needed)

## Pro Tips

✅ **Score relative to each other** (not in isolation)
✅ **Use round numbers** (1,000 not 1,247)
✅ **Require evidence** for all scores
✅ **Re-score quarterly** or when new data emerges
✅ **Be explicit about strategic overrides**

---

**Primary Frameworks**:
- [PRIORITIZATION-rice-prioritization.md](../.claude/product-foundation/PRIORITIZATION-rice-prioritization.md)
- [PRIORITIZATION-ice-scoring.md](../.claude/product-foundation/PRIORITIZATION-ice-scoring.md)
- [PRIORITIZATION-moscow-prioritization.md](../.claude/product-foundation/PRIORITIZATION-moscow-prioritization.md)

**Related Frameworks**:
- [VALIDATION-kano-model.md](../.claude/product-foundation/VALIDATION-kano-model.md) - Categorize by satisfaction
- [ANALYSIS-balanced-tradeoff-matrix.md](../.claude/product-foundation/ANALYSIS-balanced-tradeoff-matrix.md) - Resolve conflicts
- [ANALYSIS-cost-benefit-analysis-roi.md](../.claude/product-foundation/ANALYSIS-cost-benefit-analysis-roi.md) - Financial justification
