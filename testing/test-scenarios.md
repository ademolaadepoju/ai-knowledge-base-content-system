# AI Knowledge Base Assistant - Test Scenarios
**Version:** 1.0  
**Last Updated:** February 1, 2026  
**Purpose:** Validation test cases for the GothPay AI assistant

---

## How to Use This Test Suite

For each scenario:
1. **Input** the user query
2. **Expected Response** describes what should happen
3. **Success Criteria** defines what makes a good response
4. **Sources** lists which documents should be cited

---

## Test Category 1: Simple, Well-Documented Questions

### Test 1.1: Refund Timeline (Happy Path)

**User Query:**
```
How long do refunds take?
```

**Expected Response Type:** Template 1 (Direct Answer)

**Expected Content:**
- Clear answer: 3-5 business days to card, with additional bank processing
- Step-by-step if applicable
- Citation to Refund Policy (Jan 2025)
- High confidence language

**Success Criteria:**
✓ Answer in first 1-2 sentences  
✓ Specific timeline mentioned  
✓ Source cited with date  
✓ No hedging language (should be definitive)  
✓ Under 200 words  

**Sources to Cite:**
- Refund Policy (POL-REF-001, updated January 2025) — Processing Timeline section

**Mock Response:**
```
Your refund will take 3-5 business days to reach your original payment method after it's approved.

For credit/debit card refunds:
1. GothPay processes the refund immediately upon approval
2. Your card issuer receives it within 3-5 business days
3. Your bank may take an additional 1-3 business days to post it to your account

Total timeline: Usually 5-10 business days from approval to seeing funds in your account.

Based on:
• Refund Policy (updated January 2025) — Processing Timeline section

I assumed you paid with a card. If you paid with bank account or GothPay balance, timing differs slightly.
```

---

### Test 1.2: Account Verification Levels

**User Query:**
```
What's the difference between Basic and Enhanced verification?
```

**Expected Response Type:** Template 10 (Comparison/Which Option)

**Expected Content:**
- Table or clear comparison
- Sending/receiving limits for each
- How to upgrade
- Citation to verification docs

**Success Criteria:**
✓ Clear differentiation between levels  
✓ Actionable next steps (how to upgrade)  
✓ Limits clearly stated  
✓ Source cited  

**Sources to Cite:**
- Account Security & Verification Policy (POL-SEC-003, updated January 2025) — Identity Verification Levels
- Account Limits & Verification FAQ (FAQ-VER-002, updated October 2024) — Verification Tiers

---

### Test 1.3: Payment Decline - Insufficient Funds

**User Query:**
```
My payment was declined. The error says insufficient funds. What do I do?
```

**Expected Response Type:** Template 8 (Troubleshooting)

**Expected Content:**
- Explain what this means
- Troubleshooting steps
- How to check balance
- Alternative solutions

**Success Criteria:**
✓ Acknowledges user's issue  
✓ Explains the error clearly  
✓ Provides actionable steps  
✓ Offers alternatives  

**Sources to Cite:**
- Payment Declined Troubleshooting Guide (PROC-DEC-001, updated November 2024) — Insufficient Funds section

---

## Test Category 2: Outdated Source Scenarios

### Test 2.1: Chargeback Fee (Outdated Info)

**User Query:**
```
What's the chargeback fee if I dispute with my bank?
```

**Expected Response Type:** Template 5 (Outdated Source Warning)

**Expected Content:**
- Answer from outdated source ($15 according to March 2023 doc)
- ⚠️ Clear freshness warning
- Recommendation to verify with support
- Explain why chargeback is not recommended

**Success Criteria:**
✓ Provides available information  
✓ **MUST include ⚠️ outdated warning**  
✓ Recommends verification  
✓ Notes document is almost 2 years old  
✓ Still helpful despite age  

**Sources to Cite:**
- Chargeback Handling Guide — ⚠️ Last updated March 2023

**Mock Response:**
```
⚠️ The most recent documentation on chargebacks is from March 2023, so please verify this information is still current.

According to the Chargeback Handling Guide (last updated March 2023):

GothPay charges a $15 fee when you file a chargeback with your bank instead of using GothPay's dispute process. This fee applies even if you win the chargeback.

**Important:**
Because this information is almost 2 years old, I recommend:
• Contacting GothPay support to confirm the current chargeback fee
• Asking about the current timeline for chargeback resolution

For most cases, it's better to file a dispute through GothPay first rather than going directly to your bank. GothPay's process is faster (10-15 days vs 45-90 days) and has no fees.

Based on:
• Chargeback Handling Guide — ⚠️ Last updated March 2023
```

---

### Test 2.2: Chargeback Process Details

**User Query:**
```
How long does the chargeback process take?
```

**Expected Response Type:** Template 5 (Outdated Source Warning)

