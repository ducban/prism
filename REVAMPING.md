# PRISM v1.0 - Revamping Requirements

**Date**: 2025-11-27
**Status**: Planning Phase
**Target**: Minimize Root for Claude-only, production-ready PRISM

---

## Project Identity

### Name Change: Root → PRISM
**Vietnamese**: Lăng kính
**Concept**: Lấy một vấn đề phức tạp (ánh sáng trắng) và phân tách nó thành các thành phần dễ hiểu (các màu sắc của cầu vồng).

**Meaning**: Taking complex problems (white light) and breaking them into understandable components (rainbow colors).

### Version
- **Current**: Root v2.1 (multi-platform)
- **Target**: PRISM v1.0 (Claude-only, production)

---

## Structural Changes

### Directory Removals

**Delete entirely**:
```
00-BACKLOGS/              # Historical development logs
01-HUMAN-DOCS/            # Development-phase documentation
02-AI-DOCS/               # Multi-platform AI guidelines
.gemini/                  # Gemini CLI support
.opencode/                # OpenCode support
.iflow/                   # iFlow support
.factory/                 # Factory Droid support
```

**Delete specific files**:
```
SPECIALIZED-AGENT-GUIDELINE.md    # Multi-platform dev doc
SLASH-COMMAND-GUIDELINE.md        # Multi-platform dev doc
SMART-COMMANDS-README.md          # Development reference
IFLOW.md                          # Platform-specific
GEMINI.md                         # Platform-specific (if exists)
*init.sh scripts                  # Development setup scripts
```

**Delete slash command folders**:
```
.claude/commands/seed/            # Development tools only
.claude/commands/project/         # Development/maintenance tools only
```

### Directory Renames

```
04-ROOT-CONVOS/  →  PRISM-CONVOS/
```

### Directory Moves

```
03-PRODUCT-FOUNDATION/  →  .claude/product-foundation/
```

### Final Structure

```
prism/
├── PRISM-CONVOS/
│   ├── 00-CONVO-LOGS.md
│   └── [conversation-files].md
├── data/
│   ├── items/
│   ├── prds/
│   ├── roadmaps/
│   ├── metrics/
│   ├── retrospectives/
│   └── scores/
├── .claude/
│   ├── commands/
│   │   ├── assist.md
│   │   ├── scenario/
│   │   │   ├── feedback.md
│   │   │   ├── prioritize.md
│   │   │   ├── chart.md
│   │   │   ├── interview.md
│   │   │   ├── launch.md
│   │   │   ├── churn.md
│   │   │   └── pmf.md
│   │   └── gh/
│   │       ├── commit.md
│   │       └── init.md
│   └── product-foundation/          # 45 frameworks (HIDDEN)
│       ├── COMPETENCY-MAP.md
│       ├── SCENARIO-INDEX.md
│       ├── DISCOVERY-*.md
│       ├── PRIORITIZATION-*.md
│       ├── VALIDATION-*.md
│       ├── ANALYSIS-*.md
│       ├── STRATEGY-*.md
│       ├── DOCUMENTATION-*.md
│       ├── EXECUTION-*.md
│       ├── LAUNCH-*.md
│       ├── OPTIMIZATION-*.md
│       ├── METRICS-*.md
│       ├── ANALYTICS-*.md
│       ├── PSYCHOLOGY-*.md
│       ├── PEOPLE-*.md
│       ├── COMMUNICATION-*.md
│       ├── FINTECH-*.md
│       ├── TRAVELTECH-*.md
│       ├── UXDESIGN-*.md
│       ├── UXRESEARCH-*.md
│       ├── UIOPTIMIZATION-*.md
│       └── REFERENCE-*.md
├── .gitignore                       # UPDATE REQUIRED
├── CLAUDE.md                        # MAJOR REWRITE
├── RULES.md                         # MAJOR REWRITE
└── README.md                        # MAJOR REWRITE
```

---

## Core Functionality

### User Experience
1. User invokes Claude slash commands via CLI
2. Claude reads hidden frameworks from `.claude/product-foundation/`
3. Claude **synthesizes** guidance and provides keywords/concepts directly
4. Conversations logged to `PRISM-CONVOS/` with existing YAML rules
5. User never sees framework file paths

### Framework Usage Philosophy Change

**OLD APPROACH** (Root v2.x):
```
User: "How do I prioritize features?"
Claude: "Read 03-PRODUCT-FOUNDATION/PRIORITIZATION-rice-prioritization.md"
```

