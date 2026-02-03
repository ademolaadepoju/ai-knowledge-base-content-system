# User Feedback & Admin Tools - Microcopy Guide
**Version:** 1.0  
**Purpose:** Copy patterns for feedback collection and content improvement workflows

---

## Feedback Mechanism Design

### Primary Goal
Collect actionable feedback to improve:
1. Answer quality and accuracy
2. Knowledge base completeness
3. User experience with AI assistant

### Secondary Goals
- Identify outdated documentation
- Flag conflicting sources
- Detect common pain points
- Prioritize content updates

---

## Feedback Collection - "Was this helpful?"

### Basic Thumbs Up/Down

**Placement:** After every AI assistant response

**Copy:**

```
Was this helpful?
👍 Yes     👎 No
```

**Interaction:**
- Single click captures sentiment
- No interruption to user flow
- Optional follow-up for details

---

### Positive Feedback Flow

**After user clicks 👍:**

```
Glad I could help! 

[Optional: Brief follow-up]
□ This answered my question completely
□ This helped me solve my problem
□ The information was clear and easy to understand

[Skip] [Submit]
```

**Design notes:**
- Keep it brief - user already got what they needed
- Make submission optional (default to skip)
- Don't interrupt their flow

---

### Negative Feedback Flow

**After user clicks 👎:**

```
Sorry this wasn't helpful. What went wrong?

○ Answer was unclear
○ Information seems incorrect or outdated  
○ Missing important details
○ Didn't answer my question
○ Technical error or problem
○ Other: [text field]

[Skip] [Submit]
```

**With conditional follow-ups:**

**If "Answer was unclear":**
```
What would have made it clearer?
[Open text field - optional]

Helpful additions:
□ More examples
□ Step-by-step instructions
□ Simpler language
```

**If "Information seems incorrect":**
```
What seems incorrect?
[Open text field - encouraged]

This helps us verify and update our documentation.
```

**If "Missing important details":**
```
What information were you looking for?
[Open text field - encouraged]

This helps us improve our knowledge base.
```

**If "Didn't answer my question":**
```
What were you actually asking about?
[Open text field - encouraged]

Would you like to:
• Rephrase your question and try again
• Connect with live support
• Request a callback
```

---

## Feedback Analysis Categories

### Category 1: Content Quality Issues

**Triggers for content review:**
- Multiple "incorrect information" flags
- "Outdated" feedback on same document
- Conflicting information reports

**Admin dashboard alert:**
```
⚠️ Content Quality Alert

Document: Refund Policy (POL-REF-001)
Issue: 12 users reported information seems outdated (last 30 days)
Specific section: Processing Timeline

Common feedback:
• "This says 5-10 days but mine took 3 days"
• "Timeline seems faster now"
• "Is this still accurate?"

[Review Document] [Schedule Update] [Dismiss]
```

---

### Category 2: Knowledge Gaps

**Triggers:**
- "Missing details" feedback
- "Didn't answer question" with specific topics
- Questions that consistently get "no source available" responses

**Admin dashboard alert:**
```
📋 Knowledge Gap Detected

Topic: "Freezing account temporarily"
Frequency: 24 requests (last 30 days)
Current coverage: No specific documentation found

Sample user questions:
• "How do I temporarily freeze my account while traveling?"
• "Can I pause my account instead of closing it?"
• "Lock account vs close account - what's difference?"

[Create Documentation] [Add to FAQ] [Assign to Team]
```

---

### Category 3: AI Response Quality

**Triggers:**
- "Unclear" or "confusing" feedback
- Low ratings on well-documented topics
- Technical errors in responses

**Admin dashboard alert:**
```
🤖 AI Response Quality Issue

Question pattern: "How to upgrade verification"
AI response quality: 42% thumbs down (last 7 days)
Documentation available: Yes (Account Security Policy)

Analysis:
• AI response is accurate but overly detailed (avg 400 words)
• Users want simple steps, getting policy explanation
• Response template may need adjustment

[Review AI Prompt] [Update Template] [Review Documentation]
```

---

## Admin Actions - Content Improvement

### Action 1: Add a Source

**When:** User knows of documentation AI didn't reference

**User-facing copy:**

```
Know of relevant documentation?

Help improve this answer by suggesting a source:

Document title or link: [text field]
Why it's relevant: [text field]

Your suggestion will be reviewed by our content team.

[Cancel] [Submit Suggestion]
```

**Admin review interface:**

```
📄 Source Suggestion

From: user@email.com
Date: Jan 25, 2025
Question: "What are cryptocurrency tax requirements?"

Suggested source:
• IRS Publication 544 - available in Help Center
• Reason: "This has tax reporting requirements the AI didn't mention"

Current AI response cited:
• Cryptocurrency Payment Beta (updated Jan 2025)

[Add to Knowledge Base] [Update Existing Doc] [Decline with Reason]
```

---

### Action 2: Report Incorrect Information

**User-facing copy:**

