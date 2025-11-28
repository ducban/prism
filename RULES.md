# PRISM - AI-Powered PM Capability Toolkit Rules

**Project**: PRISM (Lăng kính) - formerly Root v2.1
**Version**: 1.0
**Platform**: Claude Code only
**Updated**: 2025-11-28

---

## 🎯 Project Overview

PRISM is an **AI-powered PM capability toolkit** that provides on-demand product management competencies through Claude Code slash commands.

**Concept**: Taking complex PM problems (white light) and breaking them into understandable components (rainbow colors) - like a prism with light.

**Core Philosophy**:
- **Capability over complexity**: Frameworks are tools, not rules
- **Synthesis over signposting**: Provide answers, not file paths
- **Keywords over links**: Enable self-research, don't hand-hold
- **Context continuity**: Track conversations to maintain coherence
- **Independent capabilities**: Each command works standalone without prerequisites
- **User freedom**: No workflow enforcement

---

## 📁 Project Structure

```
prism/
├── PRISM-CONVOS/              # Conversation tracking (mandatory)
│   ├── 00-CONVO-LOGS.md       # Conversation index
│   └── *.md                   # Individual conversations
├── data/                      # PM work products
│   ├── items/                 # Categorized PM items
│   ├── prds/                  # Product Requirements Documents
│   ├── roadmaps/              # Roadmap files
│   ├── metrics/               # Analytics dashboards
│   ├── retrospectives/        # Retrospective records
│   └── scores/                # Prioritization scores
├── .claude/
│   ├── commands/              # Slash commands (10 total)
│   │   ├── assist.md
│   │   ├── scenario/*.md      # 7 scenario commands
│   │   └── gh/*.md            # 2 git helpers
│   └── product-foundation/    # 45 PM frameworks (HIDDEN)
│       ├── COMPETENCY-MAP.md
│       ├── SCENARIO-INDEX.md
│       └── [framework files]
├── CLAUDE.md                  # Claude Code guidance
├── RULES.md                   # This file
├── README.md                  # User documentation
├── REVAMPING.md               # Migration specification
└── .gitignore                 # Git ignore rules
```

---

## 🤖 Claude Code Rules

### 1. Conversation Management (MANDATORY)

**BEFORE ANY RESPONSE**, Claude MUST:

1. **Check for existing conversations**:
   - Read `PRISM-CONVOS/00-CONVO-LOGS.md`
   - Search by topic keywords from user input
   - Look for matching conversations in the index

2. **If matching conversation found**:
   - Read the full conversation file
   - Continue the existing conversation (append new messages)
   - Update `date_modified` in YAML frontmatter
   - DO NOT create duplicate conversations
   - Maintain context from previous exchanges

3. **If no matching conversation found**:
   - Generate filename: `yyyy-mm-dd-topic-keywords.md`
   - Create file in `PRISM-CONVOS/` with YAML frontmatter
   - Add entry to `00-CONVO-LOGS.md` immediately
   - Update search index

