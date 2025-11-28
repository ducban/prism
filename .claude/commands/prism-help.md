---
allowed-tools: Read
description: Welcome guide for first-time PRISM users with real-world examples
---

# Welcome to PRISM! 🌈

**Lăng kính** - *Taking complex PM problems (white light) and breaking them into understandable components (rainbow colors)*

---

## What is PRISM? (In Plain English)

Think of PRISM as your **personal PM coach** who has already read all the textbooks, so you don't have to.

### The Old Way ❌
```
You: "How do I prioritize features?"
Google: Here are 47 blog posts, 12 frameworks, and 200 pages to read
You: *spends 3 hours reading, still confused*
```

### The PRISM Way ✅
```
You: /assist I need to prioritize features
Claude: [Reads 50-page RICE framework internally]
Claude: Here's exactly how to do it + a 5-step action plan
You: *starts working in 5 minutes*
```

**Bottom line**: You ask questions in plain English, Claude reads the expert frameworks behind the scenes, you get direct answers + keywords to learn more if you want.

---

## Real-World Examples

### Example 1: You're Launching a Product Tomorrow

**Without PRISM**:
- Panic Google: "product launch checklist"
- Find 10 different checklists
- Spend 2 hours creating your own
- Still miss critical steps

**With PRISM**:
```
You: /scenario:launch I'm launching our mobile app tomorrow, what should I do?

Claude reads 3 frameworks silently (GTM strategy, PMF validation, North Star metrics)

Claude responds with:
- Pre-launch checklist (15 items)
- Day-of-launch checklist (8 items)
- Post-launch monitoring plan
- Common mistakes to avoid
- Keywords: "product launch tiers", "go-to-market strategy", "launch readiness"

Time saved: 90 minutes
Stress reduced: Significantly
```

### Example 2: Your Boss Asks "Do We Have Product-Market Fit?"

**Without PRISM**:
- Google PMF definitions
- Read Marc Andreessen's essay
- Read Sean Ellis's blog
- Still not sure how to measure it
- Meeting in 2 hours, still no answer

**With PRISM**:
```
You: /scenario:pmf CEO is asking about PMF, how do I validate this?

Claude reads PMF validation framework silently

Claude responds with:
- 5 specific PMF signals to measure
- The "40% rule" (Sean Ellis test)
- Retention curve analysis steps
- How to run the PMF survey
- Red flags that you DON'T have PMF
- Action plan for your meeting

Time to clear answer: 10 minutes
Confidence in meeting: High
```

### Example 3: Users Are Leaving After 2 Weeks

**Without PRISM**:
- Google "reduce churn"
- Get overwhelmed with analytics tools
- Not sure where to start
- Guessing at solutions

**With PRISM**:
```
You: /scenario:churn Users sign up but leave after 2 weeks, why?

Claude reads retention & churn framework silently

Claude responds with:
- Cohort analysis methodology (step-by-step)
- How to identify "aha moment" timing
- User journey friction point analysis
- Exit interview question templates
- Retention curve benchmarks
- Keywords: "time-to-value", "cohort retention", "aha moment"

Next steps: Crystal clear
Root cause hunting: Systematic approach
```

### Example 4: Stakeholder Won't Prioritize Your Feature

**Without PRISM**:
- Try to "sell" the feature emotionally
- Get shot down
- Feel frustrated
- Give up or keep pushing (both bad outcomes)

**With PRISM**:
```
You: /assist I need to convince my VP to prioritize this authentication feature but she keeps saying no

Claude reads Influence Without Authority + Stakeholder Management frameworks

Claude responds with:
- RICE score calculation (quantify impact)
- Stakeholder mapping (understand her motivations)
- Influence tactics (speaking her language: business impact)
- How to reframe the conversation
- When to push back vs. when to let go
- Keywords: "influence without authority", "stakeholder alignment", "business case"

Approach: Data-driven instead of emotional
Outcome: More likely to succeed or understand why it's truly not a priority
```

---

## How Does It Actually Work?

### Behind the Scenes

