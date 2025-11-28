---
# Core Metadata
title: "Product Requirements Document (PRD)"
title_vi: "Tài Liệu Yêu Cầu Sản Phẩm"
framework_type: "Documentation"
category: ["Product Management", "Documentation", "Communication"]

# Origin & Authority
author: "Various (Industry Standard)"
organization: "Product Management"
year_developed: "1990s"
original_source: "Software Engineering Best Practices"

# Root Integration
root_phase: ["Phase 3: Document & Plan"]
root_commands: ["/phase3:prd"]
when_to_use: "When documenting features for engineering/design, or getting stakeholder alignment before building"

# Difficulty & Time
complexity: "Medium"
estimated_time: "4-8 hours per PRD"
skill_level: "Intermediate"

# Classification
tags: ["documentation", "requirements", "communication", "stakeholder-alignment", "specifications"]
related_frameworks: ["User Stories", "Agile", "Technical Specs"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-20"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Article"
    title: "How to Write a PRD"
    url: "https://www.atlassian.com/agile/product-management/requirements"
    author: "Atlassian"
    year: "2024"
  - type: "Article"
    title: "Product Requirements Document (PRD)"
    url: "https://www.productplan.com/glossary/product-requirements-document/"
    author: "ProductPlan"
    year: "2024"
  - type: "Article"
    title: "SVPG Resources"
    url: "https://www.svpg.com/resources/"
    author: "SVPG (Marty Cagan)"
    year: "2024"
  - type: "Tool"
    title: "PRD Template (Notion)"
    url: "https://www.notion.so/templates/product-requirements-document"
    author: "Notion"
    year: "2024"
---

# PRD (Product Requirements Document) / Tài Liệu Yêu Cầu Sản Phẩm

## Overview / Tổng Quan

**English:**
A PRD is like a recipe for building a product. It tells engineers, designers, and stakeholders exactly what to build and why. It's the single source of truth that aligns everyone on the problem, solution, requirements, and success criteria.

**Think of it like this:**
- **Recipe** = PRD
- **Ingredients** = Requirements
- **Steps** = Implementation plan
- **Final dish** = Shipped product
- **Taste test** = Success metrics

A great PRD answers three fundamental questions:
1. **Why are we building this?** (Problem & Goals)
2. **What exactly are we building?** (Requirements & Specifications)
3. **How will we know if it's successful?** (Success Metrics)

**Vietnamese:**
PRD giống như một công thức nấu ăn để xây dựng sản phẩm. Nó cho kỹ sư, nhà thiết kế và các bên liên quan biết chính xác cần xây dựng cái gì và tại sao. Đây là nguồn chân lý duy nhất giúp mọi người đồng thuận về vấn đề, giải pháp, yêu cầu và tiêu chí thành công.

**Hiểu đơn giản:**
- **Công thức nấu ăn** = PRD
- **Nguyên liệu** = Yêu cầu
- **Các bước** = Kế hoạch triển khai
- **Món ăn hoàn thành** = Sản phẩm ra mắt
- **Nếm thử** = Chỉ số thành công

Một PRD tốt trả lời ba câu hỏi cơ bản:
1. **Tại sao chúng ta xây dựng điều này?** (Vấn đề & Mục tiêu)
2. **Chính xác chúng ta đang xây dựng gì?** (Yêu cầu & Thông số kỹ thuật)
3. **Làm thế nào để biết nó thành công?** (Chỉ số thành công)

---

## Why PRDs Matter / Tại Sao PRD Quan Trọng

**English:**

### The Cost of Poor Documentation

Without a clear PRD, teams face:
- **Misalignment**: Engineering builds X, design expects Y, stakeholders wanted Z
- **Rework**: 30-50% of development time wasted on wrong implementations
- **Missed deadlines**: Scope creep and unclear requirements cause delays
- **Frustrated teams**: Constant "what should this do?" questions interrupt flow
- **Failed launches**: Product doesn't solve the actual problem

### The Value of Good PRDs

A well-written PRD:
- **Saves 40% of development time** by preventing rework
- **Reduces meetings** by 60% (answers documented upfront)
- **Increases launch success rate** from 35% to 70%
- **Improves team morale** (no more guessing games)
- **Creates institutional knowledge** (future reference)

**Real Example - Slack's "Threads" Feature:**

Slack's PRD for threads likely included:
- **Problem**: Messages in busy channels get lost (1,200 support tickets/month)
- **Solution**: Allow replies to specific messages
- **Success Metric**: 40% reduction in "I can't find that message" support tickets
- **User Story**: "As a team member, I want to reply to a specific message without cluttering the main channel"
- **Requirements**: Threading UI, notifications, search integration

Result: Threads became one of Slack's most-used features, reducing support costs and improving user satisfaction.

**Vietnamese:**

### Chi Phí Của Tài Liệu Kém

Không có PRD rõ ràng, các đội nhóm phải đối mặt với:
- **Thiếu đồng bộ**: Kỹ thuật xây dựng X, thiết kế mong đợi Y, các bên liên quan muốn Z
- **Làm lại**: 30-50% thời gian phát triển lãng phí vào triển khai sai
- **Trễ deadline**: Mở rộng phạm vi và yêu cầu không rõ gây trzadržení
- **Đội nhóm thất vọng**: Liên tục bị gián đoạn bởi câu hỏi "cái này phải làm gì?"
- **Ra mắt thất bại**: Sản phẩm không giải quyết vấn đề thực tế

### Giá Trị Của PRD Tốt

Một PRD được viết tốt:
- **Tiết kiệm 40% thời gian phát triển** bằng cách ngăn chặn làm lại
- **Giảm 60% cuộc họp** (câu trả lời được ghi chép sẵn)
- **Tăng tỷ lệ thành công ra mắt** từ 35% lên 70%
- **Cải thiện tinh thần đội nhóm** (không còn đoán mò)
- **Tạo kiến thức tổ chức** (tài liệu tham khảo tương lai)

---

## Standard PRD Structure / Cấu Trúc PRD Chuẩn

**English:**

A comprehensive PRD typically includes these sections:

### 1. Executive Summary
**Purpose**: 30-second elevator pitch
**What to include**:
- One-sentence description
- Problem statement
- Proposed solution
- Expected impact

**Example:**
> "We're building a dark mode feature to reduce eye strain for users working at night, which affects 45% of our active users. Expected result: 20% increase in evening engagement."

### 2. Problem Statement
**Purpose**: Define the problem you're solving
**What to include**:
- Current situation
- Who is affected
- Why it matters (business + user impact)
- Data/evidence supporting the problem

**Example:**
> "Currently, 45% of our users (18,000 people) work in our app between 8 PM - 12 AM. We receive 250 support tickets/month about eye strain. Competitors (Notion, Slack) all have dark mode. Lack of dark mode contributes to 15% churn in our evening user segment."

### 3. Goals & Success Metrics
**Purpose**: Define what success looks like
**What to include**:
- Business goals (revenue, retention, acquisition)
- User goals (satisfaction, usage, efficiency)
- Specific, measurable targets
- Timeline for measurement

**Example:**
| Metric | Baseline | Target | Timeline |
|--------|----------|--------|----------|
| Evening engagement | 120 min/week | 150 min/week | 3 months post-launch |
| Eye strain tickets | 250/month | 100/month | 1 month post-launch |
| User preference adoption | 0% | 40% | 6 months post-launch |
| Evening user churn | 15% | 10% | 3 months post-launch |

### 4. Target Users & User Stories
**Purpose**: Define who this is for and what they need
**What to include**:
- User personas
- User stories (As a [role], I want [action], so that [benefit])
- Use cases and scenarios
- Edge cases

**Example User Stories:**
- "As a developer working late, I want dark mode, so my eyes don't hurt after 8 hours of coding"
- "As a night owl, I want to toggle dark mode automatically at sunset, so I don't have to remember"
- "As a designer, I want dark mode that maintains brand colors, so our UI stays recognizable"

### 5. Requirements & Specifications
**Purpose**: Define exactly what to build
**What to include**:
- **Functional requirements**: What the feature must do
- **Non-functional requirements**: Performance, security, accessibility
- **Technical constraints**: Platform limitations, dependencies
- **Design requirements**: UX/UI specifications
- **Priority levels**: Must-have vs. nice-to-have

**Example:**

**Functional Requirements (Must-Have):**
- FR-1: User can toggle between light and dark mode from settings
- FR-2: System remembers user's preference across sessions
- FR-3: All text remains readable (WCAG AA contrast standards)
- FR-4: Images/icons have dark mode variants

**Functional Requirements (Nice-to-Have):**
- FR-5: Auto-switch based on system preferences
- FR-6: Scheduled auto-switch (sunset/sunrise)
- FR-7: Per-workspace dark mode settings

**Non-Functional Requirements:**
- NFR-1: Mode switch completes in <200ms
- NFR-2: No flash of wrong theme on page load
- NFR-3: Works on all supported browsers (Chrome, Safari, Firefox, Edge)

### 6. Out of Scope
**Purpose**: Prevent scope creep by explicitly stating what's NOT included
**What to include**:
- Features considered but deferred
- Related features for future versions
- Explicit boundaries

**Example:**
- ❌ Custom color themes (v2.0)
- ❌ Per-page dark mode (v2.0)
- ❌ Dark mode for marketing website (separate PRD)
- ❌ Accessibility audit for existing features (separate initiative)

### 7. User Experience & Design
**Purpose**: Show how users will interact with the feature
**What to include**:
- User flows
- Wireframes/mockups
- Interaction patterns
- Error states
- Edge cases

**Example User Flow:**
```
1. User opens Settings → Appearance
2. User sees toggle: [Light Mode] / [Dark Mode]
3. User clicks Dark Mode
4. System immediately applies dark theme (200ms transition)
5. System saves preference to user profile
6. Confirmation toast: "Dark mode enabled"
```

### 8. Dependencies & Risks
**Purpose**: Identify blockers and potential issues
**What to include**:
- Technical dependencies
- Team dependencies
- Third-party services
- Known risks and mitigation plans

**Example:**

**Dependencies:**
- Design system update (dark mode color tokens)
- CSS variables support in legacy components
- Image asset creation (dark variants)

**Risks:**
| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|------------|
| CSS conflicts in legacy code | High | Medium | Audit + refactor legacy components first |
| Performance issues | Low | High | Performance testing + optimization |
| Accessibility failures | Medium | High | Accessibility audit + WCAG testing |

### 9. Implementation Plan
**Purpose**: Break down how to build this
**What to include**:
- Phases/milestones
- Estimated effort
- Team assignments
- Timeline

**Example:**

**Phase 1: Foundation (2 weeks)**
- Design system update (dark mode tokens)
- Core infrastructure (theme context, storage)

**Phase 2: UI Implementation (3 weeks)**
- Update all components (buttons, forms, cards)
- Create dark mode image variants
- Testing + bug fixes

**Phase 3: Launch (1 week)**
- Beta testing with 100 users
- Rollout to 100% of users
- Monitor metrics

### 10. Launch & Rollout Plan
**Purpose**: Define how to release this safely
**What to include**:
- Rollout strategy (feature flag, gradual rollout, all-at-once)
- Beta testing plan
- Rollback plan
- Communication plan

**Example:**
- Week 1: Internal dogfooding (company employees)
- Week 2: Beta to 5% of users (opt-in)
- Week 3: Gradual rollout to 25% → 50% → 100%
- Feature flag: Can roll back in <5 minutes if critical issues

### 11. Success Criteria & Validation
**Purpose**: Define when we can call this "done"
**What to include**:
- Launch criteria (what must be true to ship)
- Acceptance criteria (definition of done)
- Validation plan (how to test)
- Post-launch monitoring

**Example:**

**Launch Criteria:**
- ✅ All must-have requirements implemented
- ✅ Passes accessibility audit (WCAG AA)
- ✅ Performance <200ms theme switch
- ✅ Zero critical bugs
- ✅ Beta users report >80% satisfaction

**Post-Launch Monitoring (First 30 Days):**
- Daily: Error rates, performance metrics
- Weekly: Adoption rate, user feedback
- Monthly: Impact on success metrics

### 12. Open Questions & Assumptions
**Purpose**: Document unknowns and assumptions
**What to include**:
- Questions that need answers
- Assumptions that need validation
- Decisions pending

**Example:**

**Open Questions:**
- Q: Should we migrate existing users to dark mode automatically?
- Q: What about users with custom CSS?
- Q: Do we need dark mode for email notifications?

**Assumptions:**
- Users will manually enable dark mode (not auto-enabled)
- Most users use modern browsers (95%+)
- Design team can create all dark assets in 1 week

**Vietnamese:**

Một PRD toàn diện thường bao gồm các phần sau:

### 1. Tóm Tắt Điều Hành
Giới thiệu 30 giây về tính năng

### 2. Phát Biểu Vấn Đề
Định nghĩa vấn đề bạn đang giải quyết

### 3. Mục Tiêu & Chỉ Số Thành Công
Định nghĩa thành công trông như thế nào

### 4. Người Dùng Mục Tiêu & User Stories
Định nghĩa cho ai và họ cần gì

### 5. Yêu Cầu & Thông Số Kỹ Thuật
Định nghĩa chính xác cần xây dựng gì

### 6. Ngoài Phạm Vi
Ngăn chặn mở rộng phạm vi bằng cách nói rõ những gì KHÔNG bao gồm

### 7. Trải Nghiệm Người Dùng & Thiết Kế
Cho thấy người dùng sẽ tương tác với tính năng như thế nào

### 8. Phụ Thuộc & Rủi Ro
Xác định blocker và vấn đề tiềm ẩn

### 9. Kế Hoạch Triển Khai
Chia nhỏ cách xây dựng điều này

### 10. Kế Hoạch Ra Mắt
Định nghĩa cách phát hành an toàn

### 11. Tiêu Chí Thành Công & Xác Thực
Định nghĩa khi nào có thể gọi là "hoàn thành"

### 12. Câu Hỏi Mở & Giả Định
Ghi chép những điều chưa biết và giả định

---

## PRD Writing Playbook / Hướng Dẫn Viết PRD

**English:**

### Step 1: Start with the Problem (30 minutes)

**Before writing anything, answer these questions:**
1. What problem are we solving?
2. Who has this problem?
3. How do we know it's a real problem? (Data)
4. What happens if we don't solve it?
5. Why now?

**Good Problem Statement:**
> "45% of our users (18,000 people) work in our app at night. We receive 250 support tickets/month about eye strain. Competitors have dark mode. This contributes to 15% churn in evening users. Market research shows 78% of users prefer dark mode for night usage."

**Bad Problem Statement:**
> "Some users want dark mode because it looks cool."

**Red Flags:**
- ❌ Solution disguised as problem ("We need dark mode" vs. "Users get eye strain")
- ❌ No data or evidence
- ❌ Vague language ("some users", "could be better")
- ❌ Missing impact (why does this matter?)

### Step 2: Define Success Metrics (30 minutes)

**Ask yourself:**
1. How will we measure if this solves the problem?
2. What specific numbers can we track?
3. What's realistic? (Don't set impossible targets)
4. When will we measure?

