---
# Core Metadata
title: "User Story Mapping"
title_vi: "Lập Bản Đồ User Story"
framework_type: "Documentation"
category: ["Product Management", "Documentation", "Planning", "Agile"]

# Origin & Authority
author: "Jeff Patton"
organization: "Independent (Agile Coach)"
year_developed: "2005"
original_source: "User Story Mapping (Book, 2014)"

# Root Integration
root_phase: ["Phase 2: Collaborate & Align", "Phase 3: Document & Plan"]
root_commands: ["/phase2:story-map", "/phase3:plan"]
when_to_use: "When planning features, releases, or understanding user journey through product"

# Difficulty & Time
complexity: "Medium"
estimated_time: "2-4 hours for initial mapping, iterative refinement"
skill_level: "Beginner-Intermediate"

# Classification
tags: ["user-stories", "story-mapping", "agile", "planning", "user-journey", "release-planning"]
related_frameworks: ["Jobs to Be Done", "Product Roadmapping", "Agile/Scrum", "User Journey Map"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-21"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Book"
    title: "User Story Mapping: Discover the Whole Story, Build the Right Product"
    author: "Jeff Patton"
    year: "2014"
  - type: "Article"
    title: "The New User Story Backlog is a Map"
    url: "https://jpattonassociates.com/the-new-backlog/"
    author: "Jeff Patton"
    year: "2008"
  - type: "Video"
    title: "User Story Mapping"
    url: "https://www.youtube.com/watch?v=AorAgSrHjKM"
    author: "Jeff Patton"
    year: "2015"
---

# User Story Mapping / Lập Bản Đồ User Story

## Overview / Tổng Quan

**English:**
User Story Mapping is a collaborative technique for organizing user stories by visualizing the user's journey through your product. Instead of a flat backlog, you create a 2D map showing user activities and tasks.

**The Problem It Solves:**
Traditional backlogs are flat lists—hard to prioritize, see the big picture, or plan releases:
```
Backlog (Traditional):
- As a user, I want to log in
- As a user, I want to search products
- As a user, I want to add to cart
- As a user, I want to check out
- As a user, I want to view order history
(85 more stories...)
```

**What's missing?**
- How do these fit together?
- What's the user flow?
- What's MVP vs future releases?

**User Story Map (Better):**
```
Activities:    Discover → Select → Purchase → Track
                 |         |         |         |
Tasks:        Browse    Add Cart  Checkout   Status
              Search    View Item  Payment    History
              Filter    Compare    Shipping   Refund
                ↓         ↓         ↓         ↓
           (Stories organized by user flow + priority)
```

**Real Example - Airbnb MVP:**

Jeff Patton helped Airbnb in early days create story map:

**Backbone (Activities):**
Find Place → Book → Stay → Review

**Walking Skeleton (MVP - Release 1):**
- Find: Browse listings (no search yet)
- Book: Email host (no instant book)
- Stay: Offline experience
- Review: Email feedback (no rating system)

**Later Releases:**
- Release 2: Search, filters, instant book
- Release 3: Reviews, ratings, profiles
- Release 4: Wish lists, messaging

**Result:** Focused MVP, clear roadmap, successful launch

**Vietnamese:**
User Story Mapping là kỹ thuật tổ chức user stories bằng cách hình dung hóa hành trình người dùng qua sản phẩm.

**Vấn Đề Nó Giải Quyết:**
- Backlog truyền thống là danh sách phẳng - khó ưu tiên
- Story map là bản đồ 2D theo hành trình người dùng

**Ví Dụ - Airbnb MVP:**
- **Hoạt động**: Tìm → Đặt → Ở → Đánh giá
- **MVP**: Browse, email host, offline, email feedback
- **Sau**: Tìm kiếm, instant book, ratings, profiles
- **Kết quả**: MVP tập trung, roadmap rõ ràng

---

## Story Map Structure / Cấu Trúc Story Map

**English:**

### The Anatomy of a Story Map

```
User Activities (Backbone - Horizontal)
────────────────────────────────────────
        ↓           ↓           ↓
User Tasks (Walking Skeleton - Horizontal)
────────────────────────────────────────
        ↓           ↓           ↓
User Stories (Vertical - by Priority)
        ↓           ↓           ↓
    ─────────   ─────────   ─────────
    MVP (R1)    MVP (R1)    MVP (R1)
    ─────────   ─────────   ─────────
    Release 2   Release 2   Release 2
    ─────────   ─────────   ─────────
    Release 3   Release 3   Release 3
    ─────────   ─────────   ─────────
```

### Layer 1: Activities (Top Row)
**What**: High-level user goals (verb + noun)
**Example**: "Plan Trip", "Book Stay", "Experience Stay"
**Characteristics**:
- 5-10 activities max
- Left-to-right = chronological user flow
- Strategic level

### Layer 2: Tasks (Second Row)
**What**: Steps to complete activity
**Example**: Under "Book Stay" → "Select Dates", "Choose Room", "Enter Payment"
**Characteristics**:
- 3-8 tasks per activity
- Still left-to-right flow
- Tactical level

### Layer 3: Stories (Vertical Columns)
**What**: Detailed user stories under each task
**Example**: Under "Select Dates" →
- "As a guest, I want to see calendar..."
- "As a guest, I want to see pricing..."
**Characteristics**:
- Top-to-bottom = priority (high to low)
- Smallest shippable increments
- Execution level

### Release Slicing (Horizontal Cuts)
**What**: Draw horizontal lines to separate releases
**Example**:
- **Above line 1**: MVP (minimum viable product)
- **Between lines 1-2**: Release 2 (nice-to-have)
- **Below line 2**: Release 3+ (future)

**Vietnamese:**

### Cấu Trúc 3 Tầng:

**1. Activities (Hoạt động)**
- Cấp độ cao, mục tiêu người dùng
- 5-10 hoạt động
- Từ trái sang phải

**2. Tasks (Nhiệm vụ)**
- Các bước hoàn thành hoạt động
- 3-8 tasks/hoạt động

**3. Stories (Câu chuyện)**
- Chi tiết dưới mỗi task
- Từ trên xuống = ưu tiên

**Release Cuts**: Đường ngang ngăn cách các phiên bản

---

## Creating a Story Map: Playbook / Tạo Story Map

**English:**

### Step 1: Identify User Persona (15 min)
**Who are you mapping for?**
- Primary user type (e.g., "Sarah - Home Buyer")
- One persona per map (create separate maps for different personas)

**Example - Netflix:**
- Persona 1: New subscriber
- Persona 2: Returning viewer
- (Create 2 separate maps)

### Step 2: Frame the Problem (15 min)
**What job is the user trying to do?**
Use JTBD format: "When [situation], I want to [motivation], so I can [outcome]"

**Example - Uber:**
"When I need to get somewhere quickly, I want to summon a ride, so I can arrive on time without hassle"

### Step 3: Map Activities (30 min)
**Brainstorm high-level steps in user journey**

**Technique: "A day in the life"**
Walk through user's entire experience:
- What do they do first?
- Then what?
- What's the end goal?

**Example - E-commerce:**
```
Activities: Discover → Browse → Evaluate → Purchase → Receive → Use → Support
```

**Write each on sticky note, arrange left-to-right**

### Step 4: Add Tasks (45 min)
**For each activity, break down into tasks**

**Example - "Purchase" activity:**
```
Purchase
  ↓
Add to Cart → Review Cart → Enter Shipping → Enter Payment → Confirm → Receipt
```

**Tips:**
- Keep tasks small (5-15 min to complete)
- Sequence them chronologically
- Don't worry about details yet

### Step 5: Add Stories (60 min)
**Under each task, add detailed user stories**

**Format**: "As a [who], I want to [what], so that [why]"

**Example - Under "Enter Payment":**
- "As a customer, I want to save payment info, so I don't re-enter it"
- "As a customer, I want to see accepted cards, so I know what I can use"
- "As a customer, I want payment security badge, so I feel safe"
- "As a customer, I want to apply promo code, so I get discount"

**Tips:**
- Write on sticky notes
- One story per note
- Include acceptance criteria (back of note)

### Step 6: Prioritize Vertically (30 min)
**Arrange stories top-to-bottom by priority**

**Prioritization Criteria:**
1. **Must-have** (top): Without it, user can't complete job
2. **Should-have** (middle): Improves experience significantly
3. **Nice-to-have** (bottom): Delighters, but not critical

**Technique: Dot Voting**
- Give each person 5 dots
- Vote on most important stories
- Arrange by votes

### Step 7: Slice for Releases (45 min)
**Draw horizontal lines to define releases**

**Release 1 (MVP): Walking Skeleton**
- Bare minimum to complete user journey end-to-end
- Functional but not polished
- Goal: Validate value proposition

**Release 2: Enhanced Experience**
- Improve usability
- Add convenience features
- Fix obvious pain points

**Release 3+: Optimization & Delight**
- Advanced features
- Personalization
- Delighters

**Example - Notion (Early Releases):**

**MVP (2016):**
- Create text blocks
- Nest pages
- Basic markdown
- Share link (view-only)

**Release 2 (2017):**
- Templates
- Databases
- Real-time collaboration
- Comments

**Release 3 (2018+):**
- Advanced databases
- API
- Integrations
- Mobile apps

### Step 8: Document & Digitize (30 min)
**Capture the map**

**Tools:**
- **Physical**: Photo of sticky notes
- **Digital**: Miro, Mural, StoriesOnBoard, Jira Advanced Roadmaps
- **Spreadsheet**: Google Sheets (simple but works)

**Example Digital Format:**
```
| Activity 1 | Activity 2 | Activity 3 |
|------------|------------|------------|
| Task 1.1   | Task 2.1   | Task 3.1   |
| - Story R1 | - Story R1 | - Story R1 |
| - Story R2 | - Story R2 | - Story R2 |
| - Story R3 | - Story R3 | - Story R3 |
```

**Vietnamese:**

### Quy Trình 8 Bước:

1. **Xác Định Persona** (15 phút): Bạn đang map cho ai?
2. **Định Khung Vấn Đề** (15 phút): Công việc người dùng muốn làm?
3. **Map Activities** (30 phút): Các bước cấp cao
4. **Thêm Tasks** (45 phút): Chia nhỏ hoạt động
5. **Thêm Stories** (60 phút): Chi tiết dưới mỗi task
6. **Ưu Tiên** (30 phút): Sắp xếp từ trên xuống
7. **Chia Releases** (45 phút): Đường ngang ngăn phiên bản
8. **Lưu Trữ** (30 phút): Chụp ảnh hoặc số hóa

**Tổng Thời Gian**: 4-5 giờ (workshop team)

---

## Real Examples / Ví Dụ Thực Tế

### Example 1: Spotify - Personalized Playlists

**Persona**: Music lover who wants personalized recommendations

**Story Map:**
```
Activities:  Discover Music → Listen → Organize → Share

Tasks:
Discover:
  - See recommendations
  - Browse genres
  - Search artists
    ↓ (Stories)
    R1: Daily Mix (basic algo)
    R2: Discover Weekly (ML-powered)
    R3: Release Radar (new releases)

Listen:
  - Play song
  - Skip
  - Adjust quality
    ↓ (Stories)
    R1: Basic player
    R2: Offline mode
    R3: Lyrics

Organize:
  - Create playlist
  - Add songs
  - Sort/filter
    ↓ (Stories)
    R1: Manual playlists
    R2: Collaborative playlists
    R3: Smart playlists (auto-update)

Share:
  - Share playlist
  - Follow friends
  - See what friends listen to
    ↓ (Stories)
    R1: Share link
    R2: Social features
    R3: Blend (combined playlists)
```

**Result**: Clear progression from MVP to advanced features

### Example 2: Slack - Team Messaging

**Persona**: Remote team member who needs to communicate

**Activities**: Join Team → Send Messages → Organize Conversations → Search History

**MVP Walking Skeleton (Release 1):**
- Join: Email invite → sign up
- Message: Send text to channel
- Organize: Create channels (public only)
- Search: Basic keyword search

**Release 2:**
- Direct messages
- File uploads
- Mentions (@user)
- Emoji reactions

**Release 3:**
- Threads
- Private channels
- Integrations
- Advanced search

**Insight**: MVP was extremely limited but functional end-to-end

---

## Story Mapping Workshop Facilitation / Điều Phối Workshop

**English:**

### Workshop Setup

**Participants (5-10 people):**
- Product Manager (facilitator)
- Designers (2-3)
- Engineers (2-3)
- QA (1)
- Optional: Customer support, sales

**Materials:**
- Sticky notes (3 colors: blue=activities, yellow=tasks, pink=stories)
- Sharpies (thick markers force conciseness)
- Large wall space or whiteboard
- Painter's tape (for release lines)
- Dot stickers (for voting)

**Duration**: 3-4 hours (with breaks)

### Facilitation Tips

**1. Set the Stage (10 min)**
- Explain why story mapping
- Show example map
- Define persona and problem

**2. Diverge Then Converge**
- First: Individual brainstorming (silent)
- Then: Share and cluster
- Avoid groupthink

**3. Keep it Flowing**
- Time-box each step
- Don't get stuck in details
- Parking lot for off-topic items

**4. Make it Visual**
- Draw user flow
- Use different colors
- Take photos at each stage

**5. Get Buy-in on MVP**
- Debate what's truly "minimum"
- Challenge every "must-have"
- Ask: "Can we launch without this?"

### Common Workshop Challenges

**Challenge**: Team wants to include everything in MVP
**Solution**: Walking skeleton test—"Can user complete journey end-to-end?"

**Challenge**: Disagreement on priorities
**Solution**: Dot voting + tie-breaker by PM/stakeholder

**Challenge**: Too many stories (100+)
**Solution**: Group similar stories, create epics

**Challenge**: Engineers push back on timeline
**Solution**: Estimate stories in map, adjust scope

**Vietnamese:**

### Workshop:

**Người Tham Gia**: PM, Designers, Engineers, QA (5-10 người)
**Vật Liệu**: Sticky notes, markers, tường lớn, tape
**Thời Gian**: 3-4 giờ

**Tips:**
1. Thiết lập bối cảnh
2. Phân kỳ rồi hội tụ
3. Giữ động lực
4. Hình ảnh hóa
5. Cam kết MVP

---

## Common Mistakes / Sai Lầm Thường Gặp

### Mistake 1: Too Much Detail Too Soon
**Problem**: Spending hours writing detailed stories before mapping
**Solution**: Start high-level, add detail as you slice releases

### Mistake 2: Technology-Centric Activities
**Problem**: Activities like "Set up database", "Build API"
**Solution**: Activities should be user actions, not tech tasks

### Mistake 3: Flat Backlog in Disguise
**Problem**: Just creating columns without user flow
**Solution**: Ensure left-to-right = chronological user journey

### Mistake 4: MVP is Too Big
**Problem**: "MVP" includes 50 stories, 6 months work
**Solution**: Walking skeleton should be 2-4 weeks, bare bones

### Mistake 5: Forgetting to Update
**Problem**: Map created once, never revisited
**Solution**: Living document—update as you learn

### Mistake 6: No Clear Releases
**Problem**: Stories prioritized but no release boundaries
**Solution**: Draw clear horizontal lines, date each release

---

## Tools for Story Mapping / Công Cụ

### Physical Tools
- **Sticky Notes**: Post-its, index cards
- **Whiteboard**: Dry-erase markers
- **Wall Space**: Painter's tape, sticky notes on wall
- **Pros**: Tactile, collaborative, easy for workshops
- **Cons**: Not persistent, hard for remote teams

### Digital Tools
- **Miro**: Infinite canvas, templates, collaborative
- **Mural**: Similar to Miro, great for workshops
- **StoriesOnBoard**: Purpose-built for story mapping
- **Jira Advanced Roadmaps**: Integrates with Jira
- **Cardboard**: Simple, Trello-like
- **Google Sheets**: Lightweight, universally accessible

### Hybrid Approach
1. Physical workshop to create map
2. Photo documentation
3. Digitize in tool
4. Maintain digitally going forward

---

## Related Frameworks / Khung Liên Quan

### Jobs to Be Done (JTBD)
**Use Before Story Mapping**: Define the "job" user is trying to do
- JTBD = Why (user motivation)
- Story Map = How (user flow to get job done)

### Product Roadmapping
**Use After Story Mapping**: Story map feeds into roadmap
- Story map = Feature breakdown
- Roadmap = Timeline and themes

### User Journey Mapping
**Complementary**: Different perspectives
- Journey map = Emotions, touchpoints, service design
- Story map = Features, releases, development planning

### Agile/Scrum
**Story Mapping Feeds Backlog**: Stories from map → sprint backlog
- Map provides context
- Backlog pulls from map

---

## Quick Reference Card / Thẻ Tham Khảo Nhanh

### Story Map Layers (Top to Bottom)
1. **Activities** (5-10): High-level user goals
2. **Tasks** (3-8 per activity): Steps to complete activity
3. **Stories** (many): Detailed requirements, prioritized

### Story Format
**As a** [user type]
**I want to** [action]
**So that** [benefit]

**Example**: As a shopper, I want to save items to wishlist, so I can buy them later

### MVP Criteria (Walking Skeleton)
- ✅ End-to-end user flow
- ✅ Functional (not polished)
- ✅ Validates core value
- ✅ Can ship in 2-4 weeks

### Workshop Checklist
- [ ] Define persona
- [ ] Frame problem (JTBD)
- [ ] Map activities (left-to-right)
- [ ] Add tasks under activities
- [ ] Add stories under tasks
- [ ] Prioritize stories (top-to-bottom)
- [ ] Slice for releases (horizontal lines)
- [ ] Document and digitize

### Color Coding
- 🔵 Blue: Activities
- 🟡 Yellow: Tasks
- 🔴 Pink: Stories
- 🟢 Green: Release 1 (MVP)
- 🟠 Orange: Release 2
- 🟣 Purple: Release 3+

---

**Last Updated**: 2025-11-21
**Version**: 1.0
**Root Commands**: `/phase2:story-map`, `/phase3:plan`
**Next Review**: 2025-12-21

---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