```
Report incorrect information

What's incorrect?
[Open text field - required]

What should it say instead?
[Open text field - optional]

Your report helps us keep documentation accurate and up-to-date.

[Cancel] [Submit Report]
```

**Admin review interface:**

```
⚠️ Accuracy Report

Document: Refund Policy (POL-REF-001)
Section: Processing Timeline
Reported by: 3 users (last 14 days)

Claim: "Refunds take 5-10 days"
User reports:
• "Mine took 3 days, not 5-10"
• "I got refund in 2 days"
• "This timeline seems wrong"

Current documentation (updated Jan 2025):
"3-5 business days to original payment method"

Analysis: AI may be citing old version or FAQ (Oct 2024) instead of policy.

[Update Documentation] [Fix AI Citation Logic] [Investigate Further] [No Action Needed]
```

---

### Action 3: Mark Source as Outdated

**User-facing copy:**

```
Is this information outdated?

What's changed since this was written?
[Open text field]

Do you know what the current information is?
[Open text field - optional]

[Cancel] [Submit]
```

**Admin review interface:**

```
📅 Outdated Content Report

Document: Chargeback Handling Guide (PROC-CHG-001)
Last updated: March 2023 (nearly 2 years old)
Reports: 8 users flagged as outdated (last 30 days)

User feedback themes:
• "Fee seems different now"
• "Is this 2023 info still right?"
• "Timeline doesn't match my experience"

Document already marked: ⚠️ OUTDATED in knowledge base

[Schedule Update] [Request SME Review] [Archive Document] [Extend Review Date]
```

---

### Action 4: Request Documentation Update

**User-facing copy:**

```
Request documentation update

What topic needs better documentation?
[Text field]

What information is missing?
[Text field]

How would this help you?
[Text field - optional]

[Cancel] [Submit Request]
```

**Admin triage interface:**

```
📝 Documentation Request

Topic: "How to report a scam payment"
Priority: High (15 similar requests last 30 days)

User need:
"I sent money to someone who scammed me. The dispute process 
doc talks about merchant issues but not scams between individuals. 
I don't know if I should report as fraud or dispute or what."

Current coverage:
• Unauthorized Transaction Policy - covers account takeover, not scams
• Dispute Resolution - covers buyer/seller disputes, not scam prevention
• Gap: No guidance for "I willingly sent money but got scammed"

[Create New Doc] [Update Existing Doc] [Add to FAQ] [Assign to Legal] [Defer]
```

---

### Action 5: Flag for Content Review

**User-facing copy:**

```
Flag this response for review

What needs review?
○ Information seems incomplete
○ Multiple interpretations possible
○ Conflicting with other sources
○ Edge case not covered
○ Other: [text field]

Additional context: [optional text field]

[Cancel] [Submit]
```

**Admin review queue:**

```
🚩 Content Review Flag

Response ID: #A1B2C3
Question: "Can I get refund if I paid with cryptocurrency?"
AI Answer: [Shows answer citing both Refund Policy and Crypto Beta]

Flag reason: "Conflicting with other sources"
User note: "One part says yes, another says no. Very confusing."

Analysis:
• Refund Policy: Standard refunds available
• Crypto Beta: "No refunds for crypto transactions"
• AI correctly identified conflict but explanation may be unclear

[Improve Response Template] [Add Disambiguation] [Update Source Docs] [No Action]
```

---

## Contextual Feedback Prompts

### After Complex/Multi-Part Answers

```
This was a complex question. Did I cover everything you needed?

□ Yes, this was complete
□ Need more details on: [text field]
□ Still have questions about: [text field]

[Submit] [I'm all set]
```

---

### After "No Source Available" Response

```
I couldn't find documentation on this topic.

Would you like to:
○ Rephrase your question (maybe I'll find relevant docs)
○ Connect with live support who can help
○ Request this topic be added to documentation

[Continue]
```

---

### After Outdated Source Warning

```
I provided information from an older document (updated [date]).

Did you:
○ Contact support to verify (recommended)
○ Use the information as-is (understanding it may have changed)
○ Found the answer elsewhere

This helps us prioritize documentation updates.

[Skip] [Submit]
```

---

## Admin Dashboard - Key Metrics

### Content Health Scorecard

```
📊 Knowledge Base Health (Last 30 Days)

Overall Satisfaction: 78% 👍
↑ 3% from last month

Top Issues:
1. Outdated information (142 reports)
   • Focus: Chargeback Guide, older FAQs
2. Missing details (89 reports)
   • Top gap: Scam prevention guidance
3. Unclear responses (67 reports)
   • Pattern: Verification process explanations

Documents Needing Attention:
⚠️ Chargeback Handling Guide - 24 months old, 45 outdated flags
⚠️ Account Limits FAQ - 4 months old, 12 accuracy reports
✓ Refund Policy - 2 weeks old, 92% satisfaction

[View Full Report] [Schedule Reviews] [Export Data]
```