**Framework for Metrics:**
- **Input metrics**: What users do (adoption rate, usage frequency)
- **Output metrics**: What we achieve (satisfaction, retention, revenue)
- **Leading indicators**: Early signals (beta feedback, early adoption)
- **Lagging indicators**: Long-term results (churn, NPS)

**Good Metrics:**
| Metric | Baseline | Target | Timeline |
|--------|----------|--------|----------|
| Dark mode adoption | 0% | 40% | 6 months |
| Evening engagement | 120 min/week | 150 min/week | 3 months |
| Eye strain tickets | 250/month | 100/month | 1 month |

**Bad Metrics:**
- "Make users happy" (not measurable)
- "Improve the app" (too vague)
- "Be better than competitors" (not specific)

### Step 3: Write User Stories (1 hour)

**Use this format:**
> As a [type of user], I want [action], so that [benefit].

**Good User Stories:**
- "As a developer working late, I want dark mode, so my eyes don't hurt after 8 hours"
- "As a manager reviewing reports at night, I want dark mode that's easy to toggle, so I can switch it on quickly"
- "As a designer, I want dark mode that maintains brand colors, so our UI stays recognizable"

**For each story, add:**
- **Acceptance criteria**: How do we know it's done?
- **Priority**: Must-have, should-have, nice-to-have
- **Estimate**: How long to build?