**Expected Content:**
- Timeline from outdated doc (45-90 days)
- Freshness warning
- Comparison to GothPay dispute process
- Recommendation to use GothPay process instead

**Success Criteria:**
✓ Provides timeline with caveat  
✓ Clear outdated warning  
✓ Offers better alternative (GothPay disputes)  

---

## Test Category 3: Conflicting Sources

### Test 3.1: Cryptocurrency Refunds (Major Conflict)

**User Query:**
```
Can I get a refund if I paid with cryptocurrency?
```

**Expected Response Type:** Template 6 (Conflicting Sources)

**Expected Content:**
- Clearly explains standard refund policy
- Clearly explains crypto is EXCEPTION
- Highlights the conflict
- Helps user understand which applies

**Success Criteria:**
✓ Identifies both policies  
✓ Explains the key difference  
✓ Makes it crystal clear crypto = no refunds  
✓ Cites both sources  

**Sources to Cite:**
- Refund Policy (POL-REF-001, updated January 2025)
- Cryptocurrency Payment Beta (BETA-CRYPTO-001, updated January 2025)

**Mock Response:**
```
The answer depends on whether you're using cryptocurrency or regular USD, because different policies apply:

**For regular USD payments (standard GothPay):**
You CAN request a refund if you don't receive the goods or services you paid for. File a dispute through the app within 180 days and GothPay will investigate.

**For cryptocurrency payments (beta feature):**
You CANNOT get a refund under any circumstances. Cryptocurrency transactions are final and irreversible—even if you were scammed or didn't receive what you paid for.

**The key difference:**
Cryptocurrency operates on blockchain technology where transactions cannot be reversed. GothPay's standard refund and dispute policies do NOT apply to crypto payments. This is why GothPay recommends using regular USD for purchases, and crypto only for investments or transfers to people you fully trust.

Based on:
• Refund Policy (updated January 2025) — Standard Refund Eligibility
• Cryptocurrency Payment Beta (updated January 2025) — Risks & Disclaimers section
```

---

### Test 3.2: Cryptocurrency Beta Availability

**User Query:**
```
How do I buy cryptocurrency on GothPay?
```

**Expected Response Type:** Template 4 (No Source) OR Beta Feature explanation

**Expected Content:**
- Explain it's beta-only
- Clarify invitation-required
- Describe feature briefly (since user asked)
- How to know if they have access

**Success Criteria:**
✓ Clear about beta status  
✓ Explains access requirements  
✓ Doesn't promise availability  
✓ Helpful even if user doesn't have access  

**Sources to Cite:**
- Cryptocurrency Payment Beta (BETA-CRYPTO-001, updated January 2025) — with ⚠️ BETA disclaimer

---

## Test Category 4: No Source Available

### Test 4.1: Temporary Account Freeze

**User Query:**
```
How do I temporarily freeze my account while I'm traveling?
```

**Expected Response Type:** Template 4 (No Source Available)

**Expected Content:**
- Honest "not in documentation"
- Possible interpretations
- How to get answer
- Alternative solutions if any

**Success Criteria:**
✓ Honest about lack of documentation  
✓ Doesn't make up information  
✓ Provides clear next steps  
✓ Offers related alternatives  

**Mock Response:**
```
I couldn't find information about temporarily freezing your account in the current GothPay documentation.

This might mean:
• The feature hasn't been documented yet
• It's not currently available
• It goes by a different name (like "account lock" or "travel mode")

**Here's how to get an answer:**
• Contact GothPay support at support@gothpay.com
• Live chat available 24/7 in the app
• Phone support: 1-800-GOTH-PAY

**Related options that ARE documented:**
If you're concerned about security while traveling, you can:
• Enable 2-factor authentication (required for all logins from new locations)
• Set up transaction notifications (get alerts for every payment)
• Lock your account if suspicious activity occurs (Settings > Security > Lock Account)

Would you like me to explain any of these security features?
```

---

### Test 4.2: Feature Not Documented

**User Query:**
```
Can I schedule payments for future dates?
```

**Expected Response Type:** Template 4 (No Source Available)

**Expected Content:**
- Not found in docs
- How to contact support
- No speculation

**Success Criteria:**
✓ Clear "not in documentation"  
✓ Support contact info  
✓ No fabricated features  

---

## Test Category 5: Complex Multi-Part Questions

### Test 5.1: Wrong Recipient + Prevention

**User Query:**
```
I accidentally sent $200 to the wrong person. How do I get it back and how can I prevent this in the future?
```

**Expected Response Type:** Template 2 or 7 (Conditional/How-To)

**Expected Content:**
- Part 1: Explains P2P payments can't be reversed
- Part 2: What user can do (contact recipient)
- Part 3: Prevention tips (verify before sending)
- Empathetic tone

