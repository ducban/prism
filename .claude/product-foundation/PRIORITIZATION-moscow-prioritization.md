---
# Core Metadata
title: "MoSCoW Prioritization"
title_vi: "Ưu Tiên MoSCoW"
framework_type: "Prioritization"
category: ["Product Management", "Prioritization", "Requirements"]

# Origin & Authority
author: "Dai Clegg"
organization: "Oracle"
year_developed: "1994"
original_source: "DSDM Consortium"

# Root Integration
root_phase: ["Phase 2: Prioritize & Decide"]
root_commands: ["/phase2:moscow"]
when_to_use: "When working with stakeholders on release planning, or need clear must-haves vs nice-to-haves"

# Difficulty & Time
complexity: "Low"
estimated_time: "2-4 hours per release"
skill_level: "Beginner"

# Classification
tags: ["prioritization", "requirements", "release-planning", "stakeholder-alignment", "simple"]
related_frameworks: ["RICE Prioritization", "ICE Scoring", "Kano Model"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-20"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Article"
    title: "MoSCoW Prioritization Method"
    url: "https://www.productplan.com/glossary/moscow-prioritization/"
    author: "ProductPlan"
    year: "2024"
  - type: "Article"
    title: "How to Use the MoSCoW Method"
    url: "https://www.agilebusiness.org/page/ProjectFramework_10_MoSCoWPrioritisation"
    author: "Agile Business Consortium"
    year: "2014"
  - type: "Tool"
    title: "MoSCoW Template"
    url: "https://miro.com/templates/moscow-matrix/"
    author: "Miro"
    year: "2024"
---

# MoSCoW Prioritization / Ưu Tiên MoSCoW

## Overview / Tổng Quan

**English:**
MoSCoW helps you categorize features into 4 buckets. Think of packing for a trip.

**Categories:**
- **Must Have**: Passport, tickets (can't travel without)
- **Should Have**: Phone charger (really need it)
- **Could Have**: Book to read (nice to have)
- **Won't Have**: Entire wardrobe (leave it behind)

**Real example - Tesla Model 3 launch:**
- **Must Have**: Autopilot, electric powertrain, safety features
- **Should Have**: Premium interior, long-range battery
- **Could Have**: Performance upgrade package
- **Won't Have**: Full self-driving (saved for later versions)

This helped Tesla ship on time by focusing on essentials first.

---

**Vietnamese:**
MoSCoW giúp bạn phân loại tính năng thành 4 nhóm. Hãy nghĩ về việc chuẩn bị hành lý cho chuyến đi.

**Các danh mục:**
- **Must Have (Phải có)**: Hộ chiếu, vé máy bay (không thể đi du lịch nếu thiếu)
- **Should Have (Nên có)**: Sạc điện thoại (thực sự cần)
- **Could Have (Có thể có)**: Sách để đọc (tốt nếu có)
- **Won't Have (Không có)**: Toàn bộ tủ quần áo (để lại)

**Ví dụ thực tế - Ra mắt Tesla Model 3:**
- **Phải có**: Autopilot, hệ thống điện, tính năng an toàn
- **Nên có**: Nội thất cao cấp, pin tầm xa
- **Có thể có**: Gói nâng cấp hiệu suất
- **Không có**: Tự lái hoàn toàn (để dành cho phiên bản sau)

Điều này giúp Tesla giao hàng đúng hạn bằng cách tập trung vào những thứ thiết yếu trước.

---

## MoSCoW Prioritization Playbook / Hướng Dẫn Ưu Tiên MoSCoW

**English:**

MoSCoW is a classification framework, not a scoring system. Use it to categorize features into 4 buckets based on necessity.

### Category 1: Must Have (Phải có)

**Definition**: Features without which the product/release is useless or non-viable.

**How to Identify**:
Ask: "Can we ship without this?"
- If answer is NO → Must Have
- If answer is YES → Not Must Have

**Criteria**:
- ✅ **Critical functionality**: Core purpose of product depends on it
- ✅ **Legal/Regulatory**: Required by law or compliance
- ✅ **Security**: Major security vulnerability if missing
- ✅ **Blocking issue**: Prevents users from basic tasks

**Examples for Root**:
| Feature | Why Must Have |
|---------|---------------|
| Core slash commands for Phase 1-3 | Product is unusable without ability to capture, prioritize, document |
| Argument handling | Without this, commands don't work at all |
| Basic data storage | Need to save user data somewhere |
| Multi-platform support (core platforms) | Product definition requires it |

**Common Mistakes**:
- ❌ "This would be really nice" ≠ Must Have
- ❌ "CEO wants this" ≠ Must Have (unless truly essential)
- ❌ "We promised customers" ≠ Must Have (unless contractual)

**Rule of Thumb**: Only 20-30% of features should be Must Have. If everything is Must Have, you're not prioritizing.

---

### Category 2: Should Have (Nên có)

**Definition**: Important features that add significant value, but product can launch without them (with workarounds).

**How to Identify**:
Ask: "Can users work around this?"
- If answer is YES (but it's painful) → Should Have
- If answer is NO → Might be Must Have

**Criteria**:
- ✅ **High impact**: Significantly improves user experience
- ✅ **Workaround exists**: Users can achieve goal differently
- ✅ **Important but not critical**: Valuable, but not essential
- ✅ **Planned for soon**: Will add in next release

**Examples for Root**:
| Feature | Why Should Have |
|---------|----------------|
| Phase 4-7 commands (Plan, Track, Launch, Analyze) | Valuable but users can manage without initially |
| Detailed error messages | Important for UX, but basic errors work |
| Command documentation | Helpful but users can learn through trial |
| Export to multiple formats | Nice feature, one format is sufficient initially |

**Rule of Thumb**: 40-50% of features are Should Have. These are your "next iteration" items.

---

### Category 3: Could Have (Có thể có)

**Definition**: Nice-to-have features that improve experience but aren't necessary. Include only if time/budget permits.

**How to Identify**:
Ask: "Will anyone notice if this is missing?"
- If answer is NO or "only power users" → Could Have
- If answer is YES → Might be Should Have

**Criteria**:
- ✅ **Low impact**: Small improvement
- ✅ **Edge cases**: Helps minority of users
- ✅ **Polish**: Makes things prettier/smoother
- ✅ **First to cut**: If running out of time, cut these first

**Examples for Root**:
| Feature | Why Could Have |
|---------|----------------|
| Dark mode | Nice polish, not essential functionality |
| Command aliases | Convenience for power users |
| Advanced filtering | Most users don't need it |
| Custom templates | Default templates work fine |
| Keyboard shortcuts | Mouse/typing works fine |

**Rule of Thumb**: 20-30% of features are Could Have. Add if you have extra time.

---

### Category 4: Won't Have (this time) (Không có lần này)

**Definition**: Features that are out of scope for this release. Not saying never, just not now.

**How to Identify**:
Ask: "Is this aligned with current goals?"
- If answer is NO → Won't Have
- If answer is "nice to have someday" → Won't Have

**Criteria**:
- ✅ **Out of scope**: Not aligned with current objectives
- ✅ **Too complex**: Would delay release significantly
- ✅ **Uncertain value**: Not validated, might be waste
- ✅ **Future consideration**: Good idea for later

**Examples for Root**:
| Feature | Why Won't Have |
|---------|---------------|
| Visual GUI interface | Product is CLI-based by design |
| Real-time collaboration | Too complex, not core value |
| AI-powered prioritization | Interesting but unvalidated |
| Mobile app | Out of scope for v1.0 |
| Integration with 50+ tools | Start with top 5 |

**Rule of Thumb**: 30-40% of initial ideas are Won't Have. Be ruthless - saying NO is important.

---

## Distribution Guidelines / Hướng Dẫn Phân Bổ

### Recommended Distribution / Phân Bổ Khuyến Nghị

Your distribution should roughly be:
- **Must Have**: 20-30%
- **Should Have**: 40-50%
- **Could Have**: 20-30%
- **Won't Have**: (Everything else)

**Warning Signs / Dấu Hiệu Cảnh Báo:**
- ⚠️ If you have too many Must Haves (>40%), you're not prioritizing!
- ⚠️ If you have no Could Haves, you're being too rigid
- ⚠️ If you have no Won't Haves, you haven't said NO enough

---

## How to Use MoSCoW for Root / Cách Sử Dụng MoSCoW cho Root

**Step 1: List All Features**
Write down everything you want to build.

**Step 2: Classify Each Feature**
Put each feature in one of 4 buckets. Be honest.

**Step 3: Check Distribution**
Your distribution should roughly be:
- **Must Have**: 20-30%
- **Should Have**: 40-50%
- **Could Have**: 20-30%
- **Won't Have**: (Everything else)

If you have too many Must Haves, you're not prioritizing!

**Step 4: Build in Order**
1. Build all Must Haves first
2. Then Should Haves (as many as time allows)
3. Then Could Haves (if time remains)
4. Won't Haves → Backlog for next release

**Step 5: Re-evaluate**
As you build, some things may move categories:
- Must Have becomes easy → Add more Should Haves
- Should Have takes too long → Move to Could Have or Won't Have

---

## Complete Example: Root v1.0 Release / Ví Dụ Hoàn Chỉnh: Phát Hành Root v1.0

**Goal**: Ship MVP in 3 months with core PM capabilities

### Must Have (30%)

- ✅ Phase 1 commands (Capture) - 13 commands
- ✅ Phase 2 commands (Prioritize) - RICE, ICE
- ✅ Phase 3 commands (Document) - PRD, specs
- ✅ Data storage (markdown + YAML)
- ✅ Multi-platform support (Claude, Gemini, OpenCode)
- ✅ Basic documentation

### Should Have (45%)

- ✅ Phase 4-7 commands (Plan, Track, Launch, Analyze)
- ✅ Specialized agents for complex tasks
- ✅ iFlow and Factory Droid support
- ✅ Comprehensive examples
- ✅ Error handling and validation

### Could Have (20%)

- ✅ Dark mode
- ✅ Command shortcuts/aliases
- ✅ Export to multiple formats
- ✅ Advanced search/filtering
- ✅ Custom templates

### Won't Have (not in v1.0)

- ❌ Visual GUI
- ❌ Real-time collaboration
- ❌ Mobile apps
- ❌ AI-powered auto-prioritization
- ❌ Integration with 50+ external tools

**Result**: Focus on Must + Should = Ship a valuable product in 3 months!

---

## How to Run a MoSCoW Workshop / Cách Tổ Chức Workshop MoSCoW

### Preparation / Chuẩn Bị

**Before the workshop:**
1. **Gather stakeholders** (PM, Engineering, Design, Business)
2. **Prepare feature list** - all proposed features for the release
3. **Set context** - what's the release goal, timeline, constraints
4. **Create template** - use a whiteboard, Miro, or spreadsheet with 4 columns

**Materials needed:**
- Feature cards or sticky notes
- Whiteboard or digital board (Miro, FigJam)
- Timer (timeboxing is key)
- Distribution guideline reference

---

### Workshop Agenda (2-3 hours)

#### Part 1: Context Setting (15 minutes)
- Share release goals and timeline
- Explain MoSCoW categories
- Establish ground rules ("Must Have means non-negotiable")

#### Part 2: Individual Classification (30 minutes)
- Each stakeholder independently classifies features
- No discussion yet - just initial gut feeling
- Use voting dots or digital tools

#### Part 3: Group Discussion (90 minutes)
- Review each feature where there's disagreement
- Use the "Can we ship without this?" test
- Challenge "Must Haves" aggressively
- Move features until consensus is reached

#### Part 4: Distribution Check (15 minutes)
- Count features in each bucket
- Verify distribution (20-30% Must, 40-50% Should, etc.)
- If distribution is off, re-classify some features

#### Part 5: Commitment (15 minutes)
- Get explicit commitment from engineering on Must Haves
- Agree on "nice-to-have" approach for Should/Could
- Document Won't Haves clearly for stakeholder alignment

---

### Facilitation Tips / Mẹo Điều Phối

**English:**

1. **Be the enforcer of "Must Have"**
   - Challenge every Must Have: "What happens if we don't ship this?"
   - Push back on emotional arguments ("CEO wants it")
   - Focus on objective criteria (legal, blocking, core functionality)

2. **Use timeboxing**
   - Don't spend 20 minutes debating one feature
   - If no consensus in 5 minutes, park it and revisit

3. **Watch for patterns**
   - If someone marks everything "Must Have", call it out
   - If engineering says "Should" and business says "Must", dig deeper

4. **Make it visual**
   - Physical or digital board where everyone can see
   - Use colors: Red (Must), Orange (Should), Yellow (Could), Gray (Won't)

5. **Create parking lot**
   - For features that need more research
   - For debates that can't be resolved quickly

**Vietnamese:**

1. **Làm người thực thi "Phải có"**
   - Thách thức mọi Must Have: "Điều gì xảy ra nếu chúng ta không ship?"
   - Phản đối các lập luận cảm tính ("CEO muốn")
   - Tập trung vào tiêu chí khách quan (pháp lý, chặn, chức năng cốt lõi)

2. **Sử dụng timebox**
   - Đừng dành 20 phút tranh luận một tính năng
   - Nếu không đồng thuận trong 5 phút, gác lại và xem xét lại

3. **Quan sát các mô hình**
   - Nếu ai đó đánh dấu mọi thứ là "Must Have", hãy chỉ ra
   - Nếu engineering nói "Should" và business nói "Must", tìm hiểu sâu hơn

4. **Làm cho nó trực quan**
   - Bảng vật lý hoặc kỹ thuật số mà mọi người có thể nhìn thấy
   - Sử dụng màu: Đỏ (Must), Cam (Should), Vàng (Could), Xám (Won't)

5. **Tạo bãi đỗ**
   - Cho các tính năng cần nghiên cứu thêm
   - Cho các cuộc tranh luận không thể giải quyết nhanh chóng

---

## Common Mistakes / Sai Lầm Thường Gặp

### Mistake 1: Too Many Must Haves

**Problem**: Team marks 80% of features as "Must Have"

**Why it happens**:
- Fear of disappointing stakeholders
- Unclear on what "Must" really means
- Confusing "important" with "critical"

**Solution**:
- Ask: "If we only shipped 5 features, which 5?"
- Use the "Can we ship without this?" test
- Force rank within Must Haves - which would you cut first?

**Example**:
```
Before: 40 Must Haves, 10 Should Haves
After: 12 Must Haves, 28 Should Haves, 10 Could Haves
```

---

### Mistake 2: Confusing "Important" with "Must Have"

**Problem**: High-value features automatically become Must Have

**Why it happens**:
- Stakeholders equate importance with necessity
- Business pressure to include everything

**Solution**:
- Separate value from necessity
- High value + Can ship without = Should Have
- High value + Can't ship without = Must Have

**Example**:
```
Feature: Advanced analytics dashboard
- Value: High (stakeholders love it)
- Necessity: Low (basic metrics work)
- Classification: Should Have, not Must Have
```

---

### Mistake 3: Ignoring Distribution Guidelines

**Problem**: 50% Must, 50% Should, 0% Could/Won't

**Why it happens**:
- Team doesn't want to say "no"
- Fear of under-delivering

**Solution**:
- Enforce distribution guidelines
- If too many Must Haves, force re-classification
- Make Won't Have explicit and visible

**Example**:
```
Initial: 25 Must, 25 Should, 0 Could, 0 Won't
Adjusted: 15 Must, 20 Should, 10 Could, 5 Won't
```

---

### Mistake 4: Not Documenting "Won't Have"

**Problem**: Features removed from scope keep coming back

**Why it happens**:
- Won't Haves not explicitly documented
- Stakeholders forget the decision

**Solution**:
- Document Won't Haves clearly
- Include rationale for each
- Share with all stakeholders
- Reference during scope creep discussions

**Example Won't Have Documentation**:
```
Feature: Real-time collaboration
Category: Won't Have (v1.0)
Reason: Too complex, delays launch by 3 months
Future: Consider for v2.0 if validated need
Decided by: Product team, 2024-11-15
```

---

### Mistake 5: Treating MoSCoW as Static

**Problem**: Initial classification never changes

**Why it happens**:
- Team treats it as one-time exercise
- Fear of looking indecisive

**Solution**:
- Review weekly during development
- Move features as you learn more
- Easy Must Have? Add more Should Haves
- Hard Should Have? Move to Could/Won't

**Example**:
```
Week 1: Feature X = Must Have
Week 3: Discover it's easier than expected (done in 2 days)
Week 4: Move 2 Should Haves → Must Have
Result: Ship more value in same time
```

---

### Mistake 6: HiPPO (Highest Paid Person's Opinion) Syndrome

**Problem**: CEO/VP opinion overrides logical classification

**Why it happens**:
- Power dynamics in the room
- Fear of pushing back on leadership

**Solution**:
- Establish criteria before workshop
- Use objective tests ("Can we ship without?")
- Have leadership commit to framework upfront
- PM role: Be the gatekeeper

**Example**:
```
CEO: "This feature is Must Have"
PM: "Let's test it: Can we ship without?"
CEO: "Yes, but customers will love it"
PM: "Then it's Should Have - high value but not blocking"
Result: CEO agrees, feature moves to Should Have
```

---

### Mistake 7: Ignoring Technical Dependencies

**Problem**: Must Haves depend on Won't Haves

**Why it happens**:
- Classification without technical review
- Business-led prioritization only

**Solution**:
- Include engineering in workshop
- Map dependencies before finalizing
- If Must Have needs Won't Have, re-classify

**Example**:
```
Feature A: Social sharing (Must Have)
Feature B: User authentication (Won't Have)
Problem: Can't share without auth
Solution: Move social sharing to Won't Have OR auth to Must Have
```

---

## When to Use MoSCoW / Khi Nào Sử Dụng MoSCoW

### Best Use Cases / Trường Hợp Sử Dụng Tốt Nhất

**English:**

1. **Release planning** - Deciding what goes in next release
2. **Scope management** - When features > capacity
3. **Stakeholder alignment** - Multiple opinions on priorities
4. **Time-constrained projects** - Fixed deadline, need to cut scope
5. **MVP definition** - What's truly minimum for viable?

**Use MoSCoW when:**
- ✅ Clear deadline exists
- ✅ Features can be independently classified
- ✅ Team needs simple, understandable framework
- ✅ Stakeholders need to agree on priorities
- ✅ You need to say NO to some features

**Vietnamese:**

1. **Lập kế hoạch phát hành** - Quyết định điều gì trong bản phát hành tiếp theo
2. **Quản lý phạm vi** - Khi tính năng > năng lực
3. **Căn chỉnh bên liên quan** - Nhiều ý kiến về ưu tiên
4. **Dự án hạn chế thời gian** - Thời hạn cố định, cần cắt phạm vi
5. **Định nghĩa MVP** - Điều gì thực sự tối thiểu để khả thi?

**Sử dụng MoSCoW khi:**
- ✅ Thời hạn rõ ràng tồn tại
- ✅ Các tính năng có thể được phân loại độc lập
- ✅ Nhóm cần framework đơn giản, dễ hiểu
- ✅ Các bên liên quan cần đồng ý về ưu tiên
- ✅ Bạn cần nói KHÔNG với một số tính năng

---

### When NOT to Use MoSCoW / Khi KHÔNG Sử Dụng MoSCoW

**Avoid MoSCoW when:**
- ❌ You need precise scoring/ranking (use RICE, ICE instead)
- ❌ Features are highly interdependent
- ❌ You need to optimize for specific metrics
- ❌ Long-term roadmap (use Now-Next-Later instead)
- ❌ Comparing different types of work (features vs bugs vs tech debt)

**Better alternatives:**
- **For scoring**: Use RICE or ICE Scoring
- **For metrics**: Use AARRR or North Star
- **For roadmap**: Use Now-Next-Later
- **For strategy**: Use Opportunity Solution Trees

---

## Related Frameworks / Framework Liên Quan

### 1. RICE Prioritization

**Relationship**: Complementary
- MoSCoW: Qualitative classification (Must/Should/Could/Won't)
- RICE: Quantitative scoring (Reach × Impact × Confidence / Effort)

**How to combine**:
1. Use RICE to score all features
2. Use MoSCoW to classify into buckets
3. High RICE + Business critical = Must Have
4. High RICE + Can work around = Should Have

**Example**:
```
Feature: User authentication
- RICE Score: 85 (high)
- Classification: Must Have (can't ship without)

Feature: Social sharing
- RICE Score: 90 (higher)
- Classification: Should Have (can ship with basic sharing)
```

---

### 2. ICE Scoring

**Relationship**: Complementary
- MoSCoW: What's necessary vs nice-to-have
- ICE: What's impactful and easy

**How to combine**:
1. Score features with ICE
2. Classify high-ICE features with MoSCoW
3. Must Have = High impact, blocks core functionality
4. Should Have = High ICE but not blocking

---

### 3. Kano Model

**Relationship**: Different focus
- MoSCoW: Necessity-based prioritization
- Kano: Satisfaction-based classification

**How to combine**:
- Basic Needs (Kano) → Must Have (MoSCoW)
- Performance Needs (Kano) → Should Have (MoSCoW)
- Delight Features (Kano) → Could Have (MoSCoW)

**Example**:
```
Feature: Core search functionality
- Kano: Basic Need (dissatisfied if missing)
- MoSCoW: Must Have

Feature: Advanced filters
- Kano: Performance Need (satisfied if present)
- MoSCoW: Should Have

Feature: Search animations
- Kano: Delighter (wow factor)
- MoSCoW: Could Have
```

---

### 4. Now-Next-Later Roadmap

**Relationship**: Time-based vs Necessity-based
- MoSCoW: What's critical vs nice-to-have
- Now-Next-Later: When to build it

**How to combine**:
- Must Have → Now (this release)
- Should Have → Next (next 1-2 releases)
- Could Have → Later (future releases)
- Won't Have → Not on roadmap (or far future)

---

## Learning Resources / Tài Nguyên Học Tập

### Articles / Bài Viết

1. **"MoSCoW Prioritization Method"**
   - Author: ProductPlan
   - URL: https://www.productplan.com/glossary/moscow-prioritization/
   - Description: Comprehensive guide to MoSCoW with examples and templates
   - Best for: Understanding fundamentals

2. **"How to Use the MoSCoW Method"**
   - Author: Agile Business Consortium
   - URL: https://www.agilebusiness.org/page/ProjectFramework_10_MoSCoWPrioritisation
   - Description: Official guide from the organization that formalized MoSCoW
   - Best for: In-depth methodology

3. **"MoSCoW Method: A Simple Prioritization Technique"**
   - Author: Mind the Product
   - URL: https://www.mindtheproduct.com/moscow-method-prioritization/
   - Description: Practical application in product management
   - Best for: Real-world examples

---

### Tools / Công Cụ

1. **Miro MoSCoW Template**
   - URL: https://miro.com/templates/moscow-matrix/
   - Description: Interactive template for remote workshops
   - Best for: Distributed teams

2. **Productboard**
   - URL: https://www.productboard.com/
   - Description: Product management tool with MoSCoW support
   - Best for: Large-scale prioritization

3. **Google Sheets Template**
   - Description: Simple spreadsheet with 4 columns
   - Best for: Quick classification without tools

---

### Videos / Video

1. **"MoSCoW Prioritization Explained"**
   - Platform: YouTube
   - Channel: Product School
   - Duration: 10 minutes
   - Best for: Visual learners

2. **"How to Run a MoSCoW Workshop"**
   - Platform: YouTube
   - Channel: Agile Academy
   - Duration: 25 minutes
   - Best for: Facilitation skills

---

### Books / Sách

1. **"The Lean Product Playbook"**
   - Author: Dan Olsen
   - Chapter: Feature Prioritization
   - Description: Includes section on MoSCoW in context of MVP definition
   - Best for: Holistic product approach

2. **"Inspired: How to Create Tech Products Customers Love"**
   - Author: Marty Cagan
   - Description: Discusses prioritization frameworks including MoSCoW
   - Best for: Product leadership perspective

---

## Summary / Tóm Tắt

**English:**

MoSCoW is a simple, effective framework for categorizing features into Must Have, Should Have, Could Have, and Won't Have. It helps teams:
- Ship on time by focusing on essentials
- Align stakeholders on what's truly necessary
- Say NO to nice-to-haves without guilt
- Make release planning transparent and objective

**Key takeaways:**
1. Only 20-30% should be Must Have
2. Use objective criteria: "Can we ship without this?"
3. Challenge every Must Have aggressively
4. Document Won't Haves explicitly
5. Re-evaluate as you learn more

**Best combined with**: RICE for scoring, Kano for satisfaction, Now-Next-Later for roadmaps

---

**Vietnamese:**

MoSCoW là framework đơn giản, hiệu quả để phân loại tính năng thành Must Have, Should Have, Could Have, và Won't Have. Nó giúp teams:
- Ship đúng hạn bằng cách tập trung vào điều cần thiết
- Căn chỉnh các bên liên quan về những gì thực sự cần thiết
- Nói KHÔNG với nice-to-haves mà không cảm thấy tội lỗi
- Làm cho việc lập kế hoạch phát hành minh bạch và khách quan

**Điểm chính:**
1. Chỉ 20-30% nên là Must Have
2. Sử dụng tiêu chí khách quan: "Chúng ta có thể ship mà không có điều này không?"
3. Thách thức mỗi Must Have một cách mạnh mẽ
4. Ghi chép Won't Haves một cách rõ ràng
5. Đánh giá lại khi bạn học thêm

**Kết hợp tốt nhất với**: RICE để tính điểm, Kano để thỏa mãn, Now-Next-Later cho roadmaps

---

## Root Integration / Tích Hợp Root

### Using MoSCoW in Root

**Command**: `/phase2:moscow`

**What it does**:
- Guides you through MoSCoW classification
- Creates structured prioritization document
- Validates distribution (warns if too many Must Haves)
- Generates output for stakeholder review

**Example workflow**:
```bash
# Step 1: Capture all features
/phase1:ideas

# Step 2: Run MoSCoW prioritization
/phase2:moscow

# Step 3: Document in PRD
/phase3:prd

# Step 4: Build Must Haves first
/phase4:sprint-plan
```

---

### Templates Available

1. **MoSCoW Workshop Template** - For facilitation
2. **Distribution Checker** - Validates percentages
3. **Stakeholder Review Doc** - For alignment meetings
4. **Release Plan** - Must + Should Haves for this release

---

## Questions to Reflect / Câu Hỏi Để Suy Ngẫm

**English:**
1. If you had to cut 50% of features, which ones would you cut?
2. What's the smallest set of features that delivers value?
3. Which features are stakeholders most emotionally attached to?
4. Can users achieve their goal without this feature?
5. What happens if we don't ship this feature?

**Vietnamese:**
1. Nếu bạn phải cắt 50% tính năng, bạn sẽ cắt những cái nào?
2. Tập hợp tính năng nhỏ nhất cung cấp giá trị là gì?
3. Các bên liên quan gắn bó cảm xúc nhất với những tính năng nào?
4. Người dùng có thể đạt được mục tiêu của họ mà không có tính năng này không?
5. Điều gì xảy ra nếu chúng ta không ship tính năng này?

---

**Version**: 1.0
**Last Updated**: 2025-11-20
**Status**: Active
**Language**: Bilingual (English/Vietnamese)

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
