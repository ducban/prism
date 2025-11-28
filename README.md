# PRISM

**Product Management Capability Toolkit for Claude Code**

*Lăng kính: Taking complex PM problems (white light) and breaking them into understandable components (rainbow colors)*

---

## What is PRISM?

PRISM is an AI-powered PM capability toolkit that provides on-demand product management competencies through Claude Code slash commands. Get expert PM guidance synthesized from 45 comprehensive frameworks - without reading lengthy documentation.

**Version**: 1.0
**Platform**: Claude Code
**Frameworks**: 45 comprehensive PM frameworks
**Commands**: 10 slash commands
**Status**: ✅ Production Ready

---

## Quick Start

### Installation

1. Clone this repository:
   ```bash
   git clone <your-repo-url> prism
   cd prism
   ```

2. Open in Claude Code:
   ```bash
   code .
   ```

3. Start using slash commands:
   ```
   /assist I need to prioritize features for Q2
   ```

That's it! No configuration needed.

---

## How It Works

### The PRISM Philosophy

**Traditional approach**: "Read this 50-page framework document"
**PRISM approach**: Claude reads it, you get synthesized guidance + keywords for deeper research

```
You ask: "How do I prioritize features?"

Claude:
1. Reads RICE prioritization framework silently
2. Synthesizes the methodology for your context
3. Provides actionable steps
4. Shares keywords for independent research

You get: Direct guidance + ability to learn more on your own
```

### Core Principles

- **Capability over complexity**: Frameworks are tools, not rules
- **Synthesis over signposting**: Get answers, not file paths
- **Keywords over links**: Learn independently with research terms
- **Context continuity**: Conversations are tracked and continued
- **No workflow enforcement**: Use what you need, when you need it

---

## Available Commands

### Smart Assistant

**`/assist [description]`**
AI-powered framework navigator that analyzes your scenario and provides synthesized guidance from relevant frameworks.

```
/assist I'm launching a new product next month
/assist Users are churning and I don't know why
/assist Need to convince executives to prioritize this feature
```

### Scenario Commands

**`/scenario:feedback`** - Giving/receiving effective feedback
**`/scenario:prioritize`** - Feature prioritization
**`/scenario:chart`** - Data visualization guidance
**`/scenario:interview`** - PM interview preparation
**`/scenario:launch`** - Product launch & GTM planning
**`/scenario:churn`** - Churn analysis & retention
**`/scenario:pmf`** - Product-Market Fit validation

### Git Helpers

**`/gh:commit`** - Analyze changes and create commit
**`/gh:init`** - Initialize git repository

---

## Framework Library

PRISM includes 45 comprehensive PM frameworks across 15 categories:

### Discovery & Research (6)
- Jobs-to-Be-Done (JTBD)
- Persona Development
- Value Proposition Canvas
- Opportunity Solution Tree
- Double Diamond
- Design Thinking & Lean Startup

### Prioritization (3)
- RICE Prioritization
- ICE Scoring
- MoSCoW Prioritization

### Validation (2)
- Product-Market Fit (PMF)
- Kano Model

### Analysis (4)
- Market Sizing (TAM/SAM/SOM)
- Cost-Benefit Analysis & ROI
- MECE Framework
- Balanced Tradeoff Matrix

### Strategy (3)
- Product Roadmapping
- SWOT Analysis
- Product-Led Growth (PLG)

### Documentation (2)
- PRD Template
- User Story Mapping

### Execution (1)
- OKRs (Objectives & Key Results)

### Launch (1)
- Go-to-Market (GTM) Strategy

### Optimization (1)
- A/B Testing & Experimentation

### Metrics (6)
- Product Metrics
- North Star Framework
- AARRR (Pirate Metrics)
- Retention & Churn Analysis
- Cohort Analysis
- Feature Adoption

### Analytics (1)
- Data Visualization & Charts

### Psychology (1)
- Gamification Tactics

### People Management (3)
- Interviewing Framework
- Feedback Framework
- One-on-One Framework

### Communication (2)
- Stakeholder Management
- Influence Without Authority

### Domain-Specific (8)
- **FinTech** (3): Financial Inclusion, Payment Systems, Business Models
- **TravelTech** (2): Industry Overview, Optimization Strategies
- **UX/UI** (3): UX Research, UX Design, UI Optimization

---

## Example Usage

### Example 1: Feature Prioritization

```
You: /assist I need to prioritize 10 features for Q2

Claude:
🎯 I Understand Your Scenario
You need a systematic way to evaluate and rank 10 features for Q2 planning.

📚 Framework Approach: RICE Prioritization

Core methodology:
RICE helps you score features objectively using 4 factors:
- Reach: How many users affected? (estimate 0-1000+)
- Impact: Value per user (Minimal=0.25, Low=0.5, Medium=1, High=2, Massive=3)
- Confidence: How certain are you? (Low=50%, Medium=80%, High=100%)
- Effort: Person-months required

Score = (Reach × Impact × Confidence) / Effort

⚡ Quick Action Plan
- [ ] List all 10 features in a spreadsheet
- [ ] For each feature, estimate Reach (# of users)
- [ ] Rate Impact using the 0.25-3 scale
- [ ] Assign Confidence percentage
- [ ] Estimate Effort in person-months
- [ ] Calculate RICE scores
- [ ] Prioritize top 3-5 highest scores

Time estimate: 2-3 hours

🎓 Key Takeaway
RICE removes gut feeling from prioritization by forcing you to quantify impact,
reach, and effort for every feature.

💡 Pro Tips
- Don't overthink precision - rough estimates work fine
- Review scores with your team to calibrate assumptions
- Revisit quarterly as market conditions change

🔍 Keywords for Further Research
- RICE prioritization framework
- Opportunity cost analysis
- Value vs effort matrix
- Feature scoring methodologies
- Product prioritization best practices
```