---

### Question Coverage Analysis

```
❓ Question Coverage (Last 30 Days)

Total questions: 3,847
Answered with high confidence: 2,891 (75%)
Answered with caveats: 623 (16%)
No documentation found: 333 (9%)

Top unanswered topics:
1. "Temporary account freeze" - 47 questions
2. "Scam prevention tips" - 38 questions  
3. "Business vs personal account" - 31 questions
4. "Cryptocurrency tax implications" - 27 questions
5. "International student usage" - 19 questions

[Create Documentation Plan] [Assign Topics] [View Details]
```

---

### Source Quality Trends

```
📚 Source Quality Overview

Active documents: 10
Outdated (12+ months): 2
Under review: 0
Scheduled for update: 1

Average document age: 4.2 months
Documents updated last 30 days: 2

Citation patterns:
• Refund Policy: 847 citations (most referenced)
• Payment Declined Guide: 623 citations
• Account Security Policy: 521 citations
• Chargeback Guide: 12 citations (⚠️ low + outdated)

Recommendation: Review/update Chargeback Guide or archive

[View Details] [Schedule Updates] [Archive Old Docs]
```

---

## User Journey - Feedback Loop

### Scenario: User Gets Unhelpful Answer

**Step 1: User asks question**
```
User: "Why was my payment declined?"
AI: [Provides generic answer citing multiple possible causes]
```

**Step 2: User provides feedback**
```
Was this helpful?
👍 Yes     👎 No

[User clicks 👎]

Sorry this wasn't helpful. What went wrong?
[User selects: "Missing important details"]

What information were you looking for?
[User types: "It didn't ask about my specific error code CH-403"]
```

**Step 3: System captures context**
```
Logged data:
• Question: "Why was my payment declined?"
• AI cited: Payment Declined Troubleshooting Guide
• Feedback: Missing details
• Specific need: Error code CH-403 not covered
• Document gap identified: Error code reference table
```

**Step 4: Admin reviews**
```
📋 Knowledge Gap Alert

Topic: Payment decline error codes
User need: "Error code CH-403 meaning"
Frequency: 1 report (new gap)

Current documentation: Generic troubleshooting only, no error codes

[Monitor for Patterns] [Create Error Code Guide] [Add to Backlog]
```

**Step 5: Content update (if pattern emerges)**
```
After 10 similar reports over 2 weeks...

Task created:
Title: Add error code reference table to Payment Declined Guide
Priority: Medium
Assigned to: Content Team
Due: March 15, 2026

Scope:
• Add comprehensive error code table
• Update AI prompt to check for error codes in questions
• Cross-reference with engineering error code documentation
```

---

## Feedback Response - Closing the Loop

### When User Reports Issue

**Immediate acknowledgment:**
```
✓ Thanks for your feedback!

Your report helps us improve our documentation. 

We review all feedback and make updates regularly. If we need more 
information, we may reach out to [user@email.com].

[Continue] [Contact Support Instead]
```

---

### When Content is Updated Based on Feedback

**Email to users who reported (optional):**
```
Subject: We updated our documentation based on your feedback

Hi [Name],

You recently reported that our documentation on [topic] was [outdated/
incomplete/unclear].

Good news: We've just updated the [Document Name] with:
• [Improvement 1]
• [Improvement 2]
• [Improvement 3]

Try asking the AI assistant again, or view the updated documentation here: [link]

Thanks for helping us improve!

The GothPay Documentation Team
```

---

## Integration Points

### Link to Live Support

**When AI can't help:**
```
I wasn't able to find a good answer in our documentation.

Connect with support for help:

💬 Live Chat (2-3 min wait)
[Start Chat]

📞 Phone Support (1-800-GOTH-PAY)
Available 24/7

📧 Email Support (support@gothpay.com)
Response within 24 hours

Before you go, would you like to report this gap so we can add documentation?
[Yes, Report Gap] [No, Just Connect Me]
```

---

### Escalation Path

**When user repeatedly gets unhelpful answers:**

After 3 negative feedbacks in same conversation:

```
I'm having trouble finding the right information for you.

Let me connect you with a specialist who can help:

○ Live chat with support specialist
○ Schedule callback within 1 hour
○ Email detailed question to priority queue

We'll also flag this conversation for our documentation team to review.

[Connect with Specialist]
```

---

## Success Metrics

### What to Measure

**User Satisfaction:**
- Overall thumbs up rate 
- Thumbs up rate by document (identify weak content)
- Repeat question rate (if user re-asks, first answer failed)

**Content Coverage:**
- % of questions with high-confidence answers 
- % of questions with no documentation 
- Time to add documentation for gaps 

**Documentation Quality:**
- Average document age (target: <6 months)
- Outdated flags per document 
- Accuracy reports per document 

**Feedback Volume:**
- Feedback submission rate
- Detailed feedback rate 
- Admin action completion rate 

---

*Version 1.0 | Last updated: February 1, 2026*