**Example:**
```
Story: As a developer working late, I want dark mode, so my eyes don't hurt

Acceptance Criteria:
- [ ] Dark mode toggle exists in Settings
- [ ] Dark mode applies to all pages
- [ ] Text meets WCAG AA contrast standards
- [ ] Preference persists across sessions

Priority: Must-Have
Estimate: 3 weeks (design + development + testing)
```

### Step 4: Detail Requirements (2-3 hours)

**Break into categories:**

**1. Functional Requirements (What it does):**
- FR-1: User can toggle dark mode from settings
- FR-2: System remembers preference
- FR-3: All text remains readable

**2. Non-Functional Requirements (How well it does it):**
- NFR-1: Toggle responds in <200ms
- NFR-2: Works on all supported browsers
- NFR-3: Meets WCAG AA accessibility standards

**3. Design Requirements (How it looks/feels):**
- DR-1: Uses brand-approved dark color palette
- DR-2: Smooth 200ms transition animation
- DR-3: Consistent with iOS/Android system dark modes

**For each requirement:**
- Assign a unique ID (FR-1, NFR-1, etc.)
- Mark priority (P0 = must-have, P1 = should-have, P2 = nice-to-have)
- Link to designs/specs if applicable
- Add acceptance criteria

**Example:**
```
FR-1: User can toggle dark mode [P0]
- User navigates to Settings → Appearance
- Toggle switch labeled "Dark Mode"
- Toggle state clearly visible (on/off)
- Immediate visual feedback (<200ms)
- Confirmation message displays
See designs: figma.com/file/abc123
```

### Step 5: Define What's Out of Scope (30 minutes)

**This is critical to prevent scope creep!**

List everything that's related but NOT included:
- ❌ Custom color themes (v2.0)
- ❌ Per-page dark mode (v2.0)
- ❌ Marketing website dark mode (separate PRD)
- ❌ Accessibility audit of existing features (separate initiative)

**For each out-of-scope item:**
- Explain why it's excluded
- When it might be included (v2.0, separate PRD, never)
- Who to contact if questions arise

### Step 6: Identify Dependencies & Risks (1 hour)

**Dependencies:**
List everything that must happen first:
- Design system update (dark mode color tokens) → Design team, 1 week
- Image assets (dark variants) → Design team, 1 week
- Feature flag infrastructure → Platform team, already exists

**Risks:**
| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|------------|
| CSS conflicts | High | Medium | Audit legacy code first |
| Performance issues | Low | High | Load testing + optimization |
| Accessibility failures | Medium | High | WCAG audit + testing |

**For each risk:**
- Describe what could go wrong
- Assess likelihood (Low/Medium/High)
- Assess impact (Low/Medium/High)
- Define mitigation plan
- Assign owner

### Step 7: Create Implementation Plan (1 hour)

**Break into phases:**

**Phase 1: Foundation (2 weeks)**
- Week 1: Design system update
- Week 2: Core infrastructure

**Phase 2: Implementation (3 weeks)**
- Week 3-4: Component updates
- Week 5: Testing + bug fixes

**Phase 3: Launch (1 week)**
- Week 6: Beta testing + gradual rollout

**For each phase:**
- List deliverables
- Assign team members
- Estimate effort
- Define "done" criteria

### Step 8: Plan the Launch (1 hour)

**Rollout Strategy:**
- Week 1: Internal dogfooding
- Week 2: Beta to 5% of users
- Week 3: Gradual rollout (25% → 50% → 100%)
- Feature flag for quick rollback

**Communication Plan:**
- Announce in-app notification
- Blog post about dark mode
- Social media campaign
- Email to power users

**Monitoring Plan:**
- Daily: Error rates, performance
- Weekly: Adoption, user feedback
- Monthly: Impact on success metrics

### Step 9: Review & Iterate (1-2 hours)

**Before sharing with stakeholders, review:**

**Completeness Checklist:**
- [ ] Problem clearly stated with data
- [ ] Success metrics defined and measurable
- [ ] User stories cover all personas
- [ ] Requirements complete and prioritized
- [ ] Out-of-scope explicitly stated
- [ ] Dependencies identified
- [ ] Risks assessed with mitigation
- [ ] Implementation plan realistic
- [ ] Launch plan detailed
- [ ] Stakeholders identified

**Get feedback from:**
- Engineering lead (is this buildable?)
- Design lead (is this designable?)
- Product manager (is this aligned with strategy?)
- Stakeholders (does this solve the business problem?)

**Iterate based on feedback:**
- Add missing requirements
- Clarify ambiguous sections
- Adjust estimates
- Update success metrics
- Refine scope

### Step 10: Maintain the PRD (Ongoing)

**PRDs are living documents!**

**Update when:**
- Requirements change
- Dependencies shift
- Risks materialize
- Timeline changes
- Scope adjusts

**Version control:**
- Track major changes
- Document decision rationale
- Keep history for future reference

**Example:**
```
Version History:
- v1.0 (2025-01-15): Initial PRD
- v1.1 (2025-01-22): Added NFR-4 (browser compatibility)
- v1.2 (2025-02-01): Removed FR-5 (auto-switch) - moved to v2.0
- v2.0 (2025-02-15): Launch complete, updated with actual metrics
```

**Vietnamese:**

### Bước 1: Bắt Đầu Với Vấn Đề (30 phút)
Trước khi viết bất cứ điều gì, trả lời những câu hỏi này

### Bước 2: Định Nghĩa Chỉ Số Thành Công (30 phút)
Làm thế nào để đo lường nếu điều này giải quyết vấn đề?

### Bước 3: Viết User Stories (1 giờ)
Sử dụng định dạng: Là một [loại người dùng], tôi muốn [hành động], để [lợi ích]

### Bước 4: Chi Tiết Yêu Cầu (2-3 giờ)
Chia thành các loại: Chức năng, Phi chức năng, Thiết kế

### Bước 5: Định Nghĩa Ngoài Phạm Vi (30 phút)
Liệt kê mọi thứ liên quan nhưng KHÔNG bao gồm

### Bước 6: Xác Định Phụ Thuộc & Rủi Ro (1 giờ)
Liệt kê mọi thứ phải xảy ra trước và những gì có thể sai

### Bước 7: Tạo Kế Hoạch Triển Khai (1 giờ)
Chia thành các giai đoạn với các sản phẩm và ước tính

### Bước 8: Lập Kế Hoạch Ra Mắt (1 giờ)
Chiến lược rollout, kế hoạch truyền thông, kế hoạch giám sát

### Bước 9: Xem Xét & Lặp Lại (1-2 giờ)
Kiểm tra tính đầy đủ, nhận phản hồi, lặp lại

### Bước 10: Duy Trì PRD (Liên tục)
PRD là tài liệu sống! Cập nhật khi yêu cầu thay đổi

---

## Best Practices / Thực Hành Tốt Nhất

**English:**

### 1. Write for Your Audience

**Different stakeholders need different things:**

**For Engineers:**
- Detailed functional requirements
- Technical constraints
- API specifications
- Edge cases
- Performance requirements

**For Designers:**
- User flows
- Interaction patterns
- Accessibility requirements
- Visual specifications
- Responsive behavior

**For Business Stakeholders:**
- Executive summary
- Business goals
- Success metrics
- Timeline
- Budget/resources

**For QA/Testing:**
- Acceptance criteria
- Test scenarios
- Edge cases
- Success criteria

**Pro Tip:** Create a "TL;DR" section at the top with role-specific summaries:
```
TL;DR:
- Engineers: See "Requirements" (section 5) and "Technical Specs" (section 8)
- Designers: See "User Experience" (section 7) and "User Stories" (section 4)
- Leadership: See "Executive Summary" (section 1) and "Success Metrics" (section 3)
```

