---
# Core Metadata
title: "Persona Development Framework"
title_vi: "Khung Phát Triển Persona"
framework_type: "Discovery"
category: ["Product Management", "Discovery", "Research", "User Experience"]

# Origin & Authority
author: "Alan Cooper"
organization: "Cooper Interaction Design"
year_developed: "1999"
original_source: "The Inmates Are Running the Asylum (Cooper, 1999)"

# Root Integration
root_phase: ["Phase 1: Research & Discover", "Phase 2: Collaborate & Align"]
root_commands: ["/phase1:personas", "/phase2:research"]
when_to_use: "When understanding target users, building empathy, or aligning team on who you're building for"

# Difficulty & Time
complexity: "Medium"
estimated_time: "2-4 weeks (research + synthesis)"
skill_level: "Beginner-Intermediate"

# Classification
tags: ["personas", "user-research", "discovery", "empathy", "segmentation", "ux"]
related_frameworks: ["Jobs to Be Done", "Value Proposition Canvas", "User Story Mapping", "Customer Journey Map"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-21"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Book"
    title: "The Inmates Are Running the Asylum"
    author: "Alan Cooper"
    year: "1999"
  - type: "Book"
    title: "The User Is Always Right: A Practical Guide to Creating and Using Personas"
    author: "Steve Mulder, Ziv Yaar"
    year: "2006"
  - type: "Article"
    title: "Personas Make Users Memorable for Product Team Members"
    url: "https://www.nngroup.com/articles/persona/"
    author: "Nielsen Norman Group"
    year: "2015"
---

# Persona Development Framework / Khung Phát Triển Persona

## Overview / Tổng Quan

**English:**
A persona is a fictional character that represents a key user segment of your product. It's a research-based archetype that brings your users to life.

**What a Persona Is:**
- Fictional but based on real data
- Represents a user segment (not an individual)
- Includes demographics, behaviors, goals, pain points
- Makes users memorable and relatable

**What a Persona Is NOT:**
- ❌ Made-up stereotype ("millennials like avocado toast")
- ❌ Marketing demographics only (age, income, location)
- ❌ Your assumptions about users
- ❌ One persona for everyone

**Why Personas Matter:**
1. **Empathy**: Team understands users deeply
2. **Alignment**: Everyone builds for same user
3. **Decisions**: "Would Sarah use this?" becomes decision filter
4. **Communication**: Easier to discuss users ("the busy parent")
5. **Prioritization**: Features for primary persona get priority

**Real Example - Mailchimp:**

**Before Personas (2008):**
- Team debated features based on assumptions
- "I think small businesses want..."
- Conflicting priorities

**After Personas (2009):**
Created 3 core personas:
1. **"Freddie"** - Solo entrepreneur (primary)
2. **"Melissa"** - Marketing manager at SMB
3. **"Warren"** - Agency managing multiple clients

**Impact:**
- Product decisions: "Is this for Freddie?" (primary persona)
- Simplified UI for Freddie (non-technical)
- Built agency features for Warren later
- Grew from 85K → 1M+ users in 2 years

**Vietnamese:**
Persona là nhân vật hư cấu đại diện cho phân khúc người dùng chính của sản phẩm.

**Persona Là:**
- Hư cấu nhưng dựa trên dữ liệu thực
- Đại diện phân khúc (không phải cá nhân)
- Bao gồm demographics, hành vi, mục tiêu, khó khăn

**Tại Sao Quan Trọng:**
1. Đồng cảm với người dùng
2. Liên kết đội nhóm
3. Quyết định dễ dàng
4. Giao tiếp hiệu quả
5. Ưu tiên tính năng

**Ví Dụ - Mailchimp:**
- Trước: Tranh luận dựa giả định
- Sau: 3 personas (Freddie, Melissa, Warren)
- Kết quả: 85K → 1M users trong 2 năm

---

## Persona Components / Thành Phần Persona

**English:**

### 1. Header (Quick Reference)
**Elements:**
- **Name**: Memorable, relatable (e.g., "Busy Beth", "Tech-Savvy Tom")
- **Photo**: Stock photo (represents persona, not actual user)
- **Tagline**: One-sentence descriptor
- **Demographic snapshot**: Age, occupation, location

**Example:**
```
═══════════════════════════════════════════
     📷 SARAH CHEN
     "The Multitasking Product Manager"
═══════════════════════════════════════════
Age: 32 | Location: San Francisco
Role: Product Manager at 100-person startup
Experience: 6 years in product
Tech Savvy: High
```

### 2. Background & Demographics
**Include:**
- Age range (not specific age)
- Education
- Job title & industry
- Company size (for B2B)
- Family situation (if relevant)
- Income range (if relevant)

**Example - Sarah:**
```
BACKGROUND:
• 32 years old, lives in San Francisco
• Stanford CS degree, pivoted from engineering to PM
• Works at Series B startup (100 employees)
• Reports to VP Product, manages 2 designers
• Married, no kids yet, active social life
• Income: $150K-$180K
```

### 3. Goals & Motivations
**What do they want to achieve?**

**Categories:**
- **Professional goals**: Career advancement, recognition
- **Personal goals**: Work-life balance, learning
- **Product-specific goals**: What they want from YOUR product

**Example - Sarah:**
```
GOALS:
Professional:
• Ship products that move key metrics
• Get promoted to Senior PM
• Build strong team culture

Personal:
• Learn data analysis skills
• Maintain work-life balance
• Stay on top of industry trends

With Our Product:
• Make faster, data-driven decisions
• Reduce time in meetings
• Collaborate seamlessly with engineering
```

### 4. Frustrations & Pain Points
**What problems do they face?**

**Categories:**
- **Current tools**: What's frustrating about alternatives?
- **Workflows**: What slows them down?
- **Gaps**: What's missing?

**Example - Sarah:**
```
FRUSTRATIONS:
• Juggles 12+ tools (Jira, Figma, Notion, Slack, etc.)
• Wastes 2 hours/day switching contexts
• Hard to get team aligned on priorities
• Analytics tools too complex for quick insights
• Difficult to communicate roadmap to stakeholders
• Always feels behind, reactive vs proactive
```

### 5. Behaviors & Patterns
**How do they work? What's their routine?**

**Include:**
- Daily routines
- Tool usage
- Information sources
- Decision-making process

**Example - Sarah:**
```
BEHAVIORS:
Daily Routine:
• 8am: Check metrics dashboard
• 9-11am: Deep work (docs, planning)
• 11am-12pm: Stand-ups, syncs
• 1-3pm: User research, calls
• 3-5pm: Ad-hoc meetings, Slack
• Evening: Industry reading (Twitter, newsletters)

Tools Used:
• Amplitude (analytics) - daily
• Jira (tickets) - daily
• Figma (design review) - 3x/week
• Google Docs (specs) - daily
• Slack (communication) - constantly

Info Sources:
• Lenny's Newsletter
• Reforge courses
• Product Twitter
• PM communities (Slack groups)
```

### 6. Needs & Expectations
**What must the product provide?**

**Framework: Must-haves vs Nice-to-haves**

**Example - Sarah:**
```
MUST-HAVES:
✓ Fast (she's impatient)
✓ Integrates with existing tools
✓ Easy for non-technical stakeholders
✓ Mobile access (works on-the-go)
✓ Collaborative (team can contribute)

NICE-TO-HAVES:
• AI-powered insights
• Beautiful design
• Customization options
• Templates
• Social features
```

### 7. User Journey Touchpoints
**When/how do they interact with your product?**

**Example - Sarah:**
```
JOURNEY WITH PRODUCT:

Discovery:
• Hears about product from PM community
• Reads reviews on G2/Capterra
• Watches demo video

Evaluation:
• Signs up for trial
• Invites 2 teammates
• Tests with real project

Purchase:
• Discusses with manager (budget approval)
• Negotiates team plan
• Purchases annual subscription

Usage:
• Daily user (checks metrics, updates roadmap)
• Champion within company (onboards new PMs)
• Provides feedback (feature requests)
```

### 8. Quote (Brings Persona to Life)
**A memorable quote that captures essence**

**Example - Sarah:**
```
💬 "I don't have time to learn another complex tool.
   I need something that works immediately and
   doesn't require a PhD to understand the data."
```

**Vietnamese:**

### 8 Thành Phần Persona:

1. **Header**: Tên, ảnh, tagline, demographics
2. **Background**: Tuổi, học vấn, công việc
3. **Goals**: Mục tiêu (nghề nghiệp, cá nhân, sản phẩm)
4. **Frustrations**: Khó khăn hiện tại
5. **Behaviors**: Thói quen hàng ngày, công cụ sử dụng
6. **Needs**: Must-haves vs Nice-to-haves
7. **Journey**: Discovery → Evaluation → Purchase → Usage
8. **Quote**: Câu nói đặc trưng

---

## Creating Personas: Playbook / Tạo Personas

**English:**

### Phase 1: Research (Week 1-2)

**Step 1: Gather Qualitative Data**

**Methods:**
- **User interviews** (10-20 people): 30-60 min each
- **Field studies**: Observe users in their environment
- **Support tickets**: Common complaints
- **Sales calls**: Questions prospects ask

**Interview Questions:**
```
BACKGROUND:
• Tell me about your role
• Walk me through a typical day
• What tools do you use?

GOALS:
• What are you trying to achieve?
• What does success look like?
• What metrics do you care about?

CHALLENGES:
• What's most frustrating?
• What takes too much time?
• What's missing in your current tools?

BEHAVIORS:
• How do you make decisions?
• Where do you find information?
• Who do you collaborate with?
```

**Step 2: Gather Quantitative Data**

**Sources:**
- **Analytics**: User behavior data
- **Surveys**: Demographics, preferences (100+ responses)
- **CRM data**: Customer segments, company size
- **Market research**: Industry reports

**Survey Questions:**
```
• What's your role? (dropdown)
• Company size? (dropdown)
• How often do you use [product category]? (scale)
• What's your biggest challenge with [task]? (open-ended)
• What tools do you use for [task]? (multi-select)
```

### Phase 2: Analysis (Week 3)

**Step 3: Find Patterns**

**Look for clustering:**
- Similar goals
- Similar pain points
- Similar behaviors
- Similar contexts

**Technique: Affinity Mapping**
1. Write each insight on sticky note
2. Group similar notes together
3. Name each group (potential persona)
4. Look for 3-5 distinct groups

**Example - Slack (Early Days):**
```
Pattern Analysis:

Group 1: Tech Startups
• Small teams (10-50 people)
• Fast-moving, collaborative
• Replace email internally
• Care about integrations

Group 2: Distributed Teams
• Remote/hybrid work
• Timezone challenges
• Need async communication
• Video/voice important

Group 3: Enterprise Teams
• Large orgs (1000+ people)
• Security/compliance needs
• IT admin requirements
• Integration with enterprise tools

→ Created 3 personas (initially focused on Group 1)
```

**Step 4: Prioritize Personas**

**Not all personas are equal:**

**Primary Persona (1):**
- Main target user
- Most common use case
- Drives majority of product decisions
- Gets features first

**Secondary Personas (2-3):**
- Important but not primary focus
- Features added after primary persona satisfied
- Inform edge cases

**Tertiary/Negative Personas:**
- Users you're NOT targeting
- Helps say "no" to requests

**Example - Superhuman:**
```
PRIMARY:
"Executive Emma"
• C-level or VP
• Processes 200+ emails/day
• Values speed above all
• Willing to pay premium

SECONDARY:
"Investor Ian"
• VC partner
• High email volume
• Mobile-first
• Early adopter

TERTIARY:
"Casual Casey"
• Personal email only
• 10 emails/day
• Not willing to pay
→ NOT our target
```

### Phase 3: Creation (Week 4)

**Step 5: Write Persona Document**

**Format Options:**
1. **One-pager**: Simple, easy to share
2. **Detailed report**: 3-5 pages per persona
3. **Poster**: Visual, hang on wall
4. **Digital**: Interactive (Figma, Notion)

**Template Structure:**
```
┌─────────────────────────────────────┐
│  [Photo]  "Persona Name"            │
│           Tagline                   │
├─────────────────────────────────────┤
│ BACKGROUND                          │
│ • Demographics                      │
│ • Role & context                    │
├─────────────────────────────────────┤
│ GOALS                               │
│ • What they want to achieve         │
├─────────────────────────────────────┤
│ FRUSTRATIONS                        │
│ • Pain points & challenges          │
├─────────────────────────────────────┤
│ BEHAVIORS                           │
│ • How they work                     │
├─────────────────────────────────────┤
│ NEEDS                               │
│ • Must-haves from product           │
├─────────────────────────────────────┤
│ QUOTE                               │
│ "Memorable quote..."                │
└─────────────────────────────────────┘
```

**Step 6: Validate with Real Users**

**Test your personas:**
- Show to users who fit persona
- Ask: "Does this sound like you?"
- Refine based on feedback

**Red Flags:**
- "That's not really me"
- "I don't care about that"
- "This is too generic"

**Green Lights:**
- "Wow, you nailed it!"
- "How did you know that?"
- "That's exactly my situation"

### Phase 4: Activation (Ongoing)

**Step 7: Socialize Personas**

**Make personas visible:**
- Posters on walls
- Slack channels (e.g., #ask-sarah)
- Presentation to entire company
- Include in onboarding

**Technique: Persona Roleplay**
- Team members "become" persona in meetings
- "As Sarah, I would want..."
- Builds empathy

**Step 8: Use in Decision-Making**

**Apply persona to decisions:**
```
BEFORE:
"Should we add this feature?"
"I think users want it"

AFTER:
"Would Sarah use this feature?"
"It doesn't align with her goals (speed + simplicity)"
"No - doesn't fit primary persona"
```

**Step 9: Keep Personas Alive**

**Update regularly:**
- **Quarterly**: Review and refresh
- **Annually**: Full update (new research)
- **As needed**: When entering new market

**Signs persona needs update:**
- Users don't match persona anymore
- New user segments emerging
- Product pivot

**Vietnamese:**

### Quy Trình 4 Giai Đoạn:

**Giai Đoạn 1: Nghiên Cứu (Tuần 1-2)**
1. Dữ liệu định tính (interviews, field studies)
2. Dữ liệu định lượng (analytics, surveys)

**Giai Đoạn 2: Phân Tích (Tuần 3)**
3. Tìm patterns (affinity mapping)
4. Ưu tiên personas (primary, secondary, tertiary)

**Giai Đoạn 3: Tạo (Tuần 4)**
5. Viết persona document
6. Xác thực với người dùng thực

**Giai Đoạn 4: Kích Hoạt (Liên Tục)**
7. Xã hội hóa (posters, presentations)
8. Sử dụng trong quyết định
9. Cập nhật đều đặn

---

## Real Persona Examples / Ví Dụ Personas Thực Tế

### Example 1: Spotify - "Disco Dan"

```
═══════════════════════════════════
    [Photo: 20s male, casual style]
    DISCO DAN
    "The Social Music Lover"
═══════════════════════════════════

BACKGROUND:
• 24 years old, lives in NYC
• Works in marketing at startup
• Music is core to his identity
• Active social life, parties, concerts

GOALS:
• Discover new music before friends do
• Create perfect playlist for every occasion
• Share music taste (social status)

FRUSTRATIONS:
• Radio too mainstream
• YouTube doesn't work offline
• Hard to organize music
• Can't share easily

BEHAVIORS:
• Listens 3+ hours/day (commute, work, gym)
• Creates 2-3 playlists/week
• Shares music on social media
• Follows 100+ artists

NEEDS:
• Personalized recommendations
• Easy playlist creation
• Social sharing
• Offline mode
• Cross-device sync

QUOTE:
"I need music that fits my mood and helps me
 discover what I'll love next—before everyone
 else finds it."
```

**How Spotify Built for Dan:**
- Discover Weekly (personalized, updated Monday)
- Collaborative playlists (social)
- Offline mode (premium feature)
- Connect with friends (social features)

### Example 2: Figma - "Designer Diana"

```
═══════════════════════════════════
    [Photo: 30s female, creative]
    DESIGNER DIANA
    "The Collaborative Craftsperson"
═══════════════════════════════════

BACKGROUND:
• 28, Senior Product Designer
• Works at mid-size tech company (200 people)
• 5 years design experience
• Reports to Design Director

GOALS:
• Create beautiful, functional designs
• Collaborate smoothly with developers
• Maintain design system consistency
• Get stakeholder buy-in faster

FRUSTRATIONS:
• Sketch doesn't work on Windows (dev team uses PC)
• Sharing designs via email/Slack is clunky
• Version control nightmare
• Hard to get feedback from remote team

BEHAVIORS:
• Designs 6-8 hours/day
• 10+ syncs/week with developers
• Works from coffee shops (need cloud)
• Pixel-perfect, detail-oriented

NEEDS:
• Real-time collaboration
• Works in browser (cross-platform)
• Developer handoff tools
• Version history
• Fast performance

QUOTE:
"I shouldn't have to export, email, and
 explain. Just share a link and collaborate
 in real-time like Google Docs."
```

**How Figma Built for Diana:**
- Browser-based (works anywhere)
- Multiplayer (real-time collab)
- Dev handoff (code snippets)
- Versioning (automatic)
- Fast (WebAssembly performance)

---

## Behavioral Personas vs Demographic Personas / So Sánh

**English:**

### Demographic Personas (Old School)
**Focus:** Who they are (age, gender, income)

**Example:**
```
"Millennial Michelle"
• Age: 28-35
• Gender: Female
• Income: $75K-$100K
• Location: Urban
• Education: College degree
```

**Problem:** Demographics don't predict behavior
- Not all 30-year-old women behave the same
- Income doesn't tell you goals or frustrations

### Behavioral Personas (Modern)
**Focus:** What they do, why they do it

**Example:**
```
"Efficiency-Focused Emily"
• Behavior: Optimizes every workflow
• Goal: Do more in less time
• Uses: Keyboard shortcuts, automation
• Values: Speed > aesthetics
• Frustration: Slow, clunky tools

(Could be 25 or 55, male or female—behavior matters)
```

**Advantage:** Predicts how they'll use product

**Best Practice:** Include demographics but emphasize behaviors

**Vietnamese:**

**Demographic Personas**: Tập trung vào WHO (tuổi, giới tính, thu nhập)
- Vấn đề: Demographics không dự đoán hành vi

**Behavioral Personas**: Tập trung vào WHAT & WHY (hành vi, mục tiêu)
- Ưu điểm: Dự đoán cách sử dụng sản phẩm

**Best Practice**: Bao gồm demographics nhưng nhấn mạnh behaviors

---

## Common Mistakes / Sai Lầm Thường Gặp

### Mistake 1: Making Up Personas Without Research
**Problem**: "Let's just imagine our ideal user"
**Solution**: Base on real user data (interviews, analytics)

### Mistake 2: Too Many Personas
**Problem**: Creating 10 personas, trying to please all
**Solution**: Start with 1 primary persona, max 3 total

### Mistake 3: Too Generic
**Problem**: "Our user is everyone ages 18-65"
**Solution**: Be specific—narrow is better than broad

### Mistake 4: One-Time Exercise
**Problem**: Create personas, file away, never use again
**Solution**: Make personas living documents, reference constantly

### Mistake 5: Personas as Marketing Demographics
**Problem**: Just age, gender, income
**Solution**: Focus on behaviors, goals, frustrations

### Mistake 6: No Negative Personas
**Problem**: Trying to serve everyone
**Solution**: Define who you're NOT building for

---

## Personas vs Related Frameworks / So Sánh

| Framework | Focus | When to Use |
|-----------|-------|-------------|
| **Personas** | Who users are, behaviors | Empathy, alignment |
| **Jobs to Be Done** | What users want to accomplish | Product strategy |
| **User Journey Map** | Experience over time | Service design |
| **Segmentation** | Grouping by characteristics | Marketing |
| **Use Cases** | Specific scenarios | Requirements |

**Relationship:**
- Personas + JTBD = Powerful combo
- Persona is WHO, JTBD is WHAT they're trying to do
- Use together for holistic understanding

---

## Quick Reference Card / Thẻ Tham Khảo Nhanh

### Persona Checklist
- [ ] Based on real research (not assumptions)
- [ ] 3-5 total personas (max)
- [ ] 1 primary persona identified
- [ ] Includes behaviors (not just demographics)
- [ ] Goals clearly defined
- [ ] Frustrations documented
- [ ] Memorable name and tagline
- [ ] Quote that captures essence
- [ ] Validated with real users
- [ ] Visible to team (posters, docs)
- [ ] Used in decision-making
- [ ] Updated regularly

### Key Questions for Persona
1. **Who** are they? (role, background)
2. **What** do they want? (goals)
3. **Why** do they want it? (motivations)
4. **What** stops them? (frustrations)
5. **How** do they behave? (patterns)
6. **What** do they need? (must-haves)

### Red Flags
- ❌ No research data
- ❌ All assumptions
- ❌ Too generic ("everyone")
- ❌ 10+ personas
- ❌ Never referenced after creation
- ❌ Just demographics

### Green Lights
- ✅ Research-backed
- ✅ 1 primary, 2-3 secondary
- ✅ Behavioral focus
- ✅ Specific and memorable
- ✅ Team uses in decisions
- ✅ Updated quarterly

---

**Last Updated**: 2025-11-21
**Version**: 1.0
**Root Commands**: `/phase1:personas`, `/phase2:research`
**Next Review**: 2025-12-21

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