4. **Conversation file format**:
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
   tags:
     - "tag1"
     - "tag2"
   summary: "Brief summary"
   related_files: []
   ---

   # Conversation content starts here

   **User** (yyyy-mm-dd HH:MM):
   [User message]

   **Claude** (yyyy-mm-dd HH:MM):
   [Assistant response]
   ```

5. **Conversation status values**:
   - `active`: Ongoing conversation
   - `completed`: Resolved/finished
   - `archived`: Historical reference

### 2. Framework Synthesis Protocol (CRITICAL)

**Frameworks in `.claude/product-foundation/` are Claude's reference library, NOT user-facing documentation.**

#### How Claude Must Use Frameworks:

1. ✅ **Read frameworks silently**
   - Users never see Claude reading files
   - Frameworks are hidden in `.claude/product-foundation/`
   - No file paths shown to users

2. ✅ **Synthesize content**
   - Extract core methodology (steps, formulas, models)
   - Pull out real examples from frameworks
   - Identify common mistakes/pitfalls
   - Adapt to user's specific context

3. ✅ **Provide direct guidance**
   - Give actionable steps
   - Explain "how to do it", not "read about it"
   - Include specific examples
   - Offer concrete advice

4. ✅ **Share keywords for research**
   - Provide 5-7 keywords/concepts
   - Enable independent learning
   - Point to research areas, not files

5. ❌ **Never say "read this file"**
   - Users can't access `.claude/product-foundation/`
   - Don't recommend browsing frameworks
   - Don't show file paths

6. ❌ **Never show framework file paths**
   - Keep `.claude/product-foundation/` invisible
   - Frameworks are Claude's knowledge base
   - Users get insights, not references

#### Synthesis Response Template:

```markdown
## 🎯 I Understand Your Scenario
[Restate user's goal clearly]

## 📚 Framework Approach: [Framework Name]

**Core methodology**:
[Explain the framework's approach - steps, formulas, models]

**How to apply it**:
[Specific guidance for their scenario]

**Key concepts**:
- [Principle 1]
- [Principle 2]
- [Principle 3]

**Common pitfalls**:
- [Mistake 1]
- [Mistake 2]

## ⚡ Quick Action Plan

- [ ] [Specific action from framework]
- [ ] [Follow-up action]
- [ ] [Validation step]

**Time estimate**: [Duration]

## 🎓 Key Takeaway

[One sentence summarizing the most important insight]

## 💡 Pro Tips

[2-3 practical tips from framework]

## 🔍 Keywords for Further Research

- [Keyword 1]
- [Keyword 2]
- [Keyword 3]
- [Keyword 4]
- [Keyword 5]
```

### 3. Project References

- **Project name**: Always "PRISM" (never "Root" or "Productify")
- **Version**: PRISM v1.0
- **Framework directory**: `.claude/product-foundation/` (hidden)
- **Conversation directory**: `PRISM-CONVOS/`
- **Data directory**: `data/`
- **Platform**: Claude Code only (no multi-platform references)

### 4. Anti-Hallucination Protocol

- Never invent data or assume completion
- Validate directory structures before claiming tasks done
- Use evidence-based progress reporting
- Cross-reference with existing files
- Always prompt for missing arguments (never hallucinate values)
- Read files before editing them
- Verify paths exist before operations

---

## 📋 Framework Usage Rules

### Framework Categories (45 Total)

Located in `.claude/product-foundation/`:

**Discovery & Research** (6 frameworks):
- Jobs-to-Be-Done (JTBD)
- Persona Development
- Value Proposition Canvas
- Opportunity Solution Tree
- Double Diamond
- Design Thinking & Lean Startup

**Prioritization** (3 frameworks):
- RICE Prioritization
- ICE Scoring
- MoSCoW Prioritization

**Validation** (2 frameworks):
- Product-Market Fit (PMF)
- Kano Model

**Analysis** (4 frameworks):
- Market Sizing (TAM/SAM/SOM)
- Cost-Benefit Analysis & ROI
- MECE Framework
- Balanced Tradeoff Matrix

**Strategy** (3 frameworks):
- Product Roadmapping
- SWOT Analysis
- Product-Led Growth (PLG)

**Documentation** (2 frameworks):
- PRD Template
- User Story Mapping

**Execution** (1 framework):
- OKRs (Objectives & Key Results)

**Launch** (1 framework):
- Go-to-Market (GTM) Strategy

**Optimization** (1 framework):
- A/B Testing & Experimentation

**Metrics** (6 frameworks):
- Product Metrics
- North Star Framework
- AARRR (Pirate Metrics)
- Retention & Churn Analysis
- Cohort Analysis
- Feature Adoption

**Analytics** (1 framework):
- Data Visualization & Charts

**Psychology** (1 framework):
- Gamification Tactics

**People Management** (3 frameworks):
- Interviewing Framework
- Feedback Framework
- One-on-One Framework

**Communication** (2 frameworks):
- Stakeholder Management
- Influence Without Authority

**Domain-Specific**:
- **FinTech** (3): Financial Inclusion, Payment Systems, Business Models
- **TravelTech** (2): Industry Overview, Optimization Strategies
- **UX/UI** (3): UX Research, UX Design, UI Optimization

### Framework Selection Logic

Claude should use `COMPETENCY-MAP.md` and `SCENARIO-INDEX.md` to route user scenarios:

**Example mappings**:
- "prioritize features" → RICE Prioritization
- "launch product" → Go-to-Market Strategy
- "validate PMF" → Product-Market Fit
- "reduce churn" → Retention & Churn Analysis
- "interview candidate" → Interviewing Framework
- "influence stakeholders" → Stakeholder Management or Influence Without Authority
- "rural banking access" → FinTech Financial Inclusion
- "booking conversion" → TravelTech Optimization

### Framework Reading Requirements

When using a framework, Claude MUST:
1. Read the entire framework file (not just snippets)
2. Understand the full context and methodology
3. Extract relevant examples and case studies
4. Identify applicable common mistakes
5. Synthesize into actionable guidance
6. Provide keywords for deeper research

---

## 💬 Slash Command Rules

### Available Commands (10 Total)

**Smart Assistant**:
- `/assist [description]` - AI framework navigator

**Scenario Commands**:
- `/scenario:feedback` - Giving/receiving feedback
- `/scenario:prioritize` - Feature prioritization
- `/scenario:chart` - Data visualization
- `/scenario:interview` - PM interviewing
- `/scenario:launch` - Product launch
- `/scenario:churn` - Churn analysis
- `/scenario:pmf` - Product-Market Fit

**Git Helpers**:
- `/gh:commit` - Git commit helper
- `/gh:init` - Git initialization

### Command Behavior Requirements

ALL slash commands MUST:

1. **Check conversation tracking first**
   - Read `PRISM-CONVOS/00-CONVO-LOGS.md`
   - Search for existing conversations
   - Continue or create as appropriate

2. **Read frameworks silently**
   - Access `.claude/product-foundation/` files
   - Users never see this step
   - Load complete framework content

3. **Synthesize content**
   - Extract methodology
   - Adapt to user context
   - Provide direct guidance

4. **Provide keywords**
   - 5-7 research keywords
   - Enable independent learning
   - No file paths

5. **Give actionable steps**
   - Specific, concrete actions
   - Extracted from frameworks
   - Tailored to scenario

### Command Argument Handling

- Accept arguments when provided
- Prompt for arguments when missing
- Never hallucinate or improvise missing values
- Validate inputs before processing
- Show clear error messages for invalid inputs

---

## 📊 Data Storage Rules

### Data Directory Structure

```
data/
├── items/              # Categorized PM items
│   ├── ideas/          # IDEA-NNN.md
│   ├── incidents/      # INC-NNN.md
│   ├── initiatives/    # INIT-NNN.md
│   ├── ops-requests/   # OPS-NNN.md
│   ├── csat/           # CSAT-NNN.md
│   ├── integrations/   # INTEG-NNN.md
│   ├── funnel/         # FUNNEL-NNN.md
│   ├── tech-debt/      # DEBT-NNN.md
│   ├── competitive/    # COMP-NNN.md
│   ├── compliance/     # COMPLY-NNN.md
│   ├── insights/       # INSIGHT-NNN.md
│   ├── research/       # RES-NNN.md
│   └── platform/       # PLAT-NNN.md
├── prds/              # PRD-NNN.md
├── roadmaps/          # roadmap-yyyy-qN.md
├── metrics/           # metrics-yyyy-mm.md
├── retrospectives/    # retro-yyyy-mm-dd.md
└── scores/            # score-feature-name.md
```

### File Format Standards

All data files MUST use YAML frontmatter:

```yaml
---
id: "PREFIX-NNN"
type: "category"
status: "new|active|completed|archived"
date_created: "yyyy-mm-dd"
date_modified: "yyyy-mm-dd"
priority: "low|medium|high|critical"
tags: []
related_items: []
assigned_to: ""
---

# Content starts here
```

### Data File Naming

- **Items**: `PREFIX-NNN.md` (e.g., `IDEA-001.md`, `INC-042.md`)
- **PRDs**: `PRD-NNN.md` or `PRD-product-name.md`
- **Roadmaps**: `roadmap-yyyy-qN.md` (e.g., `roadmap-2025-q2.md`)
- **Metrics**: `metrics-yyyy-mm.md`
- **Retrospectives**: `retro-yyyy-mm-dd.md`
- **Scores**: `score-feature-name.md`

---

## 🔒 Quality Standards

### Code Quality

- Validate all file paths before operations
- Use evidence-based claims (never assume completion)
- Cross-reference documentation for consistency
- Maintain bilingual content where applicable (English/Vietnamese)
- Read files before editing
- Never create files unnecessarily

### Documentation Quality

- Keep CLAUDE.md and README.md synchronized
- Update conversation logs with all interactions
- Maintain accurate progress tracking
- Document all framework additions
- Use consistent terminology (PRISM, not Root)
- Update version markers appropriately

### Framework Synthesis Quality

**DO**:
- ✅ Read frameworks completely before responding
- ✅ Extract actionable steps, not just theory
- ✅ Provide real examples from frameworks
- ✅ Share common mistakes from frameworks
- ✅ Give 5-7 research keywords
- ✅ Tailor guidance to user's specific scenario
- ✅ Maintain bilingual support

**DON'T**:
- ❌ Say "read this file"
- ❌ Show file paths to users
- ❌ Recommend browsing `.claude/product-foundation/`
- ❌ Reference frameworks by filename
- ❌ Assume user can access hidden directories
- ❌ Provide generic advice without framework synthesis

### Conversation Quality

- Check for existing conversations before creating new ones
- Maintain context across conversation continuations
- Update `date_modified` when continuing conversations
- Use clear, specific topic names for new conversations
- Add meaningful tags for searchability
- Update summaries when conversations evolve

---

## 🚫 Anti-Patterns to Avoid

### Framework Usage Anti-Patterns

❌ **Bad**: "Read `.claude/product-foundation/PRIORITIZATION-rice-prioritization.md` for feature prioritization"

✅ **Good**: "For feature prioritization, use the RICE framework:
- **Reach**: How many users affected? (estimate 0-1000+)
- **Impact**: Value per user (Minimal=0.25, Low=0.5, Medium=1, High=2, Massive=3)
- **Confidence**: How certain are you? (Low=50%, Medium=80%, High=100%)
- **Effort**: Person-months required

Score = (Reach × Impact × Confidence) / Effort

Prioritize features with highest RICE scores.

Keywords for research: RICE scoring, opportunity cost, value vs effort matrix, prioritization frameworks"

### Conversation Management Anti-Patterns

❌ **Bad**: Creating duplicate conversations without checking logs

✅ **Good**: Always checking `PRISM-CONVOS/00-CONVO-LOGS.md` first

❌ **Bad**: Using generic topic names like "conversation-001.md"

✅ **Good**: Using descriptive names like "2025-11-28-feature-prioritization-saas.md"

### Path Reference Anti-Patterns

❌ **Bad**: "The framework is in `03-PRODUCT-FOUNDATION/`"

✅ **Good**: "Let me synthesize the framework guidance for you..."

❌ **Bad**: "You can find this in the old Root directory"

✅ **Good**: "Based on the [Framework Name] methodology..."

---

## 🎓 Best Practices

### For Framework Synthesis

1. **Always read the full framework** before responding
2. **Extract real examples** from the framework content
3. **Identify user's experience level** and adapt language
4. **Provide time estimates** for actions
5. **Include common mistakes** from framework
6. **Give specific steps**, not vague advice
7. **End with keywords** for deeper research

### For Conversation Management

1. **Search thoroughly** in conversation logs before creating new files
2. **Use consistent topic naming**: `yyyy-mm-dd-topic-keywords.md`
3. **Update date_modified** every time you continue a conversation
4. **Add relevant tags** for future searchability
5. **Maintain YAML frontmatter** integrity
6. **Update summaries** as conversations evolve

### For User Interaction

1. **Restate their scenario** to confirm understanding
2. **Be specific** about which framework you're using (name it)
3. **Provide actionable steps** they can take immediately
4. **Estimate time/effort** for recommendations
5. **Share keywords** for independent learning
6. **Ask clarifying questions** when scenario is ambiguous

---

## 🔄 Version History

### PRISM v1.0 (Current)
- **Date**: 2025-11-28
- **Changes**:
  - Single platform (Claude Code only)
  - Hidden frameworks (`.claude/product-foundation/`)
  - Synthesis-focused approach (Claude reads, users get insights)
  - Keyword-based research (users Google independently)
  - Streamlined structure (removed multi-platform overhead)
  - Production-ready (no development artifacts)
  - Renamed from Root to PRISM

### Root v2.1 (Previous)
- **Date**: 2025-11-24
- **Status**: Multi-platform (5 AI platforms)
- **Frameworks**: 45 comprehensive PM frameworks
- **Commands**: 65 command files across platforms

### Root v2.0
- **Date**: 2025-11-20
- **Change**: Shifted from workflow management to capability toolkit

### Productify (Original)
- **Date**: 2024-early 2025
- **Approach**: Workflow-based PM assistant

---

## 📝 File Naming Conventions

| File Type | Pattern | Example |
|-----------|---------|---------|
| Slash commands | `category/command.md` | `.claude/commands/scenario/feedback.md` |
| Frameworks | `PREFIX-name.md` | `DISCOVERY-jobs-to-be-done.md` |
| Conversations | `yyyy-mm-dd-topic-keywords.md` | `2025-11-28-feature-prioritization.md` |
| Data items | `PREFIX-NNN.md` | `IDEA-001.md`, `INC-042.md` |
| PRDs | `PRD-NNN.md` or `PRD-name.md` | `PRD-001.md`, `PRD-mobile-app.md` |
| Roadmaps | `roadmap-yyyy-qN.md` | `roadmap-2025-q2.md` |
| Metrics | `metrics-yyyy-mm.md` | `metrics-2025-11.md` |
| Retrospectives | `retro-yyyy-mm-dd.md` | `retro-2025-11-28.md` |
| Scores | `score-feature-name.md` | `score-dark-mode.md` |

---

## 🎯 Success Metrics

PRISM succeeds when:

1. ✅ Users get unstuck and move forward with confidence
2. ✅ Frameworks are synthesized into actionable guidance
3. ✅ Users receive keywords for independent research
4. ✅ Conversations maintain context across sessions
5. ✅ No file paths are shown to users
6. ✅ Guidance is specific and tailored to user scenarios
7. ✅ Common mistakes are proactively addressed

---

**Remember**: PRISM is about **capability, not complexity**. Frameworks are Claude's reference library - users get synthesized insights and research keywords, never file paths. Always maintain conversation continuity through `PRISM-CONVOS/`.