### 2. Use Data, Not Opinions

**Bad:**
> "Users probably want dark mode because it's trendy"

**Good:**
> "45% of users (18,000) work at night. Survey shows 78% prefer dark mode. Competitors (Notion, Slack, GitHub) all have dark mode. We receive 250 tickets/month about eye strain."

**Sources of data:**
- User research (interviews, surveys)
- Analytics (usage patterns, behavior data)
- Support tickets (pain points, requests)
- Competitive analysis (market trends)
- A/B tests (validation experiments)

### 3. Be Specific and Concrete

**Bad:**
> "The feature should be fast and easy to use"

**Good:**
> "Dark mode toggle must respond in <200ms (NFR-1). Toggle must be accessible within 2 clicks from any page (DR-1). 90% of users should successfully enable dark mode on first attempt without help (measured in beta testing)."

**Specificity checklist:**
- [ ] Numbers instead of adjectives ("30% increase" not "significant improvement")
- [ ] Concrete criteria ("3 clicks" not "easy")
- [ ] Measurable outcomes ("200ms" not "fast")
- [ ] Clear definitions ("WCAG AA" not "accessible")

### 4. Prioritize Ruthlessly

**Use MoSCoW:**
- **Must-Have (P0)**: Ship-blockers, core functionality
- **Should-Have (P1)**: Important but not critical
- **Could-Have (P2)**: Nice-to-haves, can be deferred
- **Won't-Have**: Out of scope for this version