### Example 2: Churn Analysis

```
You: /scenario:churn Users are leaving after 2 weeks

Claude:
🎯 I Understand Your Scenario
You're experiencing churn at the 2-week mark - users aren't sticking around.

📚 Framework Approach: Retention & Churn Analysis

Core methodology:
1. Measure cohort retention curves
2. Identify the "aha moment" (when users see value)
3. Calculate time-to-value
4. Analyze drop-off points

Key concepts:
- Cohort analysis: Group users by signup date, track retention %
- Retention curve: Should flatten after 4-6 weeks (PMF signal)
- Churn signals: Feature abandonment, decreased activity, support tickets

Common pitfalls:
- Focusing on acquisition before fixing retention
- Not segmenting users (power users vs casual)
- Ignoring qualitative feedback

⚡ Quick Action Plan
- [ ] Create cohort retention table (Week 0, 1, 2, 3, 4+)
- [ ] Calculate retention % for each cohort
- [ ] Identify commonalities among churned users
- [ ] Interview 5-10 churned users (exit interviews)
- [ ] Map user journey to find friction points

Time estimate: 1 week for analysis

🔍 Keywords for Further Research
- Cohort retention analysis
- Time-to-value metrics
- Aha moment identification
- User onboarding optimization
- Retention curve analysis
```

---

## Data Storage

PRISM includes a structured `data/` directory for organizing PM work products:

```
data/
├── items/              # Categorized PM items
│   ├── ideas/          # Product ideas
│   ├── incidents/      # Production incidents
│   ├── initiatives/    # Strategic initiatives
│   ├── csat/           # Customer satisfaction issues
│   └── [10 more categories]
├── prds/              # Product Requirements Documents
├── roadmaps/          # Roadmap files
├── metrics/           # Analytics dashboards
├── retrospectives/    # Retrospective records
└── scores/            # Prioritization scores
```

All files use YAML frontmatter for consistency and searchability.

---

## Conversation Tracking

PRISM automatically tracks all conversations in `PRISM-CONVOS/` to maintain context across sessions:

- **Continuous context**: Pick up where you left off
- **No duplicates**: Related questions are grouped together
- **Searchable**: Find past conversations by topic
- **Organized**: YAML metadata for every conversation

You don't need to do anything - Claude handles this automatically.

---

## Project Structure

```
prism/
├── PRISM-CONVOS/              # Your conversation history
├── data/                      # Your PM work products
├── .claude/
│   ├── commands/              # 10 slash commands
│   └── product-foundation/    # 45 frameworks (hidden)
├── CLAUDE.md                  # Claude Code guidance
├── RULES.md                   # Detailed project rules
└── README.md                  # This file
```

**Note**: Frameworks in `.claude/product-foundation/` are hidden - Claude reads them, you get synthesized insights.

---

## FAQ

### Do I need to read the framework files?

**No!** That's the whole point of PRISM. Claude reads the frameworks and synthesizes them into actionable guidance for you. You get:
- Direct, contextualized advice
- Actionable steps
- Keywords for deeper research if you want to learn more

### How is this different from searching Google?

PRISM provides:
1. **Contextualized guidance**: Tailored to your specific scenario
2. **Synthesized insights**: Combined knowledge from multiple frameworks
3. **Actionable steps**: Not just theory, but what to do next
4. **Conversation continuity**: Build on previous discussions
5. **45 curated frameworks**: Vetted PM methodologies in one place

### Can I still access the frameworks directly?

Yes, they're in `.claude/product-foundation/`, but:
- They're optimized for Claude to read (bilingual, comprehensive)
- You'll get faster value from synthesized guidance
- Use keywords provided to research topics independently

### What if I need a framework that's not included?

Use `/assist [description]` and Claude will:
1. Check if an existing framework covers it
2. Synthesize guidance from related frameworks
3. Provide keywords for you to research the specific area

### Is this only for Product Managers?

PRISM is built for PMs, but useful for:
- Product Designers (UX/UI frameworks)
- Engineering Managers (prioritization, roadmapping)
- Founders (PMF, GTM, market sizing)
- Anyone making product decisions

---

## Version History

### PRISM v1.0 (Current - 2025-11-28)
- Claude Code only (production-ready)
- 45 frameworks, 10 commands
- Framework synthesis approach
- Hidden framework library
- Streamlined structure

### Root v2.1 (Previous - 2025-11-24)
- Multi-platform (5 AI platforms)
- 65 command files
- Framework file recommendations

### Root v2.0 (2025-11-20)
- Capability toolkit approach
- Multi-platform support added

### Productify (Original - 2024)
- Workflow-based PM assistant
- Single platform

---

## Contributing

PRISM is a personal PM toolkit. If you want to:
- **Add frameworks**: Create `.md` file in `.claude/product-foundation/`
- **Add commands**: Create `.md` file in `.claude/commands/`
- **Improve existing frameworks**: Edit files directly

Follow existing patterns (see `RULES.md` for guidelines).

---

## License

See `LICENSE` file.

---

## Support

For issues or questions:
- Check `RULES.md` for detailed guidelines
- Check `CLAUDE.md` for Claude Code specifics
- Review conversation logs in `PRISM-CONVOS/`

---

**Remember**: PRISM is about capability, not complexity. You ask, Claude reads the frameworks, you get synthesized guidance. Simple as that.

**Made with PRISM** 🌈