**Success Criteria:**
✓ Addresses both parts of question  
✓ Empathetic (acknowledges frustration)  
✓ Actionable on both fronts  
✓ Educational (prevention tips)  
✓ Realistic about limitations  

**Sources to Cite:**
- Dispute Resolution Process (PROC-DIS-001, updated December 2024) — P2P Dispute scenarios
- Account Security Policy (POL-SEC-003, updated January 2025) — Best practices

**Mock Response:**
```
I understand this is frustrating. Unfortunately, GothPay cannot reverse peer-to-peer payments once they're sent.

**To try to get your money back:**
1. Contact the recipient directly through GothPay messaging or any contact info you have
2. Politely explain the error and request they send the money back
3. If they refuse and you believe it's a scam, report to GothPay's fraud team

GothPay can facilitate communication but cannot force the recipient to return the funds. If the amount is significant and they refuse, small claims court may be an option.

**To prevent this in the future:**
• Always double-check the recipient's username, email, or phone number before confirming
• Use the "request money" feature first to confirm you have the right person
• Send a small test amount ($1) to new recipients before sending larger amounts
• Enable transaction notifications so you're immediately aware of all payments

Based on:
• Dispute Resolution Process (updated December 2024) — Peer-to-Peer Dispute Resolution
• Account Security & Verification Policy (updated January 2025) — Best Practices section
```

---

### Test 5.2: Payment Declined + Multiple Possible Causes

**User Query:**
```
My payment was declined but I don't know why. Can you help me figure it out?
```

**Expected Response Type:** Template 8 (Troubleshooting/Decision Tree)

**Expected Content:**
- Common causes listed
- How to diagnose each
- Prioritized by likelihood
- Clear next steps for each

**Success Criteria:**
✓ Systematic approach  
✓ User can self-diagnose  
✓ Actionable for each cause  
✓ Escalation path if none work  

**Sources to Cite:**
- Payment Declined Troubleshooting Guide (PROC-DEC-001, updated November 2024)

---

## Test Category 6: Conditional/Depends Scenarios

### Test 6.1: Weekly Sending Limit

**User Query:**
```
How much can I send per week?
```

**Expected Response Type:** Template 2 (Conditional Answer)

**Expected Content:**
- Depends on verification level
- All three tiers explained
- How to check current level
- How to upgrade

**Success Criteria:**
✓ All scenarios covered  
✓ Easy to identify which applies  
✓ Upgrade path clear  

**Sources to Cite:**
- Account Limits & Verification FAQ (FAQ-VER-002, updated October 2024)

---

### Test 6.2: Verification Requirements

**User Query:**
```
Do I need to verify my identity?
```

**Expected Response Type:** Template 2 (Conditional)

**Expected Content:**
- Depends on what user wants to do
- Basic is automatic (email + phone)
- Enhanced needed for higher limits
- When Premium is needed

**Success Criteria:**
✓ Clarifies what's required vs optional  
✓ Explains benefits of each level  

---

## Test Category 7: Policy Explanation

### Test 7.1: Why Can't P2P Be Reversed

**User Query:**
```
Why can't GothPay reverse peer-to-peer payments?
```

**Expected Response Type:** Template 9 (Policy Explanation)

**Expected Content:**
- States the policy clearly
- Explains reasoning (like cash, prevents abuse)
- What this means for users
- How it's standard across industry

**Success Criteria:**
✓ Explains "why" not just "what"  
✓ Helps user understand rationale  
✓ Acknowledges user's perspective  

**Sources to Cite:**
- Dispute Resolution Process (PROC-DIS-001, updated December 2024)

---

### Test 7.2: Why Geographic Restrictions

**User Query:**
```
Why doesn't GothPay work internationally?
```

**Expected Response Type:** Template 9 (Policy Explanation)

**Expected Content:**
- Policy statement (US only)
- Reasons (regulatory, banking, business)
- Future plans mentioned
- Alternatives suggested

**Success Criteria:**
✓ Honest about limitations  
✓ Explains business/legal reasons  
✓ Offers hope (future expansion)  
✓ Provides alternatives  

**Sources to Cite:**
- International Payment Policy (POL-INTL-001, updated January 2025)

---

## Test Category 8: Edge Cases

### Test 8.1: Cryptocurrency + Standard Policies Confusion

**User Query:**
```
I used cryptocurrency and want to dispute the transaction because I didn't receive what I paid for.
```

**Expected Response Type:** Template 6 (Conflicting Sources) + empathetic delivery

**Expected Content:**
- Acknowledges user's frustration
- Explains crypto = no dispute process
- Why this is different
- No recourse available

**Success Criteria:**
✓ Empathetic (bad news delivery)  
✓ Clear about no options  
✓ Explains why (educational)  
✓ Doesn't give false hope  

---

### Test 8.2: Outdated Info User Thinks is Current

