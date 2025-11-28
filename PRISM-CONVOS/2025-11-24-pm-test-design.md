---
conversation_id: "2025-11-24-pm-test-design"
date_created: "2025-11-24"
date_modified: "2025-11-25"
topic: "PM Test Question Generation for Hiring Competition"
status: "active"
participants:
  - role: "user"
    name: "User"
  - role: "assistant"
    platform: "Gemini"
  - role: "assistant"
    platform: "Claude"
tags:
  - "product-test"
  - "interview-questions"
  - "hiring"
  - "product-management"
  - "context-based-questions"
summary: "An iterative conversation to create four essay questions for a PM competition. Evolved from generic questions to specific context-based questions using 4 top product companies with simulated metrics to prevent AI-generated answers."
related_files:
  - "03-PRODUCT-FOUNDATION/PEOPLE-interviewing-framework.md"
  - "03-PRODUCT-FOUNDATION/PRIORITIZATION-rice-prioritization.md"
---

## Conversation Log

### User (2025-11-24)
I need 4 essay questions for a Product Test competition to evaluate candidates for UX/UI Designer and DA/BA roles at an "Apply" difficulty level.

### Assistant - Gemini (2025-11-24)
Provided initial set of 4 generic questions based on PEOPLE-interviewing-framework.md.

### User (2025-11-24)
Can you enhance with more real-world context and evaluation criteria? Need context-based questions to avoid AI abuse.

### Assistant - Gemini (2025-11-24)
Created interconnected questions based on fictional "NextUp" app.

### User (2025-11-24)
I want real-world product-based questions, each question one product. Include Spotify Wrapped.

### Assistant - Gemini (2025-11-24)
Created "Famous Features Edition" with generic template letting candidates choose their own products.

### User (2025-11-25)
Gemini created a mess. Requirements:
1. Use 4 top product companies' best features with simulated numbers
2. Questions should be real, not hallucinated
3. Questions should be clear
4. Follow context-based format to prevent AI-generated shallow answers

Guideline: "Bạn là PM của [app]. Khi phát triển tính năng X, bạn cần phối hợp với teams nào? Vai trò của mỗi team? Conflict nào có thể xảy ra?"

### Assistant - Claude (2025-11-25)
Understood. Requirements updated:
- 2 questions for UX/UI Designer role
- 2 questions for DA/BA role
- Backlog existing PM questions and DA essay assignment

**Actions taken:**
1. Created `00-BACKLOGS/BACKLOG-pm-test-questions.md` (PM questions)
2. Moved `H4TF-2025-DA-essay-assignment.md` to `00-BACKLOGS/BACKLOG-H4TF-2025-DA-essay-assignment.md`
3. Creating 4 new role-specific questions below

---

## Final Contest Questions v3: UX/UI Designer + DA/BA Evaluation

**Instructions for Candidates:** You are given specific product scenarios with real metrics. Answer based on your understanding of these products and your role-specific expertise. Generic or AI-generated answers will be easily identified by evaluators.

**Difficulty Level:** 3/4 (Apply)

---

## Part 1: UX/UI Designer Evaluation (2 Questions)

### **Question 1: Duolingo Streak Feature - UX Redesign Challenge**
**(Approx. 150-200 words)**

**Context:**
You are a UX/UI Designer at Duolingo. User research data shows:
- 83% 1-year retention rate for streak users
- However, 47% of users who break their streak never return
- "Streak Freeze" feature (protects streak for 1 day) has 23% awareness rate
- Users report feeling "guilty" and "ashamed" after breaking streaks (NPS drops 34 points)
- Current streak break screen shows: red "X", streak count reset to 0, no recovery options visible

**Question:**
1. Identify TWO specific UX problems with the current streak break experience based on the data above.
2. Sketch or describe in detail ONE redesigned screen for when a user breaks their streak. Explain what elements you would include and why (consider visual hierarchy, emotional design, and recovery paths).
3. What metrics would you track to measure if your redesign successfully reduces user churn after streak breaks?

**Evaluation Criteria:**
- **Problem Identification (30%):** Does candidate connect UX issues to specific data points?
- **Design Solution Quality (40%):** Is the proposed design detailed, user-centered, and addresses emotional needs?
- **Measurement Thinking (30%):** Are proposed metrics directly tied to the redesign goals?

---

### **Question 2: Grab Super App - Information Architecture Challenge**
**(Approx. 200-250 words)**

