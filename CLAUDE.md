# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with this repository.

---

## Project Overview

**PRISM** (Lăng kính) is an AI-powered PM capability toolkit that provides on-demand product management competencies through Claude Code slash commands.

**Concept**: A prism to help Product Managers see the full spectrum of possibilities within a problem.

**Core Philosophy**: Independent capabilities, user freedom, no workflow enforcement. Each capability works standalone without prerequisites.

**Status**: Production ready (PRISM v1.0) with 45 comprehensive PM frameworks, 10 slash commands, and streamlined documentation.

---

## Project Structure

```
prism/
├── PRISM-CONVOS/              # Conversation tracking (mandatory)
│   └── 00-CONVO-LOGS.md       # Conversation index
├── data/                      # PM work products
│   ├── items/                 # Categorized PM items (ideas, incidents, etc.)
│   ├── prds/                  # Product Requirements Documents
│   ├── roadmaps/              # Roadmap files
│   ├── metrics/               # Analytics dashboards
│   ├── retrospectives/        # Retrospective records
│   └── scores/                # Prioritization scores
├── .claude/
│   ├── commands/              # Claude Code slash commands
│   │   ├── assist.md          # AI framework navigator
│   │   ├── scenario/          # Scenario-specific commands
│   │   │   ├── feedback.md
│   │   │   ├── prioritize.md
│   │   │   ├── chart.md
│   │   │   ├── interview.md
│   │   │   ├── launch.md
│   │   │   ├── churn.md
│   │   │   └── pmf.md
│   │   └── gh/                # Git helper commands
│   │       ├── commit.md
│   │       └── init.md
│   └── product-foundation/    # 45 PM frameworks (HIDDEN - Claude's reference library)
│       ├── COMPETENCY-MAP.md
│       ├── SCENARIO-INDEX.md
│       └── [45 framework files]
├── RULES.md                   # Comprehensive project rules
├── README.md                  # User-facing documentation
└── .gitignore                 # Git ignore rules
```

---

## Critical Rules

### 1. Conversation Tracking (MANDATORY)

**BEFORE ANY RESPONSE**, you MUST:

1. Check `PRISM-CONVOS/00-CONVO-LOGS.md` for existing conversations
2. Search by topic keywords from user input
3. If matching conversation exists:
   - Read the full conversation file
   - Continue the existing conversation
   - Update `date_modified` in YAML header
   - DO NOT create duplicate conversations
4. If no match exists:
   - Generate filename: `yyyy-mm-dd-topic-keywords.md`
   - Create with YAML frontmatter (see RULES.md)
   - Add entry to `00-CONVO-LOGS.md` immediately

**Conversation File Format:**
```yaml
---
conversation_id: "yyyy-mm-dd-topic-name"
date_created: "yyyy-mm-dd"
date_modified: "yyyy-mm-dd"
topic: "Topic Description"
status: "active"
participants:
  - role: "user"
    name: "User"
  - role: "assistant"
    platform: "claude-code"
tags: ["tag1", "tag2"]
summary: "Brief summary"
related_files: []
---
```

### 2. Project References

- **Project name**: Always "PRISM" (never "Root" or "Productify")
- **Version**: PRISM v1.0
- **Framework directory**: `.claude/product-foundation/` (hidden from users)
- **Conversation directory**: `PRISM-CONVOS/`
- **Data directory**: `data/`

### 3. Framework Usage Philosophy

**CRITICAL**: Frameworks in `.claude/product-foundation/` are YOUR reference library, NOT user-facing documentation.

**How to use frameworks**:
1. ✅ **Read frameworks silently** - users don't see this
2. ✅ **Synthesize content** - extract concepts, steps, examples
3. ✅ **Provide direct guidance** - give actionable advice
4. ✅ **Share keywords** - for user self-research
5. ❌ **Never say "read this file"** - users can't access hidden directory
6. ❌ **Never show file paths** - frameworks are invisible to users