**User Query:**
```
I read that chargebacks cost $15. Is that still accurate?
```

**Expected Response Type:** Template 5 (Outdated Source Warning)

**Expected Content:**
- Acknowledge their source
- Confirm that WAS accurate (March 2023)
- Flag as potentially outdated
- Recommend verification

**Success Criteria:**
✓ Validates user's research  
✓ Provides context (when it was accurate)  
✓ Encourages verification  

---

## Test Category 9: Ambiguous Questions

### Test 9.1: "Dispute" Could Mean Multiple Things

**User Query:**
```
How do I dispute a payment?
```

**Expected Response Type:** Template 2 (Conditional) - clarification needed

**Expected Content:**
- Identifies ambiguity
- Merchant dispute vs P2P dispute vs fraud
- Asks clarifying question OR provides all three
- Helps user identify which applies

**Success Criteria:**
✓ Recognizes ambiguity  
✓ Helps user self-identify scenario  
✓ Provides relevant info for all interpretations  

**Sources to Cite:**
- Refund Policy (merchant disputes)
- Dispute Resolution Process (P2P)
- Unauthorized Transaction Policy (fraud)

---

### Test 9.2: "Verification" - Multiple Contexts

**User Query:**
```
How do I get verified?
```

**Expected Response Type:** Template 2 or 7

**Expected Content:**
- Could mean identity verification OR
- Could mean email/phone verification OR
- Could mean bank verification
- Provide most common (identity verification) with note on others

**Success Criteria:**
✓ Addresses most likely meaning  
✓ Acknowledges other possibilities  

---

## Test Category 10: Stress Testing

### Test 10.1: Completely Out of Scope

**User Query:**
```
How do I reset my Wi-Fi router?
```

**Expected Response Type:** Polite redirect

**Expected Content:**
- Not related to GothPay
- Can't help with this
- Offer GothPay help if needed

**Success Criteria:**
✓ Polite but clear boundary  
✓ Doesn't attempt to answer  
✓ Stays on brand  

---

### Test 10.2: Multiple Errors in One Question

**User Query:**
```
I sent cryptocurrency to the wrong person internationally and want a refund and my payment was also declined.
```

**Expected Response Type:** Clarification needed

**Expected Content:**
- Acknowledge complexity
- Ask for clarification
- Can't have sent crypto AND had payment declined
- Help untangle the situation

**Success Criteria:**
✓ Identifies logical inconsistency  
✓ Asks good clarifying questions  
✓ Helpful not condescending  

---

## Evaluation Rubric

For each test response, rate 1-5 on:

### Accuracy (Does it answer correctly?)
- 5: Completely accurate
- 4: Accurate with minor omissions
- 3: Mostly accurate, some confusion
- 2: Partially accurate
- 1: Inaccurate or misleading

### Completeness (Does it fully answer the question?)
- 5: Fully addresses all parts
- 4: Addresses main parts, minor gaps
- 3: Addresses some parts
- 2: Incomplete answer
- 1: Doesn't really answer

### Citation Quality (Are sources properly cited?)
- 5: Perfect citations with dates and sections
- 4: Good citations, minor formatting issues
- 3: Citations present but lacking detail
- 2: Missing some citations
- 1: No citations or wrong sources

### Clarity (Is it easy to understand?)
- 5: Crystal clear, well-organized
- 4: Clear with minor improvements possible
- 3: Understandable but could be clearer
- 2: Somewhat confusing
- 1: Very confusing

### Helpfulness (Does it help the user take action?)
- 5: User knows exactly what to do next
- 4: Clear next steps with minor ambiguity
- 3: Some guidance but not complete
- 2: Vague guidance
- 1: No actionable steps

### Appropriateness (Is the right template/approach used?)
- 5: Perfect template selection
- 4: Good template with minor improvements
- 3: Acceptable but not ideal
- 2: Wrong template used
- 1: Very inappropriate approach

---

## Success Metrics

**Excellent System (Target):**
- Average score: 4.5+ across all categories
- 90%+ of tests pass all criteria
- No responses with score below 3 in any category
- Proper freshness warnings 100% of time
- Citations present in 100% of responses

**Good System (Acceptable):**
- Average score: 4.0+
- 80%+ of tests pass all criteria
- Freshness warnings 90%+ of time
- Citations present in 95%+ of responses

**Needs Improvement:**
- Average score below 4.0
- Missing citations regularly
- Freshness warnings inconsistent
- Template selection often wrong

---

## Next Steps After Testing

1. **Run each test** and document actual responses
2. **Score each response** using the rubric
3. **Identify patterns** (which templates work best, common failures)
4. **Refine templates** based on results
5. **Update source quality rubric** if needed
6. **Document learnings** for portfolio presentation

---

*Version 1.0 | Last updated: February 1, 2026*