**NEW APPROACH** (PRISM v1.0):
```
User: "How do I prioritize features?"
Claude: [Reads .claude/product-foundation/PRIORITIZATION-rice-prioritization.md internally]
Claude: "For feature prioritization, use the RICE framework:
         - Reach: How many users affected?
         - Impact: How much value per user?
         - Confidence: How certain are you?
         - Effort: How much work required?

         Keywords for research: RICE scoring, feature prioritization matrix,
         opportunity cost, value vs effort..."
```

**Key principle**: Frameworks are Claude's reference library, NOT user-facing documentation.

---

## Mass Update Requirements

### 1. Path Updates in All Files (~70+ files)

**Old paths** → **New paths**:
```
03-PRODUCT-FOUNDATION/              →  .claude/product-foundation/
04-ROOT-CONVOS/                     →  PRISM-CONVOS/
00-BACKLOGS/                        →  [DELETE]
02-AI-DOCS/                         →  [DELETE]
01-HUMAN-DOCS/                      →  [DELETE]
```

**Files requiring updates**:
- All slash commands in `.claude/commands/` (~10-12 files)
- `PRISM-CONVOS/00-CONVO-LOGS.md`
- Framework cross-references (45 framework files)
- `CLAUDE.md`
- `RULES.md`
- `README.md`

### 2. Slash Command Behavior Changes

**Remove these patterns**:
```markdown
❌ "Read the framework at 03-PRODUCT-FOUNDATION/[file].md"
❌ "I recommend reading DISCOVERY-jobs-to-be-done.md"
❌ "Check out the full guide in the framework directory"
```

**Add these patterns**:
```markdown
✅ [Claude reads framework file silently]
✅ "For this scenario, use [Framework Name]: [synthesized guidance]"
✅ "Key concepts to research: [keywords extracted from framework]"
✅ "Here's a step-by-step approach: [actionable steps from framework]"
```

### 3. Conversation Tracking Updates

All slash commands must update conversation tracking paths:

**OLD**:
```markdown
1. Check `04-ROOT-CONVOS/00-CONVO-LOGS.md` for existing conversations
```

**NEW**:
```markdown
1. Check `PRISM-CONVOS/00-CONVO-LOGS.md` for existing conversations
```

### 4. Remove Multi-Platform References

Delete all mentions of:
- Gemini CLI
- OpenCode
- iFlow
- Factory Droid
- Cross-platform compatibility
- Platform-specific syntax tables
- Multi-platform command formats

---

## Documentation Rewrites

### CLAUDE.md

**Major changes**:
1. Remove entire "Project Structure" section for deleted folders
2. Update all directory references
3. Remove multi-platform slash command table
4. Update "Framework Library" section to reflect hidden location
5. Remove "Platform-Specific Syntax" section
6. Simplify "Slash Commands" section (Claude-only)
7. Update conversation tracking paths
8. Remove references to other platform .md files
9. Update project name throughout (Root → PRISM)
10. Add framework usage philosophy (synthesis, not file paths)

### RULES.md

**Major changes**:
1. Single platform focus (Claude Code only)
2. Update conversation tracking paths (PRISM-CONVOS)
3. Remove multi-platform requirements
4. Update framework directory paths
5. Simplify slash command creation rules (no cross-platform)
6. Update project name and version (PRISM v1.0)
7. Add "Framework Synthesis Protocol" section
8. Remove development-phase rules
9. Update all file structure references

### README.md

**Complete rewrite**:
1. PRISM branding and concept explanation
2. Claude-only installation
3. Simplified quick start (no platform selection)
4. Updated directory structure
5. Framework usage examples (synthesis approach)
6. Slash command reference (Claude-only)
7. Version: PRISM v1.0
8. Remove multi-platform comparison tables
9. Simplified architecture diagram
10. Production-ready tone (no development instructions)

### .gitignore

**Updates needed**:
1. Remove references to deleted platform folders
2. Add `.claude/product-foundation/` (if needed for IDE)
3. Update any 00-BACKLOGS, 01-HUMAN-DOCS, 02-AI-DOCS patterns
4. Ensure PRISM-CONVOS/ privacy rules
5. Review data/ ignore patterns

---

## Remaining Slash Commands (After Cleanup)

### Core Commands
```
.claude/commands/
├── assist.md                    # AI framework navigator
├── scenario/
│   ├── feedback.md             # Feedback framework
│   ├── prioritize.md           # Feature prioritization
│   ├── chart.md                # Data visualization
│   ├── interview.md            # PM interviews
│   ├── launch.md               # Product launch & GTM
│   ├── churn.md                # Churn analysis
│   └── pmf.md                  # Product-market fit
└── gh/
    ├── commit.md               # Git commit helper
    └── init.md                 # Git init helper
```

**Total**: ~10 command files (down from 65 across 5 platforms)