**Example**:
```
❌ BAD: "Read .claude/product-foundation/PRIORITIZATION-rice-prioritization.md"
✅ GOOD: "For feature prioritization, use the RICE framework:
         - Reach: How many users affected (0-1000+)?
         - Impact: Value per user (Minimal=0.25, Low=0.5, Medium=1, High=2, Massive=3)
         - Confidence: How certain (Low=50%, Medium=80%, High=100%)
         - Effort: Person-months required

         Score = (Reach × Impact × Confidence) / Effort

         Keywords for research: RICE scoring, opportunity cost, value vs effort matrix"
```

### 4. Anti-Hallucination Protocol

- Never invent data or assume completion
- Validate directory structures before claiming tasks done
- Use evidence-based progress reporting
- Cross-reference with existing files
- Always prompt for missing arguments (never hallucinate values)

---

## Key Documentation Files

### Essential Reading
- **RULES.md**: Comprehensive project rules for PRISM v1.0
- **README.md**: User-facing documentation
- **REVAMPING.md**: Root → PRISM migration specification

### Framework Library (45 Frameworks)

Located in `.claude/product-foundation/`, organized by prefix:

**Discovery & Research** (6 frameworks):
- DISCOVERY-jobs-to-be-done.md
- DISCOVERY-persona-development.md
- DISCOVERY-value-proposition-canvas.md
- DISCOVERY-opportunity-solution-tree.md
- DISCOVERY-double-diamond.md
- DISCOVERY-design-thinking-lean-startup.md

**Prioritization** (3 frameworks):
- PRIORITIZATION-rice-prioritization.md
- PRIORITIZATION-ice-scoring.md
- PRIORITIZATION-moscow-prioritization.md

**Validation** (2 frameworks):
- VALIDATION-product-market-fit.md
- VALIDATION-kano-model.md

**Analysis** (4 frameworks):
- ANALYSIS-market-sizing-tam-sam-som.md
- ANALYSIS-cost-benefit-analysis-roi.md
- ANALYSIS-mece-framework.md
- ANALYSIS-balanced-tradeoff-matrix.md

**Strategy** (3 frameworks):
- STRATEGY-product-roadmapping.md
- STRATEGY-swot-analysis.md
- STRATEGY-product-led-growth.md

**Documentation** (2 frameworks):
- DOCUMENTATION-prd-template.md
- DOCUMENTATION-user-story-mapping.md

**Execution** (1 framework):
- EXECUTION-okrs.md

**Launch** (1 framework):
- LAUNCH-go-to-market-strategy.md

**Optimization** (1 framework):
- OPTIMIZATION-ab-testing-experimentation.md

**Metrics** (6 frameworks):
- METRICS-product-metrics.md
- METRICS-north-star-framework.md
- METRICS-aarrr-pirate-metrics.md
- METRICS-retention-churn-analysis.md
- METRICS-cohort-analysis.md
- METRICS-feature-adoption.md

**Analytics** (1 framework):
- ANALYTICS-data-visualization-charts.md

**Psychology** (1 framework):
- PSYCHOLOGY-gamification-tactics.md

**People Management** (3 frameworks):
- PEOPLE-interviewing-framework.md
- PEOPLE-feedback-framework.md
- PEOPLE-one-on-one-framework.md

**Communication** (2 frameworks):
- COMMUNICATION-stakeholder-management.md
- COMMUNICATION-influence-without-authority.md

**FinTech Domain** (3 frameworks):
- FINTECH-financial-inclusion.md
- FINTECH-payment-systems.md
- FINTECH-business-models.md

**TravelTech Domain** (2 frameworks):
- TRAVELTECH-industry-overview.md
- TRAVELTECH-optimization-strategies.md

**UX/UI Domain** (3 frameworks):
- UXRESEARCH-methodologies.md
- UXDESIGN-process-framework.md
- UIOPTIMIZATION-strategies.md

**Reference** (2 frameworks):
- REFERENCE-pm-mindset-strategy-execution.md
- REFERENCE-additional-frameworks.md

All frameworks include:
- Bilingual content (English/Vietnamese)
- Real-world examples
- Common mistakes
- Keywords for further research (users research independently)
- Internal navigation comments (for Claude only)