**Context:**
You are a UX/UI Designer at Grab (Southeast Asia's super app). Current state:
- App has 8 main services: Ride, Food, Mart, Express, Pay, Rewards, Insurance, Invest
- Average user uses only 2.3 services
- 62% of users report "difficulty finding features they need"
- Home screen has 12 icons + 3 banners + bottom navigation (5 items)
- Task completion time for booking a ride increased from 8 seconds (2021) to 14 seconds (2024)
- New users take 3.2 sessions before discovering GrabFood (key revenue driver)

**Question:**
1. Analyze the information architecture problem: Why might task completion time have increased despite no major feature changes?
2. Propose TWO different navigation approaches to improve feature discoverability:
   - Approach A: Personalization-based solution
   - Approach B: Simplification-based solution
3. For each approach, describe:
   - Key UI changes you would make
   - Trade-offs (what you gain vs. what you lose)
4. Which approach would you recommend for A/B testing first and why?

**Evaluation Criteria:**
- **IA Analysis (25%):** Does candidate understand how complexity affects usability?
- **Solution Creativity (35%):** Are the two approaches genuinely different and well-thought-out?
- **Trade-off Awareness (25%):** Does candidate acknowledge what each approach sacrifices?
- **Testing Rationale (15%):** Is the A/B test recommendation logical and justified?

---

## Part 2: DA/BA Evaluation (2 Questions)

### **Question 3: Spotify Wrapped - Data Analysis Investigation**
**(Approx. 200-250 words)**

**Context:**
You are a Data Analyst at Spotify working on Wrapped 2024. The data team notices unexpected patterns:
- Wrapped 2023 share rate: 156 million social shares
- Wrapped 2024 share rate (first 48 hours): down 18% vs. same period last year
- User completion rate (viewing all cards): dropped from 60% to 52%
- "Top Artist" card share rate: stable (+2%)
- "Listening Personality" card share rate: down 41%
- No technical issues reported; feature launched on same date as previous year
- Premium subscriber share rate: stable; Free tier share rate: down 29%

**Question:**
1. Based on the data above, form THREE distinct hypotheses explaining why Wrapped 2024 shares are down (consider: content quality, user behavior changes, external factors).
2. For your TOP hypothesis, describe:
   - What additional data you would request from the engineering/product team
   - What SQL query logic you would use to validate (describe tables and joins conceptually)
   - What result would confirm or reject your hypothesis
3. If your analysis confirms "Free tier users find the new Listening Personality card irrelevant," what actionable recommendation would you give to the product team?

**Evaluation Criteria:**
- **Hypothesis Quality (35%):** Are hypotheses specific, data-driven, and diverse?
- **Analytical Approach (40%):** Does candidate demonstrate practical data analysis skills?
- **Business Recommendation (25%):** Is the recommendation actionable and tied to findings?

---

### **Question 4: Shopee - Requirements Gathering for Cart Abandonment**
**(Approx. 150-200 words)**

**Context:**
You are a Business Analyst at Shopee. The e-commerce team shares this data:
- Cart abandonment rate: 78% (industry average: 70%)
- Abandonment by stage: 45% at shipping cost reveal, 30% at payment, 25% at final review
- Mobile abandonment: 82% vs. Desktop: 68%
- Users with vouchers in cart: 65% abandonment vs. 83% without vouchers
- Average cart value at abandonment: $47 (higher than completed orders at $32)
- Time spent on checkout page before abandonment: 4.2 minutes (vs. 1.8 minutes for completed)

**Question:**
1. Based on the data, identify the TOP 2 problem areas contributing most to cart abandonment.
2. For ONE problem area, write 3 specific user stories following the format:
   "As a [user type], I want [goal], so that [benefit]"
3. What clarifying questions would you ask stakeholders before finalizing requirements? List at least 3 questions and explain why each is important.

**Evaluation Criteria:**
- **Data Interpretation (30%):** Does candidate correctly identify the highest-impact problem areas?
- **User Story Quality (35%):** Are user stories specific, actionable, and user-centered?
- **Stakeholder Communication (35%):** Are clarifying questions relevant and show business understanding?

---

## Grading Notes for Evaluators

**Red flags for AI-generated answers:**
- Generic design principles without connecting to specific data points
- User stories that could apply to any e-commerce platform
- Hypotheses that ignore the specific metrics provided
- Solutions that don't acknowledge the constraints in the scenario
- No mention of trade-offs or risks

**Strong answers will:**
- Reference the specific metrics provided in each scenario
- Show role-specific expertise (UX: visual/emotional design; DA/BA: data interpretation/requirements)
- Acknowledge trade-offs explicitly
- Propose solutions constrained by the given parameters
- Demonstrate understanding of how these companies actually operate