**Removed folders**:
- `/seed:*` commands (development tools)
- `/project:*` commands (maintenance tools)

---

## Framework Synthesis Protocol

### How Claude Should Use Frameworks

**Step 1: Silent Framework Reading**
- Claude reads relevant `.claude/product-foundation/[framework].md`
- User doesn't see this happening
- No file paths mentioned to user

**Step 2: Content Synthesis**
- Extract core concepts, steps, formulas
- Adapt to user's specific context
- Provide actionable guidance

**Step 3: Knowledge Transfer**
- Give direct answers with framework methodology
- Provide research keywords for deeper learning
- Include real-world examples from framework
- Mention common pitfalls

**Step 4: No File References**
- Never say "read this file"
- Never show framework file paths
- Keep `.claude/product-foundation/` invisible to user

### Example Pattern

**User Query**: "How do I validate product-market fit?"

**Claude Process** (invisible):
1. Read `.claude/product-foundation/VALIDATION-product-market-fit.md`
2. Read `.claude/product-foundation/METRICS-north-star-framework.md`
3. Extract 5 PMF validation methods
4. Identify key metrics and thresholds

**Claude Response** (visible):
```
To validate product-market fit, use these signals:

1. Retention Cohorts
   - 40%+ of new users return in Week 2
   - Retention curve flattens after 4-6 weeks

2. Organic Growth Rate
   - 5-7% weekly growth without paid marketing
   - NPS score above 50

3. Value Metric Progression
   - Users hitting "aha moment" within 7 days
   - Core action completion rate >60%

Keywords for deeper research: PMF validation metrics, retention curve analysis,
Sean Ellis test, value hypothesis testing, leading vs lagging indicators

Common mistakes:
- Confusing early adopter love with true PMF
- Over-relying on vanity metrics (signups, downloads)
- Not segmenting by user type
```

---

## Data Folder Retention

**Why keep `data/`**:
- Provides structured storage for PM work products
- Ready-to-use categorization system (13 item types)
- Enables conversation context persistence
- Supports slash command workflows (creating PRDs, roadmaps, etc.)
- YAML frontmatter consistency across all data files

**Usage**:
- Slash commands can create items in `data/items/[category]/`
- Conversations reference and update data files
- Users organize PM artifacts systematically

---

## Version & Status Updates

### Throughout Codebase

**Find and replace**:
```
"Root" → "PRISM"
"Root v2.1" → "PRISM v1.0"
"Productify" → "PRISM" (if any stragglers remain)
"94% complete" → "Production ready"
"v2.0 philosophy" → "v1.0 philosophy"
```

**Status markers**:
```
Development → Production
Beta → Stable
Multi-platform → Claude-optimized
```

---

## Testing Checklist (Post-Migration)

### Functionality Tests
- [ ] `/assist` command works with hidden frameworks
- [ ] All `/scenario:*` commands provide synthesized guidance
- [ ] Conversation logging creates files in `PRISM-CONVOS/`
- [ ] Framework cross-references still work (internal to Claude)
- [ ] No broken file path references in responses
- [ ] Git commands (`/gh:commit`, `/gh:init`) still work

### Documentation Tests
- [ ] CLAUDE.md has no references to deleted folders/platforms
- [ ] RULES.md reflects PRISM v1.0 structure
- [ ] README.md provides clear Claude-only setup
- [ ] No references to Root, Gemini, OpenCode, iFlow, Factory
- [ ] All example paths use new structure

### Path Validation
- [ ] No references to `00-BACKLOGS/`
- [ ] No references to `01-HUMAN-DOCS/`
- [ ] No references to `02-AI-DOCS/`
- [ ] No references to `03-PRODUCT-FOUNDATION/` (use `.claude/product-foundation/`)
- [ ] No references to `04-ROOT-CONVOS/` (use `PRISM-CONVOS/`)
- [ ] `.gitignore` updated correctly

---

## Critical Success Factors

### Must-Haves
1. ✅ All 45 frameworks remain accessible (just hidden)
2. ✅ Conversation tracking continues to work
3. ✅ Zero broken references in slash commands
4. ✅ Users never see framework file paths
5. ✅ Claude synthesizes framework content directly
6. ✅ PRISM branding consistent throughout
7. ✅ `data/` folder structure intact
8. ✅ Git history preserved (if desired)

### Quality Gates
1. ✅ No multi-platform references remain
2. ✅ All documentation uses PRISM v1.0 naming
3. ✅ Slash commands work without exposing framework files
4. ✅ New users can onboard without reading framework docs
5. ✅ Project feels production-ready (no dev artifacts)

---

## Execution Phases