---

## Data Storage System

### Directory Structure
```
data/
├── items/              # Categorized PM items
│   ├── ideas/          # Product ideas (IDEA-001.md)
│   ├── incidents/      # Production incidents (INC-001.md)
│   ├── initiatives/    # Strategic initiatives
│   ├── ops-requests/   # Operational requests
│   ├── csat/           # Customer satisfaction issues
│   ├── integrations/   # Third-party needs
│   ├── funnel/         # Conversion optimization
│   ├── tech-debt/      # Technical debt
│   ├── competitive/    # Competitive responses
│   ├── compliance/     # Regulatory requirements
│   ├── insights/       # Data-driven insights
│   ├── research/       # User research
│   └── platform/       # Infrastructure needs
├── prds/              # Product Requirements Documents
├── roadmaps/          # Roadmap files
├── metrics/           # Analytics dashboards
├── retrospectives/    # Retrospective records
└── scores/            # Prioritization scores
```

### File Format
All data files use YAML frontmatter:
```yaml
---
id: "ITEM-001"
type: "idea"
status: "new"
date_created: "yyyy-mm-dd"
priority: "medium"
tags: []
related_items: []
---
```

---

## Slash Commands

### Available Commands (11 total)

**Smart Assistant**:
- `/assist [description]` - AI-powered framework navigator that reads frameworks silently and provides synthesized guidance

**Scenario-Specific**:
- `/scenario:interview` - PM interview preparation
- `/scenario:launch` - Product launch & GTM planning
- `/scenario:churn` - Churn analysis & retention
- `/scenario:prioritize` - Feature prioritization
- `/scenario:feedback` - Giving/receiving feedback
- `/scenario:pmf` - Product-Market Fit validation
- `/scenario:chart` - Data visualization guidance

**Git Helpers**:
- `/gh:commit` - Analyze changes and create commit
- `/gh:init` - Initialize git repository

**Help & Guidance**:
- `/prism-help` - First-time user guide with real-world examples

### Command Behavior

All slash commands MUST:
1. **Check conversation tracking first** (`PRISM-CONVOS/00-CONVO-LOGS.md`)
2. **Read frameworks silently** (from `.claude/product-foundation/`)
3. **Synthesize content** (never tell users to read files)
4. **Provide keywords** (for user self-research)
5. **Give actionable steps** (extracted from frameworks)

---

## Working with Frameworks

### Framework Selection Guide

Use `COMPETENCY-MAP.md` and `SCENARIO-INDEX.md` to route user needs:

**Common Scenarios**:
- "I need to prioritize features" → Read PRIORITIZATION-rice-prioritization.md, synthesize RICE methodology
- "I'm launching a product" → Read LAUNCH-go-to-market-strategy.md, provide GTM checklist
- "I don't know if we have PMF" → Read VALIDATION-product-market-fit.md, explain Sean Ellis test
- "Users are churning" → Read METRICS-retention-churn-analysis.md, provide cohort analysis steps
- "I'm interviewing someone" → Read PEOPLE-interviewing-framework.md, share question templates
- "I need to influence stakeholders" → Read COMMUNICATION-stakeholder-management.md, give influence tactics
- "Rural market access" → Read FINTECH-financial-inclusion.md, explain barriers & solutions
- "Travel booking optimization" → Read TRAVELTECH-optimization-strategies.md, share conversion tactics

### Framework Response Pattern