1. **You ask a question** (in normal human language)
2. **Claude identifies relevant frameworks** from 45 PM frameworks
3. **Claude reads them silently** (you never see this step)
4. **Claude synthesizes the answer** tailored to YOUR specific situation
5. **You get**:
   - Direct, actionable answer
   - Step-by-step action plan
   - Common mistakes to avoid
   - Keywords to research deeper if you want

### What's in PRISM's Brain? (45 Frameworks)

Think of it like a PM library with 45 expert books:

**When you need to understand users**:
- Jobs-to-Be-Done (why people "hire" products)
- Persona Development (who are your users)
- Value Proposition (what value do you deliver)

**When you need to prioritize**:
- RICE (Reach × Impact × Confidence / Effort)
- ICE (Impact × Confidence × Ease)
- MoSCoW (Must/Should/Could/Won't)

**When you need to validate ideas**:
- Product-Market Fit (are you solving a real problem?)
- Kano Model (which features delight vs. frustrate)

**When you need to analyze**:
- Market Sizing (TAM/SAM/SOM)
- Cost-Benefit Analysis (is this worth it?)

**When you need to launch**:
- Go-to-Market Strategy (how to launch successfully)

**When you need to measure success**:
- North Star Metric (one metric that matters)
- AARRR Pirate Metrics (acquisition → retention → revenue)
- Cohort Analysis (how users behave over time)

**When you need to manage people**:
- Interviewing Framework (hire the right PMs)
- Feedback Framework (give/receive feedback effectively)
- One-on-One Framework (have productive 1:1s)

**When you need to influence**:
- Stakeholder Management (align executives)
- Influence Without Authority (get things done)

**Domain-specific**:
- FinTech (payment systems, financial inclusion, business models)
- TravelTech (booking optimization, industry insights)
- UX/UI (research methods, design process, UI optimization)

**Total**: 45 comprehensive frameworks covering Discovery, Prioritization, Validation, Analysis, Strategy, Documentation, Execution, Launch, Optimization, Metrics, Analytics, Psychology, People, Communication, and domain expertise.

---

## Available Commands

### 🎯 Smart Assistant (Start Here!)

**`/assist [your question]`**
The smart router. Just describe your problem in plain English.

**Examples**:
```
/assist I need to prioritize 15 features for Q2
/assist My users are churning and I don't know why
/assist How do I convince executives to invest in this?
/assist I'm interviewing a senior PM candidate tomorrow
```

### 📋 Scenario-Specific Commands

Use these when you know exactly what scenario you're in:

**`/scenario:prioritize`** - Need to rank features/ideas
**`/scenario:pmf`** - Validate product-market fit
**`/scenario:churn`** - Users are leaving, need to fix retention
**`/scenario:launch`** - Launching a product/feature
**`/scenario:interview`** - Preparing for PM interviews (giving or receiving)
**`/scenario:feedback`** - Giving or receiving feedback
**`/scenario:chart`** - Choose the right chart/visualization

### 🛠️ Helper Commands

**`/gh:commit`** - Smart git commit helper
**`/gh:init`** - Initialize git repository
**`/prism-help`** - This guide (welcome back anytime!)

---

## Quick Start: Your First 3 Commands

### 1. Try the Smart Assistant
```
/assist I need help with [your actual problem]
```
This is the easiest way to start. Just describe what you're stuck on.

### 2. Test a Scenario Command
```
/scenario:prioritize I have 10 features and need to pick 3 for next sprint
```
See how targeted guidance works.

### 3. Explore When Curious
```
/assist What PM frameworks does PRISM know about?
```
Learn what's available.

---

## Common Questions

### "Do I need to read framework documents?"

**No!** That's the whole point. Claude reads them for you. You just get the insights.

### "How is this different from ChatGPT/Gemini?"

Three key differences:
1. **Curated frameworks**: 45 vetted PM methodologies (not random internet knowledge)
2. **Conversation continuity**: PRISM remembers your previous questions
3. **Synthesis approach**: Direct answers + keywords (not "go read this article")

### "What if I want to learn the framework deeply?"

Perfect! Every response includes 5-7 **keywords for research**. Use those to Google and dive deeper on your own time.

Example:
```
Keywords: RICE prioritization, opportunity cost, value vs effort matrix
```
Now you can research these at your own pace.

### "Can I use this for non-PM stuff?"

PRISM is built for PM work, but the frameworks help with:
- Product Design (UX/UI frameworks)
- Engineering Management (prioritization, roadmapping)
- Startup Founders (PMF, GTM, market sizing)
- Anyone making product decisions

### "How do I know which command to use?"

**Easy**: Just use `/assist [your question]` - it's smart enough to figure it out.

**When you want speed**: Use specific `/scenario:*` commands if you already know the category.

---

## Pro Tips for New Users

### 1. Be Specific
❌ "Help with my product"
✅ "I'm launching a B2B SaaS product next month and need a GTM checklist"

### 2. Include Context
The more context you give, the more tailored the answer:
- Your role (PM, founder, designer)
- Your product type (B2B, B2C, marketplace)
- Your stage (idea, launch, growth, scaling)
- Your constraint (time, budget, team size)

### 3. Ask Follow-ups
PRISM tracks conversations! You can say:
```
/assist I need to prioritize features
[Claude responds with RICE framework]

You: "How do I estimate Reach accurately?"
[Claude provides deeper guidance on Reach estimation]
```

### 4. Use Real Examples
Instead of hypotheticals, use your actual work:
```
/assist We have 10K users but only 500 are active weekly. Is this a retention problem or an engagement problem?
```

### 5. Don't Overthink It
There's no "wrong" way to ask. Just type your question naturally.

---

## Real Users, Real Scenarios

### Junior PM (First Month on Job)
```
/assist I just joined as a PM and my first task is to create a roadmap. I have no idea where to start.

[Claude synthesizes roadmapping framework]
- Now vs. Next vs. Later framework
- Stakeholder input gathering
- Theme-based vs. feature-based roadmaps
- How to handle "everything is urgent"
- Roadmap presentation tips
```

### Founder (Building MVP)
```
/scenario:pmf We launched 2 months ago, have 100 users, 30% come back weekly. Do we have PMF?

[Claude reads PMF validation framework]
- Sean Ellis test: Would users be "very disappointed" if product disappeared?
- 40% rule benchmark
- Retention curve analysis (30% weekly is decent but check if it's flattening)
- Qualitative signals to look for
- When to pivot vs. persevere
```

### Senior PM (Stakeholder Conflict)
```
/assist Engineering wants to build v2 of the platform but Sales is demanding 15 new features. How do I resolve this?

[Claude reads Stakeholder Management + Influence frameworks]
- Map stakeholder power/interest (2x2 matrix)
- Find shared goals (revenue growth? customer satisfaction?)
- Reframe the debate (v2 enables faster feature development long-term)
- Propose hybrid approach (v2 Phase 1 + critical sales features)
- Use data to depersonalize the decision
```

---

## What Happens Next?

After you run your first command:

1. **You get an answer** (synthesized from expert frameworks)
2. **You get an action plan** (concrete next steps)
3. **You get keywords** (for deeper learning if you want)
4. **The conversation is saved** (in PRISM-CONVOS/ automatically)

Next time you ask a related question, Claude remembers the context!

---

## Remember

**PRISM is here to make you better at your job, not replace your thinking.**

You still:
- Make the final decisions
- Apply context your team knows
- Use your judgment

PRISM just:
- Saves you research time
- Provides structured approaches
- Helps you avoid common mistakes
- Gives you confidence in your methods

---

## Ready to Start?

Try one of these right now:

```
/assist What should I work on today?
```
```
/scenario:prioritize I have 8 feature requests from customers, how do I choose?
```
```
/assist How do I know if we have product-market fit?
```

**Welcome to PRISM!** You're going to do great. 🌈

---

*For detailed documentation, see:*
- `README.md` - User guide
- `RULES.md` - How PRISM works
- `CLAUDE.md` - Technical details

*For help, just ask:*
```
/assist I'm stuck on [your problem]
```