**Example:**
- ✅ P0: Toggle dark mode on/off (Must-Have)
- ✅ P1: Remember preference (Should-Have)
- ⚠️ P2: Auto-switch at sunset (Could-Have)
- ❌ P3: Custom color themes (Won't-Have this version)

**Why this matters:**
- Prevents scope creep
- Helps with trade-off decisions
- Makes cutting scope easier when needed
- Aligns team on what matters most

### 5. Include Visual Examples

**PRDs with visuals are 3x more likely to be implemented correctly!**

**Include:**
- User flows (how users navigate)
- Wireframes (basic layout)
- Mockups (visual design)
- State diagrams (different states/modes)
- Error states (what happens when things go wrong)
- Edge cases (unusual scenarios)

**Example:**
```
User Flow: Enable Dark Mode

[Settings Page]
   ↓ User clicks "Appearance"
[Appearance Settings]
   ↓ User toggles "Dark Mode" switch
[Loading State] (200ms)
   ↓ Theme applied
[Dark Mode Active]
   ↓ Confirmation toast shows
[Success State]
```

### 6. Document Decisions and Rationale

**For every major decision, document:**
- What was decided
- Why it was decided
- What alternatives were considered
- What trade-offs were made

**Example:**
```
Decision: Use CSS-in-JS for dark mode (not separate stylesheets)

Rationale:
- ✅ Dynamic theme switching without page reload
- ✅ Scoped styles prevent conflicts
- ✅ Aligns with existing tech stack

Alternatives Considered:
- ❌ Separate dark.css stylesheet → Requires page reload, worse UX
- ❌ CSS custom properties only → Not supported in legacy browsers

Trade-offs:
- 🟡 Slight bundle size increase (~15kb)
- ✅ Better UX worth the cost
```

**Why this matters:**
- Future you will forget why decisions were made
- New team members need context
- Prevents re-litigating old decisions
- Creates institutional knowledge

### 7. Keep It Updated

**PRDs are living documents!**

**Update when:**
- Requirements change (scope adjustments)
- Dependencies shift (blockers removed/added)
- Risks materialize (what we feared happened)
- Timeline changes (delays or acceleration)
- Launch happens (actual vs. planned metrics)

**How to update:**
- Use version numbers (v1.0, v1.1, v2.0)
- Track changes in version history
- Use strikethrough for removed items (not delete)
- Add date stamps to changes
- Notify stakeholders of major updates

**Example:**
```
Version History:
- v1.0 (2025-01-15): Initial PRD approved
- v1.1 (2025-01-22): Added NFR-4 browser compatibility after tech review
- v1.2 (2025-02-01): Removed FR-5 (auto-switch) due to technical constraints
- v2.0 (2025-03-01): Launch complete! Updated with actual metrics
```

### 8. Link to Related Documents

**PRD is the hub, but link to:**
- Design files (Figma, Sketch)
- Technical specs (architecture docs)
- User research (interview notes, surveys)
- Competitive analysis
- Related PRDs (dependencies)
- Project management (Jira, Linear)
- Analytics dashboards
- Launch checklist

**Example:**
```
Related Documents:
- 🎨 Designs: https://figma.com/file/dark-mode-v2
- 🏗️ Tech Spec: /docs/technical/dark-mode-architecture.md
- 📊 User Research: /research/dark-mode-user-interviews.pdf
- 🚀 Launch Checklist: /launch/dark-mode-checklist.md
- 📈 Analytics Dashboard: https://analytics.com/dashboard/dark-mode
```

### 9. Make It Scannable

**People won't read 20 pages. Make it scannable!**

**Use:**
- Clear section headings
- Bullet points (not walls of text)
- Tables for comparisons
- Visual hierarchy (headings, subheadings)
- Callout boxes for important info
- TL;DR summaries
- Table of contents (for long PRDs)

**Good structure:**
```
## Section Heading

**Key Point**: One-sentence summary of this section.

**Details:**
- Point 1: Clear, specific
- Point 2: Clear, specific
- Point 3: Clear, specific

| Comparison | Option A | Option B |
|------------|----------|----------|
| Metric 1   | Value    | Value    |
```

### 10. Get Feedback Early and Often

**Don't write the PRD in isolation!**

**Review process:**

**Draft 1 (Day 1):**
- Write problem statement, goals, user stories
- Share with PM team for feedback
- Iterate based on feedback

**Draft 2 (Day 3):**
- Add requirements, dependencies, risks
- Share with engineering + design leads
- Iterate based on technical feasibility

**Draft 3 (Day 5):**
- Complete all sections
- Share with all stakeholders
- Get final approvals

**Final (Day 7):**
- Incorporate all feedback
- Get sign-offs
- Publish and share broadly

**Who to get feedback from:**
- PM team (strategic alignment)
- Engineering (technical feasibility)
- Design (user experience)
- QA (testability)
- Legal/Compliance (if applicable)
- Customer success (support impact)
- Marketing (go-to-market)

**Vietnamese:**

### 1. Viết Cho Đối Tượng Của Bạn
Các bên liên quan khác nhau cần những thứ khác nhau

### 2. Sử Dụng Dữ Liệu, Không Phải Ý Kiến
Nguồn dữ liệu: Nghiên cứu người dùng, phân tích, ticket hỗ trợ, phân tích cạnh tranh

### 3. Cụ Thể Và Rõ Ràng
Số liệu thay vì tính từ, tiêu chí cụ thể, kết quả đo lường được

### 4. Ưu Tiên Không Thương Xót
Sử dụng MoSCoW: Must-Have, Should-Have, Could-Have, Won't-Have

### 5. Bao Gồm Ví Dụ Trực Quan
User flows, wireframes, mockups, state diagrams, error states

### 6. Ghi Chép Quyết Định Và Lý Do
Quyết định gì, tại sao, phương án thay thế, đánh đổi

### 7. Giữ Nó Được Cập Nhật
PRD là tài liệu sống! Cập nhật khi yêu cầu, phụ thuộc, rủi ro, timeline thay đổi

### 8. Liên Kết Đến Tài Liệu Liên Quan
Tệp thiết kế, thông số kỹ thuật, nghiên cứu người dùng, checklist ra mắt

### 9. Làm Cho Nó Dễ Quét
Tiêu đề rõ ràng, bullet points, bảng, phân cấp trực quan, hộp callout

### 10. Nhận Phản Hồi Sớm Và Thường Xuyên
Đừng viết PRD trong sự cô lập! Xem xét quy trình: Draft 1 → Draft 2 → Draft 3 → Final

---

## Common Mistakes to Avoid / Lỗi Thường Gặp Cần Tránh

**English:**

### 1. Solution Disguised as Problem

**❌ Wrong:**
> "Problem: We don't have dark mode."

**✅ Right:**
> "Problem: 45% of users (18,000) work at night and report eye strain (250 tickets/month). This contributes to 15% churn in evening users."

**Why it matters:** If you start with a solution, you might build the wrong thing. Start with the problem, then explore solutions.

### 2. Vague Success Metrics

**❌ Wrong:**
> "Success: Users like the feature"

**✅ Right:**
> "Success: 40% dark mode adoption within 6 months, 60% reduction in eye strain tickets within 1 month, 5% improvement in evening user retention within 3 months"

**Why it matters:** Can't improve what you can't measure. Vague metrics = no accountability.

### 3. Missing Priorities

**❌ Wrong:**
> "Requirements:
> - Dark mode toggle
> - Auto-switch at sunset
> - Custom color themes
> - Per-page dark mode"

**✅ Right:**
> "Requirements:
> - [P0] Dark mode toggle
> - [P1] Auto-switch at sunset
> - [P2] Custom color themes (v2.0)
> - [P2] Per-page dark mode (v2.0)"

**Why it matters:** Without priorities, everything feels important. This leads to scope creep and missed deadlines.

### 4. No Out-of-Scope Section

**❌ Wrong:**
> (No mention of what's NOT included)

**✅ Right:**
> "Out of Scope:
> - ❌ Custom color themes (v2.0)
> - ❌ Marketing website dark mode (separate PRD)
> - ❌ Dark mode for emails (future consideration)"

**Why it matters:** If you don't explicitly state what's excluded, stakeholders will assume it's included. Prevents scope creep.

### 5. Ignoring Dependencies and Risks

**❌ Wrong:**
> (No mention of dependencies or risks)

**✅ Right:**
> "Dependencies:
> - Design system update (1 week) - blocks development
> - Feature flag infrastructure - already exists
>
> Risks:
> - High: CSS conflicts in legacy code → Mitigation: Audit first
> - Medium: Accessibility failures → Mitigation: WCAG audit"

**Why it matters:** Ignoring dependencies and risks doesn't make them go away. Better to identify and plan for them upfront.

### 6. Writing for Yourself, Not Your Audience

**❌ Wrong:**
> "Implement dark mode using CSS-in-JS with ThemeProvider context wrapping the app tree and dynamically injecting style tags based on theme state stored in localStorage with SSR hydration support"

**✅ Right:**
> "For Engineers: Use CSS-in-JS with ThemeProvider (see tech spec for details)
> For Designers: All components will support dark mode (see Figma for colors)
> For Leadership: This solves eye strain for 18,000 evening users"

**Why it matters:** Different audiences need different information. Make it easy for them to find what they need.

### 7. Walls of Text

**❌ Wrong:**
> "The user interface for dark mode should provide users with a way to toggle between light and dark themes and this toggle should be easily accessible from the settings menu and should clearly indicate the current state and should provide immediate visual feedback when clicked and should remember the user's preference across sessions and should also support system-level dark mode preferences and automatically switch based on the user's operating system settings..."

**✅ Right:**
> "Dark Mode Toggle Requirements:
> - Location: Settings → Appearance
> - Visual: Clear on/off state
> - Feedback: Immediate (200ms)
> - Persistence: Saved to user profile
> - Auto-sync: Respects system preferences (optional)"

**Why it matters:** Nobody reads walls of text. Break it up with bullet points, tables, and headings.

### 8. No User Stories

**❌ Wrong:**
> "Add dark mode feature"

**✅ Right:**
> "User Stories:
> - As a developer working late, I want dark mode, so my eyes don't hurt after 8 hours
> - As a manager reviewing reports at night, I want dark mode that's easy to toggle, so I can switch it quickly
> - As a designer, I want dark mode that maintains brand colors, so our UI stays recognizable"

**Why it matters:** User stories keep you focused on user needs, not just shipping features.

### 9. Forgetting Edge Cases

**❌ Wrong:**
> "User clicks dark mode toggle, dark mode activates"

**✅ Right:**
> "Happy Path: User clicks toggle → Dark mode activates → Confirmation shown
>
> Edge Cases:
> - User has custom CSS → Custom CSS takes precedence with warning
> - User switches mid-page load → Wait for page load, then apply
> - User on unsupported browser → Show graceful degradation message
> - User toggles rapidly → Debounce (ignore rapid clicks)"

**Why it matters:** Edge cases are where bugs live. Better to think through them upfront.

### 10. Set It and Forget It

**❌ Wrong:**
> Writes PRD → Ships feature → Never updates PRD

**✅ Right:**
> Writes PRD → Ships feature → Updates PRD with:
> - Actual metrics vs. targets
> - What worked / what didn't
> - Lessons learned
> - Future improvements

**Why it matters:** PRDs are living documents. They're also historical records that help future teams understand what was built and why.

### 11. No Acceptance Criteria

**❌ Wrong:**
> "Build dark mode feature"

**✅ Right:**
> "Acceptance Criteria:
> - [ ] User can toggle dark mode from Settings
> - [ ] Dark mode applies to all pages
> - [ ] Text meets WCAG AA contrast standards
> - [ ] Preference persists across sessions
> - [ ] No flash of wrong theme on page load
> - [ ] Works on Chrome, Safari, Firefox, Edge
> - [ ] 90% of beta users successfully enable it"

**Why it matters:** Clear acceptance criteria = clear definition of "done". Prevents endless "is it done yet?" questions.

### 12. Ignoring Non-Functional Requirements

**❌ Wrong:**
> Only specifies what the feature does (functional requirements)

**✅ Right:**
> "Functional Requirements:
> - FR-1: Toggle dark mode
> - FR-2: Save preference
>
> Non-Functional Requirements:
> - NFR-1: Toggle responds in <200ms
> - NFR-2: Works offline
> - NFR-3: Accessible (WCAG AA)
> - NFR-4: Secure (no XSS vulnerabilities)"

**Why it matters:** Non-functional requirements (performance, security, accessibility) are just as important as functional ones. Don't forget them!

**Vietnamese:**

### Lỗi Thường Gặp:

1. **Giải pháp được ngụy trang thành vấn đề**: Bắt đầu với vấn đề, không phải giải pháp
2. **Chỉ số thành công mơ hồ**: Không thể cải thiện những gì không thể đo lường
3. **Thiếu ưu tiên**: Mọi thứ cảm thấy quan trọng → scope creep
4. **Không có phần Ngoài Phạm Vi**: Ngăn chặn scope creep
5. **Bỏ qua phụ thuộc và rủi ro**: Xác định và lập kế hoạch trước
6. **Viết cho bản thân, không phải cho đối tượng**: Làm cho dễ tìm thông tin
7. **Tường văn bản**: Chia nhỏ với bullet points, bảng, tiêu đề
8. **Không có User Stories**: Giữ tập trung vào nhu cầu người dùng
9. **Quên trường hợp biên**: Nơi lỗi sống
10. **Đặt và quên**: PRD là tài liệu sống và hồ sơ lịch sử
11. **Không có tiêu chí chấp nhận**: Định nghĩa rõ ràng về "hoàn thành"
12. **Bỏ qua yêu cầu phi chức năng**: Hiệu suất, bảo mật, khả năng truy cập cũng quan trọng

---

## PRD Template / Mẫu PRD

**English:**

Use this template as a starting point for your PRDs. Customize based on your project's needs.

```markdown
# PRD: [Feature Name]

**Version**: 1.0
**Last Updated**: [Date]
**Status**: Draft | In Review | Approved | Implemented
**Owner**: [Product Manager Name]
**Contributors**: [Engineering Lead, Design Lead, etc.]

---

## TL;DR (Quick Summary)

[One paragraph: What are we building, why, and what's the expected impact?]

**For Engineers**: See sections [5, 8, 9]
**For Designers**: See sections [4, 7]
**For Leadership**: See sections [1, 3, 11]

---

## 1. Executive Summary

**What are we building?**
[One-sentence description]

**Why are we building it?**
[Problem statement in 1-2 sentences]

**Expected impact:**
[Key metric: X% improvement in Y]

**Timeline:**
[Target launch date]

---

## 2. Problem Statement

**Current Situation:**
[Describe the current state]

**Who is Affected:**
[User personas, segments, number of users]

**Impact:**
- **User Impact**: [How users are affected]
- **Business Impact**: [How business is affected]

**Evidence:**
- [Data point 1: analytics, research, support tickets]
- [Data point 2]
- [Data point 3]

**What Happens if We Don't Solve This:**
[Consequences of inaction]

---

## 3. Goals & Success Metrics

### Business Goals
1. [Goal 1]
2. [Goal 2]
3. [Goal 3]

### Success Metrics

| Metric | Baseline | Target | Timeline | Measurement |
|--------|----------|--------|----------|-------------|
| [Metric 1] | [Current] | [Target] | [When] | [How measured] |
| [Metric 2] | [Current] | [Target] | [When] | [How measured] |
| [Metric 3] | [Current] | [Target] | [When] | [How measured] |

### Leading Indicators (Early Signals)
- [Indicator 1: What to watch in first week]
- [Indicator 2: What to watch in first month]

### Lagging Indicators (Long-term Results)
- [Indicator 1: What to measure at 3 months]
- [Indicator 2: What to measure at 6 months]

---

## 4. Target Users & User Stories

### Primary Persona: [Name]
- **Role**: [Job title]
- **Background**: [Experience, context]
- **Pain Points**:
  - [Pain 1]
  - [Pain 2]
- **Goals**:
  - [Goal 1]
  - [Goal 2]

### User Stories

**Story 1:**
> As a [type of user], I want [action], so that [benefit].

**Acceptance Criteria:**
- [ ] [Criteria 1]
- [ ] [Criteria 2]

**Priority**: P0 | P1 | P2
**Estimate**: [Time estimate]

---

## 5. Requirements & Specifications

### Functional Requirements (What it does)

**Must-Have (P0):**
- **FR-1**: [Requirement description]
  - [Detail 1]
  - [Detail 2]
  - Acceptance: [How to verify]

**Should-Have (P1):**
- **FR-X**: [Requirement description]

**Nice-to-Have (P2):**
- **FR-Y**: [Requirement description]

### Non-Functional Requirements (How well it does it)

- **NFR-1**: Performance - [Specific requirement]
- **NFR-2**: Security - [Specific requirement]
- **NFR-3**: Accessibility - [Specific requirement]
- **NFR-4**: Scalability - [Specific requirement]

### Design Requirements (How it looks/feels)

- **DR-1**: [Visual requirement]
- **DR-2**: [Interaction requirement]
- **DR-3**: [Responsive requirement]

---

## 6. Out of Scope

**Explicitly NOT included in this version:**
- ❌ [Feature 1] - Reason: [Why excluded]
- ❌ [Feature 2] - Reason: [Why excluded]
- ❌ [Feature 3] - Reason: [Why excluded]

**Future Considerations (v2.0):**
- [Feature that might come later]

---

## 7. User Experience & Design

### User Flow

```
[Start State]
   ↓ [Action 1]
[State 2]
   ↓ [Action 2]
[End State]
```

### Key Screens/Pages
- **Screen 1**: [Description] - [Link to design]
- **Screen 2**: [Description] - [Link to design]

### Edge Cases
- **Case 1**: [Scenario] → [How system handles it]
- **Case 2**: [Scenario] → [How system handles it]

### Error States
- **Error 1**: [When it happens] → [What user sees]
- **Error 2**: [When it happens] → [What user sees]

---

## 8. Dependencies & Blockers

### Dependencies (Must happen first)

| Dependency | Owner | Status | Due Date | Impact if Delayed |
|------------|-------|--------|----------|-------------------|
| [Dependency 1] | [Team] | [Status] | [Date] | [Impact] |
| [Dependency 2] | [Team] | [Status] | [Date] | [Impact] |

### Blockers (Currently blocked on)

| Blocker | Description | Owner | Resolution Plan |
|---------|-------------|-------|-----------------|
| [Blocker 1] | [Details] | [Who] | [How to unblock] |

---

## 9. Risks & Mitigation

| Risk | Likelihood | Impact | Mitigation | Owner |
|------|-----------|--------|------------|-------|
| [Risk 1] | H/M/L | H/M/L | [Plan] | [Who] |
| [Risk 2] | H/M/L | H/M/L | [Plan] | [Who] |

---

## 10. Implementation Plan

### Phase 1: [Name] (Duration)
**Goal**: [What this phase achieves]

**Deliverables:**
- [ ] [Deliverable 1]
- [ ] [Deliverable 2]

**Team**: [Who's involved]

### Phase 2: [Name] (Duration)
[Same structure]

### Phase 3: Launch (Duration)
[Same structure]

---

## 11. Launch & Rollout Plan

### Pre-Launch Checklist
- [ ] All P0 requirements implemented
- [ ] Passes QA testing
- [ ] Accessibility audit complete
- [ ] Performance testing complete
- [ ] Documentation updated
- [ ] Stakeholder sign-offs

### Rollout Strategy

**Week 1**: Internal dogfooding
- Target: Company employees
- Size: [Number]

**Week 2**: Beta testing
- Target: [Segment]
- Size: [Percentage]

**Week 3**: Gradual rollout
- Day 1: 25% of users
- Day 3: 50% of users
- Day 5: 100% of users

**Rollback Plan:**
- Feature flag: Can disable in <5 minutes
- Rollback criteria: [When to roll back]

### Communication Plan
- [ ] In-app announcement
- [ ] Email to users
- [ ] Blog post
- [ ] Social media
- [ ] Customer success team briefing

---

## 12. Success Criteria & Validation

### Launch Criteria (Can we ship?)
- [ ] [Criteria 1]
- [ ] [Criteria 2]
- [ ] [Criteria 3]

### Acceptance Criteria (Is it done?)
- [ ] [Criteria 1]
- [ ] [Criteria 2]
- [ ] [Criteria 3]

### Post-Launch Monitoring

**Daily (First Week):**
- Error rates
- Performance metrics
- User feedback

**Weekly (First Month):**
- Adoption rate
- Usage patterns
- Success metrics progress

**Monthly (First Quarter):**
- Impact on business goals
- User satisfaction (NPS, surveys)
- ROI analysis

---

## 13. Open Questions & Assumptions

### Open Questions
- **Q1**: [Question that needs an answer]
  - Owner: [Who will answer]
  - Due: [When answer needed]

- **Q2**: [Question]

### Assumptions
- **A1**: [Assumption being made]
  - Validation: [How to validate]

- **A2**: [Assumption]

---

## 14. Stakeholders & Approvals

| Role | Name | Responsibility | Approval Status |
|------|------|---------------|-----------------|
| Product Manager | [Name] | Overall ownership | ✅ Approved |
| Engineering Lead | [Name] | Technical feasibility | ⏳ Pending |
| Design Lead | [Name] | UX/UI design | ⏳ Pending |
| Business Stakeholder | [Name] | Business alignment | ⏳ Pending |

---

## 15. Related Documents

- 🎨 **Designs**: [Link to Figma/Sketch]
- 🏗️ **Technical Spec**: [Link to tech doc]
- 📊 **User Research**: [Link to research]
- 🚀 **Launch Checklist**: [Link to checklist]
- 📈 **Analytics Dashboard**: [Link to dashboard]
- 🔗 **Related PRDs**: [Links to dependent PRDs]

---

## Version History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | [Date] | [Name] | Initial PRD |
| 1.1 | [Date] | [Name] | [What changed] |

```

**Vietnamese:**

Sử dụng mẫu này làm điểm khởi đầu cho PRD của bạn. Tùy chỉnh dựa trên nhu cầu dự án của bạn.

---

## Real-World Examples / Ví Dụ Thực Tế

**English:**

### Example 1: Slack Threads Feature

**Problem:**
> "In busy channels with 100+ messages/day, important conversations get lost. Users spend 15 minutes/day scrolling to find context. Support tickets: 1,200/month about 'can't find message.'"

**Solution:**
> "Add threading: Users can reply to specific messages, creating organized sub-conversations."

**Success Metrics:**
| Metric | Baseline | Target | Actual (3 months) |
|--------|----------|--------|-------------------|
| Support tickets | 1,200/mo | 700/mo | 650/mo ✅ |
| Time to find message | 15 min/day | 5 min/day | 6 min/day ✅ |
| Message organization | 40% | 70% | 75% ✅ |

**Key Requirement:**
> "FR-1: User can click 'Reply in thread' on any message. Thread opens in side panel. Original message stays in main channel with '3 replies' indicator."

**Result:** Threads became one of Slack's most-used features, reducing support costs by 46% and improving user satisfaction by 35%.

---

### Example 2: Amazon 1-Click Ordering

**Problem:**
> "Checkout takes 6 steps, 3 minutes average. 28% of users abandon cart before completing purchase. Lost revenue: $2.4M/month."

**Solution:**
> "One-click ordering: Save payment/shipping info, enable purchase with one click."

**Success Metrics:**
| Metric | Baseline | Target | Actual (6 months) |
|--------|----------|--------|-------------------|
| Checkout time | 3 min | 10 sec | 12 sec ✅ |
| Cart abandonment | 28% | 15% | 14% ✅ |
| Revenue impact | $0 | +$1M/mo | +$2.8M/mo ✅ |

**Key Requirement:**
> "FR-1: If user has saved payment + shipping, show '1-Click Order' button. Click button → Order placed immediately. Confirmation email sent within 1 minute."

**Result:** So valuable Amazon patented it. Billions in increased revenue. Became industry standard.

---

### Example 3: Spotify Wrapped

**Problem:**
> "User engagement drops 40% in Q4. Churn increases 12% in December. Users forget they use Spotify regularly."

**Solution:**
> "Wrapped: Personalized year-end summary of listening habits. Shareable on social media."

**Success Metrics:**
| Metric | Baseline | Target | Actual (First Year) |
|--------|----------|--------|---------------------|
| Q4 engagement | -40% | -20% | +15% ✅ |
| Social shares | 0 | 1M | 60M ✅ |
| App downloads | 2M/mo | 3M/mo | 8M/mo ✅ |
| Churn reduction | 12% | 6% | 3% ✅ |

**Key Requirement:**
> "FR-1: Generate personalized summary (top artists, songs, genres, total minutes). FR-2: Animated shareable graphics. FR-3: Available Dec 1-31."

**Result:** Wrapped became viral marketing phenomenon. 60M+ social shares. One of Spotify's most anticipated annual features.

---

### Example 4: Root PRD Generation

**Problem:**
> "PMs spend 8 hours writing PRDs from scratch. No consistent format across team. 40% of PRDs missing critical sections (success metrics, out-of-scope). Engineers frequently ask clarifying questions."

**Solution:**
> "AI-powered PRD generation: `/phase3:prd` command generates comprehensive PRD from brief description."

**Success Metrics:**
| Metric | Baseline | Target |
|--------|----------|--------|
| PRD creation time | 8 hours | 3 hours |
| PRD completeness | 60% | 95% |
| Clarifying questions | 15/PRD | 5/PRD |
| PM satisfaction | 6/10 | 8/10 |

**Key Requirements:**
- **FR-1**: User runs `/phase3:prd "Feature description"`
- **FR-2**: AI generates PRD with all standard sections
- **FR-3**: PRD follows industry best practices
- **FR-4**: Output in markdown with YAML frontmatter
- **FR-5**: Includes Root-specific examples

**Implementation:**
```
/phase3:prd "Dark mode feature for evening users"

Generated PRD includes:
1. Executive Summary: What we're building
2. Problem Statement: Eye strain for 18K evening users
3. Success Metrics: 40% adoption, 60% fewer tickets
4. User Stories: 3 personas with acceptance criteria
5. Requirements: 12 functional + 4 non-functional
6. Out of Scope: Custom themes, marketing site
7. Dependencies: Design system, feature flags
8. Implementation Plan: 3 phases, 6 weeks
9. Launch Plan: Beta → gradual rollout
10. All sections complete and ready for review
```

**Expected Impact:**
- Saves 5 hours per PRD
- Ensures consistency across team
- Reduces back-and-forth with stakeholders
- Improves engineering/design handoffs

**Vietnamese:**

### Ví Dụ 1: Tính Năng Threads Của Slack
- **Vấn đề**: Tin nhắn quan trọng bị lạc trong các kênh đông đúc
- **Giải pháp**: Thêm threading để tổ chức cuộc trò chuyện phụ
- **Kết quả**: Giảm 46% chi phí hỗ trợ, tăng 35% sự hài lòng

### Ví Dụ 2: 1-Click Ordering Của Amazon
- **Vấn đề**: Thanh toán mất 3 phút, 28% bỏ giỏ hàng
- **Giải pháp**: Đặt hàng một cú nhấp chuột
- **Kết quả**: Tăng hàng tỷ đô la doanh thu, trở thành tiêu chuẩn ngành

### Ví Dụ 3: Spotify Wrapped
- **Vấn đề**: Tương tác giảm 40% trong Q4
- **Giải pháp**: Tóm tắt năm cá nhân hóa có thể chia sẻ
- **Kết quả**: 60M+ chia sẻ xã hội, tăng 15% tương tác Q4

### Ví Dụ 4: Tạo PRD Của Root
- **Vấn đề**: PM dành 8 giờ viết PRD, thiếu tính nhất quán
- **Giải pháp**: Tạo PRD bằng AI với lệnh `/phase3:prd`
- **Kết quả mong đợi**: Tiết kiệm 5 giờ/PRD, đảm bảo tính nhất quán

---

## Integration with Root / Tích Hợp Với Root

**English:**

### How to Use PRDs in Root Workflow

PRDs fit into Phase 3 of Root's capability toolkit:

**Phase 1: Capture Ideas**
- `/phase1:idea` - Capture raw ideas

**Phase 2: Prioritize**
- `/phase2:rice` - Score ideas
- `/phase2:ice` - Quick prioritization

**Phase 3: Document & Plan** ← PRDs live here
- `/phase3:prd` - Generate comprehensive PRD
- `/phase3:spec` - Technical specifications
- `/phase3:stories` - User stories

**Phase 4: Execute**
- `/phase4:sprint` - Sprint planning
- `/phase4:status` - Track progress

**Phase 5: Launch**
- `/phase5:checklist` - Launch checklist
- `/phase5:release-notes` - Release notes

**Phase 6: Measure**
- `/phase6:metrics` - Track success metrics
- `/phase6:retro` - Retrospective

**Phase 7: Learn**
- `/phase7:insights` - Analyze learnings
- `/phase7:iterate` - Plan iterations

### Example Workflow

```
1. Capture idea:
   /phase1:idea "Dark mode for evening users"
   → Creates IDEA-024

2. Prioritize:
   /phase2:rice IDEA-024
   → RICE Score: 850 (High priority)

3. Create PRD:
   /phase3:prd IDEA-024
   → Generates comprehensive PRD-024
   → Includes all standard sections
   → Ready for stakeholder review

4. Get approval:
   → Share PRD-024 with engineering, design, leadership
   → Iterate based on feedback
   → Get sign-offs

5. Plan execution:
   /phase4:sprint PRD-024
   → Creates sprint tasks
   → Assigns to team

6. Track progress:
   /phase4:status PRD-024
   → See implementation status

7. Launch:
   /phase5:checklist PRD-024
   → Launch checklist
   → Release notes

8. Measure:
   /phase6:metrics PRD-024
   → Track success metrics from PRD
   → Compare actual vs. target

9. Learn:
   /phase7:retro PRD-024
   → What worked / didn't work
   → Lessons for next time
```

### PRD Metadata for Root

Every PRD generated by Root includes YAML frontmatter for traceability:

```yaml
---
# PRD Metadata
prd_id: "PRD-024"
title: "Dark Mode Feature"
status: "Draft"
created_date: "2025-01-15"
owner: "Sarah Chen"
priority: "P0"

# Traceability
source_idea: "IDEA-024"
rice_score: 850
related_prds: ["PRD-012", "PRD-018"]

# Stakeholders
engineering_lead: "Mike Johnson"
design_lead: "Lisa Park"
business_owner: "Tom Wilson"

# Timeline
target_launch: "2025-03-15"
estimated_effort: "6 weeks"

# Metrics
primary_metric: "Dark mode adoption rate"
target_value: "40%"
measurement_timeline: "6 months"
---
```

### Benefits of Root PRD Generation

1. **Speed**: 8 hours → 3 hours (saves 5 hours per PRD)
2. **Completeness**: AI ensures all standard sections included
3. **Consistency**: Same format across all PRDs
4. **Best Practices**: Built-in industry standards
5. **Traceability**: Links to ideas, RICE scores, launches
6. **Collaboration**: Easy to share and iterate
7. **Learning**: Examples and templates built-in

**Vietnamese:**

### Cách Sử Dụng PRD Trong Quy Trình Root

PRD phù hợp với Giai đoạn 3 của bộ công cụ năng lực Root:

- **Giai đoạn 1: Thu thập ý tưởng** → `/phase1:idea`
- **Giai đoạn 2: Ưu tiên** → `/phase2:rice`, `/phase2:ice`
- **Giai đoạn 3: Ghi chép & Lập kế hoạch** ← PRD ở đây → `/phase3:prd`
- **Giai đoạn 4: Thực thi** → `/phase4:sprint`, `/phase4:status`
- **Giai đoạn 5: Ra mắt** → `/phase5:checklist`
- **Giai đoạn 6: Đo lường** → `/phase6:metrics`
- **Giai đoạn 7: Học hỏi** → `/phase7:retro`

---

## Quick Reference / Tham Khảo Nhanh

**English:**

### PRD Checklist

Use this checklist to ensure your PRD is complete:

**Essential Sections:**
- [ ] Executive Summary (30-second pitch)
- [ ] Problem Statement (with data)
- [ ] Goals & Success Metrics (specific, measurable)
- [ ] Target Users & User Stories
- [ ] Requirements (functional, non-functional, design)
- [ ] Out of Scope (explicitly stated)
- [ ] Dependencies & Risks
- [ ] Implementation Plan
- [ ] Launch Plan
- [ ] Success Criteria

**Quality Checks:**
- [ ] All requirements have priorities (P0, P1, P2)
- [ ] Success metrics are specific and measurable
- [ ] User stories include acceptance criteria
- [ ] Edge cases documented
- [ ] Stakeholders identified and assigned
- [ ] Timeline is realistic
- [ ] Links to related documents included
- [ ] Reviewed by engineering, design, stakeholders
- [ ] Approved by all stakeholders

**Before Sharing:**
- [ ] Spell check and grammar check
- [ ] Formatting is clean and scannable
- [ ] Images/diagrams are clear
- [ ] No confidential information (if sharing externally)
- [ ] Version number updated
- [ ] Table of contents (for long PRDs)

### PRD in One Page

For executives who need the summary:

```
# PRD: [Feature Name]

**TL;DR**: [One sentence: what, why, impact]

**Problem**: [2 sentences: current pain, who affected]

**Solution**: [2 sentences: what we're building]

**Success**: [3 key metrics with targets]

**Timeline**: [Target launch date]

**Risk**: [Biggest risk + mitigation]

**Need**: [Any decisions/resources needed]

**Full PRD**: [Link to complete document]
```

### Common PRD Sections by Stakeholder

**Engineering Needs:**
- Requirements & Specifications
- Technical Constraints
- Dependencies
- Implementation Plan
- Acceptance Criteria

**Design Needs:**
- User Stories
- User Experience & Design
- Design Requirements
- Acceptance Criteria
- Edge Cases

**Leadership Needs:**
- Executive Summary
- Goals & Success Metrics
- Timeline
- Risks
- Resource Needs

**QA/Testing Needs:**
- Requirements
- Acceptance Criteria
- Edge Cases
- Test Scenarios
- Success Criteria

**Vietnamese:**

### Checklist PRD

- [ ] Các phần thiết yếu: Tóm tắt, Vấn đề, Mục tiêu, User Stories, Yêu cầu, Ngoài phạm vi, Phụ thuộc, Kế hoạch
- [ ] Kiểm tra chất lượng: Ưu tiên, Chỉ số, Tiêu chí chấp nhận, Trường hợp biên
- [ ] Trước khi chia sẻ: Chính tả, Định dạng, Hình ảnh, Phiên bản

---

## Summary / Tóm Tắt

**English:**

A Product Requirements Document (PRD) is the recipe for building features. It aligns everyone (engineering, design, stakeholders) on what to build and why. A great PRD:

**Answers 3 Questions:**
1. Why are we building this? (Problem + Goals)
2. What exactly are we building? (Requirements)
3. How will we know it's successful? (Success Metrics)

**Standard Structure:**
1. Executive Summary
2. Problem Statement
3. Goals & Success Metrics
4. User Stories
5. Requirements (functional, non-functional, design)
6. Out of Scope
7. Dependencies & Risks
8. Implementation Plan
9. Launch Plan
10. Success Criteria

**Best Practices:**
- Use data, not opinions
- Be specific and measurable
- Prioritize ruthlessly (P0, P1, P2)
- Include visuals (flows, wireframes)
- Document decisions and rationale
- Keep it updated (living document)
- Get feedback early and often

**Common Mistakes to Avoid:**
- Solution disguised as problem
- Vague success metrics
- Missing priorities
- No out-of-scope section
- Ignoring dependencies and risks
- Writing for yourself, not your audience
- Walls of text
- No user stories
- Forgetting edge cases
- Set it and forget it

**Time Investment:**
- Draft 1: 4 hours (problem, goals, user stories)
- Draft 2: 2 hours (requirements, dependencies)
- Draft 3: 2 hours (implementation, launch plan)
- Total: 4-8 hours (saves 40% of development time)

**ROI:**
- Prevents rework (30-50% of dev time saved)
- Reduces meetings (60% fewer)
- Increases launch success (35% → 70%)
- Improves team morale
- Creates institutional knowledge

**Root Integration:**
Use `/phase3:prd` to generate comprehensive PRDs in 3 hours instead of 8. Includes all standard sections, best practices, and traceability to ideas and RICE scores.

**Vietnamese:**

Tài Liệu Yêu Cầu Sản Phẩm (PRD) là công thức để xây dựng tính năng. Nó giúp mọi người (kỹ thuật, thiết kế, các bên liên quan) đồng thuận về cần xây dựng gì và tại sao.

**PRD Tốt Trả Lời 3 Câu Hỏi:**
1. Tại sao chúng ta xây dựng điều này? (Vấn đề + Mục tiêu)
2. Chính xác chúng ta đang xây dựng gì? (Yêu cầu)
3. Làm thế nào để biết nó thành công? (Chỉ số thành công)

**Cấu Trúc Chuẩn:** 10 phần chính từ Tóm tắt đến Tiêu chí thành công

**Thực Hành Tốt Nhất:** Sử dụng dữ liệu, cụ thể, ưu tiên, hình ảnh, ghi chép quyết định, cập nhật, nhận phản hồi

**Lỗi Thường Gặp:** Giải pháp thay vì vấn đề, chỉ số mơ hồ, thiếu ưu tiên, không có ngoài phạm vi, bỏ qua phụ thuộc

**Đầu Tư Thời Gian:** 4-8 giờ (tiết kiệm 40% thời gian phát triển)

**ROI:** Ngăn chặn làm lại (30-50%), giảm cuộc họp (60%), tăng thành công ra mắt (35% → 70%)

**Tích Hợp Root:** Sử dụng `/phase3:prd` để tạo PRD toàn diện trong 3 giờ thay vì 8 giờ.

---

**Related Frameworks**: User Stories, Agile, Technical Specs, RICE Prioritization, MoSCoW

**When to Use**: When documenting features for engineering/design, or getting stakeholder alignment before building

**Root Command**: `/phase3:prd [idea-id or description]`

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