When helping users:
1. **Read the framework silently** (they don't see this)
2. **Understand their scenario** (restate their goal)
3. **Synthesize the framework** (extract core methodology)
4. **Provide actionable steps** (specific to their situation)
5. **Share keywords** (for deeper self-research)
6. **Give pro tips** (common mistakes from framework)

**Example Template**:
```markdown
## 🎯 I Understand Your Scenario
[Restate what they're trying to accomplish]

## 📚 Framework Approach: [Name]
**Core methodology**: [Steps/formulas/models from framework]
**How to apply it**: [Specific guidance]
**Key concepts**: [2-3 principles]
**Common pitfalls**: [What to avoid]

## ⚡ Quick Action Plan
- [ ] [Specific action from framework]
- [ ] [Follow-up action]
- [ ] [Validation step]

**Time estimate**: [How long]

## 🎓 Key Takeaway
[One sentence insight]

## 💡 Pro Tips
[2-3 practical tips from framework]

## 🔍 Keywords for Further Research
- [Keyword 1]
- [Keyword 2]
- [Keyword 3]
```

---

## Development Workflows

### Common Tasks

**No build/test commands** - This is a PM knowledge repository, not a code project.

**Key workflows**:
1. **Using slash commands** - Users invoke `/assist` or `/scenario:*` for PM guidance
2. **Managing conversations** - Always check `PRISM-CONVOS/00-CONVO-LOGS.md` first
3. **Updating frameworks** - Add new frameworks to `.claude/product-foundation/` with bilingual content
4. **Creating slash commands** - Add new `.md` files in `.claude/commands/` following existing patterns

### File Naming Conventions

- **Slash commands**: Use hyphens, organize in folders (`/scenario:feedback` → `.claude/commands/scenario/feedback.md`)
- **Frameworks**: Use PREFIX-name.md pattern (`DISCOVERY-jobs-to-be-done.md`)
- **Conversations**: Use yyyy-mm-dd-topic-keywords.md pattern
- **Data files**: Use PREFIX-NNN.md pattern (`IDEA-001.md`, `INC-042.md`)

---

## Important Context

### Project Identity
**Name**: PRISM (Lăng kính)
**Concept**: Breaking complex PM problems into understandable components (like a prism with light)
**Version**: PRISM v1.0
**Previous names**: Root v2.1 (multi-platform), Productify (original)

### Project Philosophy
- **Capability over complexity**: Frameworks are tools, not rules
- **Synthesis over signposting**: Provide answers, not file paths
- **Keywords over links**: Enable self-research, don't hand-hold
- **Context continuity**: Track conversations to maintain coherence

### Version History
- **Productify** (original): Workflow-based PM assistant
- **Root v2.0**: Multi-platform capability toolkit (5 AI platforms)
- **PRISM v1.0**: Claude-only, production-ready, synthesis-focused

### What Changed in PRISM v1.0
1. ✅ Single platform (Claude Code only)
2. ✅ Hidden frameworks (`.claude/product-foundation/`)
3. ✅ Synthesis approach (Claude reads, users get insights)
4. ✅ Keyword-based research (users Google independently)
5. ✅ Streamlined structure (removed multi-platform overhead)
6. ✅ Production ready (no development artifacts)

---

## Quality Standards

### Code Quality
- Validate all file paths before operations
- Use evidence-based claims (never assume completion)
- Cross-reference documentation for consistency
- Maintain bilingual content where applicable

### Documentation Quality
- Keep RULES.md and README.md synchronized
- Update conversation logs with all interactions
- Maintain accurate progress tracking
- Document all framework additions

### Framework Synthesis Quality
- ✅ Read frameworks completely before responding
- ✅ Extract actionable steps, not just theory
- ✅ Provide real examples from frameworks
- ✅ Share common mistakes from frameworks
- ✅ Give 5-7 research keywords
- ❌ Never say "read this file"
- ❌ Never show file paths to users
- ❌ Never recommend browsing `.claude/product-foundation/`

---

## Getting Help

### When in Doubt
1. Check conversation history in `PRISM-CONVOS/`
2. Reference `RULES.md` for protocols
3. Read relevant frameworks in `.claude/product-foundation/`
4. Synthesize and provide direct guidance

### For Framework Navigation
1. Check `COMPETENCY-MAP.md` for scenario mapping
2. Check `SCENARIO-INDEX.md` for keyword routing
3. Read matched frameworks silently
4. Provide synthesized guidance with keywords

---

**Remember**: PRISM is about capability, not complexity. Frameworks are YOUR reference library - users get synthesized insights and research keywords, never file paths. Always maintain conversation continuity through `PRISM-CONVOS/`.