### Phase 1: Structural Changes
1. **Remove git history**: Delete `.git/` folder
2. Rename `04-ROOT-CONVOS/` → `PRISM-CONVOS/`
3. Move `03-PRODUCT-FOUNDATION/` → `.claude/product-foundation/`
4. Delete folders: `00-BACKLOGS/`, `01-HUMAN-DOCS/`, `02-AI-DOCS/`
5. Delete platform folders: `.gemini/`, `.opencode/`, `.iflow/`, `.factory/`
6. Delete development files: `SPECIALIZED-AGENT-GUIDELINE.md`, `SLASH-COMMAND-GUIDELINE.md`, `SMART-COMMANDS-README.md`, `IFLOW.md`, `*.sh` scripts
7. Delete slash commands: `.claude/commands/seed/`, `.claude/commands/project/`

### Phase 2: Mass Path Updates
1. Update all slash commands (10 files)
   - Change paths: `04-ROOT-CONVOS/` → `PRISM-CONVOS/`
   - Remove "read this file" patterns
   - Add framework synthesis approach
2. Update `PRISM-CONVOS/00-CONVO-LOGS.md`
   - Update header documentation
   - Change path references
3. Update framework cross-references (45 files)
   - Remove user-facing file path references
   - Replace with "Keywords for Research" sections
   - Add internal navigation comments for Claude
4. Update `.gitignore`
   - Remove references to deleted folders
   - Add PRISM-specific patterns

### Phase 3: Documentation Rewrites
1. Rewrite `CLAUDE.md` (major changes)
2. Rewrite `RULES.md` (major changes)
3. Rewrite `README.md` (complete overhaul)
4. Update version markers throughout

### Phase 4: Behavior Changes
1. Update slash commands to synthesize frameworks
2. Remove "read this file" patterns
3. Add keyword extraction logic
4. Add framework synthesis instructions

### Phase 5: Validation
1. Test all slash commands
2. Verify no broken references
3. Check conversation logging
4. Review documentation completeness
5. Validate .gitignore rules

### Phase 6: Git Initialization
1. Initialize new git repository: `git init`
2. Create initial `.gitignore`
3. Stage all files: `git add .`
4. First commit: `git commit -m "PRISM v1.0 initial release"`
5. (Optional) Add remote and push

---

## Notes & Considerations

### Hidden Framework Directory
- `.claude/product-foundation/` is hidden (dot-prefix)
- Users can't accidentally browse/edit frameworks
- Claude still has full access via tools
- Cleaner user-facing directory structure

### Data Folder Visibility
- `data/` remains visible (no dot-prefix)
- Users need to see/manage their PM work products
- Provides clear organizational structure

### Git History
**DECISION**: Fresh start
- Remove `.git` folder entirely
- Start new git repository for PRISM v1.0
- No migration of git history from Root
- Clean slate for production project

### Backup Considerations
**DECISION**: Already backed up externally
- Safe to permanently delete all folders/files
- No archive repo needed
- Proceed with deletions

---

## Confirmed Decisions (2025-11-27)

### 1. Git Strategy ✅
**Decision**: Remove `.git` folder, fresh git init for PRISM
- No git history migration
- New repository from scratch
- First commit will be "PRISM v1.0 initial release"

### 2. Archive Strategy ✅
**Decision**: User has external backup, safe to delete
- Permanently remove `00-BACKLOGS/`, `01-HUMAN-DOCS/`, `02-AI-DOCS/`
- Permanently remove `.gemini/`, `.opencode/`, `.iflow/`, `.factory/`
- No separate archive repo needed

### 3. Framework Cross-References ✅
**Decision**: Dual approach for internal vs external
- **Remove**: User-facing cross-references (e.g., "See also: [file].md")
- **Replace with**: Research keywords (e.g., "Related concepts: JTBD, persona development, value proposition")
- **Keep**: Internal Claude navigation comments (for framework relationships)

**Implementation**:
```markdown
❌ OLD: "For more details, read DISCOVERY-jobs-to-be-done.md"
✅ NEW: "Related concepts to research: Jobs-to-Be-Done framework, outcome-driven innovation, job stories"

✅ KEEP (internal): <!-- Related frameworks: DISCOVERY-jobs-to-be-done.md, DISCOVERY-persona-development.md -->
```

### 4. Framework File Updates
Each framework file needs:
1. Remove user-facing file path references
2. Add "Keywords for Research" section at end
3. Keep internal navigation comments for Claude
4. Maintain all content (concepts, examples, steps)

---

**End of REVAMPING.md**

This document serves as the master reference for the Root → PRISM v1.0 migration.
All execution should follow this specification.
