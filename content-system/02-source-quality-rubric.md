# Source Quality Rubric & Citation Guidelines
**Version:** 1.0  
**Purpose:** Decision framework for evaluating source reliability and constructing citations

---

## Source Quality Evaluation Framework

### Trust Hierarchy

When multiple sources cover the same topic, prioritize in this order:

**Tier 1: Authoritative (Highest Trust)**
- Official policies (POL-* documents)
- Process runbooks (PROC-* documents)
- Updated within last 6 months
- Explicitly marked as "Active" status

**Tier 2: Reliable Reference (Medium-High Trust)**
- FAQ documents
- Updated within last 12 months
- Cross-references official policies
- Marked as "Active" status

**Tier 3: Use with Caution (Medium Trust)**
- Documents 12-24 months old
- Documents without clear update dates
- Beta/experimental features
- Documents marked "Under Review"

**Tier 4: Verify Before Using (Low Trust)**
- Documents over 24 months old
- Documents marked "Outdated" or "Needs Review"
- Deprecated features
- Conflicting with newer sources

**Tier 5: Do Not Use (No Trust)**
- Documents marked "Superseded"
- Archived documents
- Draft documents not marked active
- Personal notes or unofficial sources

---

## Source Selection Decision Tree

```
Question received
│
├─ Is there a Tier 1 source (Official Policy/Runbook)?
│  ├─ Yes → Is it current (< 6 months old)?
│  │  ├─ Yes → USE THIS SOURCE (cite prominently)
│  │  └─ No → Check if Tier 2 source is newer
│  └─ No → Continue to Tier 2
│
├─ Is there a Tier 2 source (FAQ)?
│  ├─ Yes → Is it current (< 12 months old)?
│  │  ├─ Yes → USE THIS SOURCE (cite with context)
│  │  └─ No → Check if sufficient for answer or need to caveat
│  └─ No → Continue to Tier 3
│
├─ Is there a Tier 3 source (Older docs)?
│  ├─ Yes → Can you verify info hasn't changed?
│  │  ├─ Yes → USE WITH WARNING about age
│  │  └─ No → Suggest user verify with support
│  └─ No → Continue to Tier 4
│
└─ Only Tier 4 sources available?
   ├─ Critical info → Cite with strong warning + verification recommendation
   └─ Non-critical → Suggest contacting support for current info
```

---

## Freshness Rules

### Age-Based Citation Requirements

**0-3 months old (Current)**
```
Based on:
• [Doc Title] (updated [Month Year]) — [Section]
```
- No freshness warning needed
- High confidence in accuracy
- Can cite as definitive

**3-6 months old (Recent)**
```
Based on:
• [Doc Title] (updated [Month Year]) — [Section]
```
- No warning needed for stable topics
- Warning for fast-changing topics (fees, limits, beta features)
- Medium-high confidence

**6-12 months old (Moderately Fresh)**
```
Based on:
• [Doc Title] (last updated [Month Year]) — [Section]
```
- Note "last updated" instead of just "updated"
- Warning for time-sensitive info
- Medium confidence
- Consider mentioning: "This is the most recent documentation available."

**12-24 months old (Aging)**
```
Based on:
• [Doc Title] — Last updated [Month Year]

⚠️ This information is over a year old. Verify it's still current by contacting support.
```
- Explicit freshness warning required
- Recommend verification
- Low-medium confidence

**24+ months old (Outdated)**
```
Based on:
• [Doc Title] — ⚠️ Last updated [Month Year] (over 2 years old)

This information is significantly outdated. Contact support for current information:
• [Contact method 1]
• [Contact method 2]
```
- Strong freshness warning required
- Must recommend contacting support
- Low confidence
- Only use if no alternative

---

## Document-Specific Quality Rules

### Policy Documents (POL-*)

**When to cite:**
- ✓ Questions about official rules, eligibility, requirements
- ✓ "Can I..." or "Am I allowed to..." questions
- ✓ Disputes about what policies allow/prohibit

**When NOT to cite:**
- ✗ Technical troubleshooting (use runbooks instead)
- ✗ Quick how-to questions (FAQs faster)
- ✗ Questions about exceptions (policies cover rules, not exceptions)

**Citation format:**
```
According to GothPay's [Policy Name]:
[Policy statement]

Based on:
• [Policy Title] (updated [Month Year]) — [Section Name]
```

---

### Process Runbooks (PROC-*)

**When to cite:**
- ✓ "How do I..." questions requiring step-by-step process
- ✓ Troubleshooting specific problems
- ✓ Understanding workflows and timelines
- ✓ Escalation procedures

**When NOT to cite:**
- ✗ Policy interpretation questions
- ✗ When FAQ has simpler explanation
- ✗ For general conceptual questions

**Citation format:**
```
Here's the standard process for [topic]:
[Steps or process]

Based on:
• [Runbook Title] (updated [Month Year]) — [Section Name]
```

---

### FAQ Documents (FAQ-*)

**When to cite:**
- ✓ Common, straightforward questions
- ✓ When users want quick answer without policy detail
- ✓ "What is..." or "How long..." questions
- ✓ As supplement to policy citations

**When NOT to cite alone:**
- ✗ Complex policy interpretations (use with policy doc)
- ✗ Disputes or formal complaints (need authoritative source)
- ✗ When information seems incomplete

**Citation format:**
```
[Direct answer]

Based on:
• [FAQ Title] (updated [Month Year])

For full details, see the [Related Policy] (POL-XXX).
```

---

### Beta/Limited Features

**Special handling required:**

**Always include availability disclaimer:**
```
⚠️ This is a beta feature available only to select invited users.

[If user likely has access]:
Here's how it works: [explanation]

[If user likely doesn't have access]:
This feature is not currently available on standard accounts. You'll receive an invitation if you're selected for the beta program.

Based on:
• [Beta Doc] (updated [Month Year]) — Beta Features section
```

**Cite conflicts with standard policies:**
```
⚠️ Important: Cryptocurrency payments work differently than standard GothPay payments.

Standard payments: [Policy A applies]
Crypto payments: [Policy B applies - contradicts A]

Based on:
• [Standard Policy] (updated [Month Year])
• [Crypto Beta Policy] (updated [Month Year])
```

---

## Handling Conflicts Between Sources

### Identifying Conflicts

**Type 1: Direct Contradiction**
- Source A says "refunds take 3-5 days"
- Source B says "refunds take 5-10 days"

**Resolution:**
- Use most recent source
- Acknowledge the conflict
- Explain which applies when (if both could be correct in different contexts)

**Type 2: Different Rules for Different Scenarios**
- Not actually a conflict, just different contexts
- Example: Standard payments vs. crypto payments have different rules

**Resolution:**
- Present both clearly
- Explain the key differentiator
- Help user identify which applies to them

**Type 3: Incomplete Information**
- Source A covers topic partially
- Source B covers different aspects
- Together they complete the picture

**Resolution:**
- Synthesize both sources
- Cite both
- Note if gaps remain

---

### Conflict Resolution Priority

**When sources conflict, prioritize:**

1. **Most recent date** (usually more accurate)
2. **Higher tier source** (Policy > FAQ)
3. **More specific source** (Specific policy > General FAQ)
4. **Official status** (Active > Under Review)

**Example:**
- FAQ from January 2025 says $15 chargeback fee
- Policy from March 2023 says $15 chargeback fee
- → Cite FAQ as primary (more recent), note policy for context

**Example 2:**
- Refund Policy (Jan 2025) says "3-5 days"
- FAQ (Oct 2024) says "5-10 days"
- → Cite Refund Policy (more recent AND higher tier)

---

## Citation Patterns

### Single Source Citation

**Basic pattern:**
```
Based on:
• [Document Title] (updated [Month Year]) — [Section Name]
```

**With document ID (rare):**
```
Based on:
• Refund Policy (POL-REF-001, updated January 2025) — Processing Timeline section
```

**With freshness warning:**
```
Based on:
• [Document Title] — ⚠️ Last updated [Month Year]
```

---

### Multiple Source Citations

**Synthesized from multiple sources:**
```
Based on:
• [Doc 1] (updated [Month Year]) — [Section A]
• [Doc 2] (updated [Month Year]) — [Section B]
```

**When sources conflict:**
```
Different sources provide different information:

According to [Doc 1] (updated [Month Year]):
[Info from Doc 1]

However, [Doc 2] (updated [Month Year]):
[Info from Doc 2]

The most recent source ([Doc 1/Doc 2]) is likely most accurate.
```

**Primary + supplementary:**
```
Based on:
• [Primary Doc] (updated [Month Year]) — [Main Section]

Additional context from:
• [Supplementary Doc] (updated [Month Year]) — [Related Section]
```

---

### No Source Available

**When documentation doesn't cover the topic:**
```
I couldn't find information about [topic] in the available GothPay documentation.

[Possible reasons why]

To get an answer:
• Contact support: [method 1]
• [method 2]
• [method 3]
```

**Do NOT:**
- Make up information
- Cite sources that don't actually cover the topic
- Pretend to have information you don't have

---

## Source Quality Rubric Table

| Criteria | High Quality | Medium Quality | Low Quality | Unusable |
|----------|-------------|----------------|-------------|----------|
| **Age** | < 6 months | 6-12 months | 12-24 months | > 24 months |
| **Status** | Active | Active | Under Review | Outdated/Superseded |
| **Type** | Policy/Runbook | FAQ | Beta/Draft | Personal notes |
| **Specificity** | Detailed, specific | General guidance | Vague | Ambiguous |
| **Authority** | Official team | Support team | Community/user | Unverified |
| **Completeness** | Comprehensive | Partial | Gaps | Fragments |
| **Consistency** | Aligns with other docs | Minor discrepancies | Conflicts | Contradicts widely |

---

## Confidence Levels in Responses

### High Confidence (Use definitive language)

**When:**
- Tier 1 source, < 6 months old
- Multiple sources agree
- Clear, unambiguous information

**Language:**
- "The refund will take..."
- "You can..."
- "This policy states..."

**Example:**
```
Your refund will be processed within 3-5 business days to your original payment method.

Based on:
• Refund Policy (updated January 2025) — Processing Timeline
```

---

### Medium Confidence (Use qualifying language)

**When:**
- Tier 2 source, or Tier 1 source 6-12 months old
- Single source without corroboration
- Information seems complete but might have edge cases

**Language:**
- "Typically..."
- "In most cases..."
- "According to the documentation..."
- "This usually takes..."

**Example:**
```
According to the documentation, refunds typically take 3-5 business days. Some users report it can take up to 10 days depending on their bank.

Based on:
• Common Payment Issues FAQ (updated January 2025)
```

---

### Low Confidence (Use cautious language + recommend verification)

**When:**
- Tier 3-4 sources (old or questionable)
- Information seems incomplete or ambiguous
- Conflicting sources without clear resolution

**Language:**
- "Based on available documentation from [date]..."
- "The most recent information suggests..."
- "I recommend verifying this with support..."

**Example:**
```
Based on available documentation from March 2023, the chargeback fee is $15. However, this information is almost 2 years old.

I recommend confirming the current fee by contacting support at 1-800-GOTH-PAY.

Based on:
• Chargeback Handling Guide — ⚠️ Last updated March 2023
```

---

## What NOT to Cite

### Never Cite:

**❌ Information not in sources**
- Don't fabricate citations for general knowledge
- Don't cite documents that don't actually contain the info

**❌ Superseded documents**
- If newer version exists, cite new one only
- Mention old version only if discussing changes

**❌ Draft/unofficial documents**
- Only cite documents marked "Active" or official status
- Drafts may contain errors or outdated info

**❌ User-generated content**
- Comments, forum posts, community wikis
- Even if helpful, not authoritative

**❌ External sources (unless specifically allowed)**
- Don't cite random websites
- Don't cite competitors
- Stick to GothPay's official documentation

---

## Special Citation Scenarios

### Cross-Referencing Related Policies

**When answer requires multiple policies:**
```
For merchant disputes, see the Refund Policy.
For fraud/unauthorized transactions, see the Unauthorized Transaction Policy.

Based on:
• Dispute Resolution Process (updated December 2024) — Types of Disputes

Related policies:
• Refund Policy (POL-REF-001)
• Unauthorized Transaction Policy (POL-UNT-002)
```

---

### Citing Absence of Information

**When policy explicitly excludes something:**
```
GothPay does not currently support international payments.

Based on:
• International Payment Policy (updated January 2025) — Supported Regions

The policy states that only U.S. and select U.S. territories are supported at this time.
```

---

### Citing Changes/Updates

**When policy has recently changed:**
```
As of January 2025, the refund timeline changed from 5-10 days to 3-5 days for card refunds.

Based on:
• Refund Policy (updated January 2025) — Processing Timeline section
```

---

## Citation Quality Checklist

Before finalizing citations, verify:

✅ **Source actually contains the information cited**  
✅ **Update date included**  
✅ **Section name provided** (for users who want to verify)  
✅ **Freshness warnings included** if source is old  
✅ **Conflicts acknowledged** if multiple sources disagree  
✅ **Confidence level matches** source quality  
✅ **No fabricated citations**  
✅ **Most authoritative source used** when multiple available  

---

## Common Citation Mistakes

### Mistake 1: Citing General Source for Specific Info

**Wrong:**
```
Based on: GothPay Help Center
```

**Right:**
```
Based on:
• Refund Policy (updated January 2025) — Merchant Dispute Timeline section
```

---

### Mistake 2: Forgetting Freshness Warnings

**Wrong:**
```
The chargeback fee is $15.

Based on: Chargeback Handling Guide
```

**Right:**
```
According to the most recent documentation (March 2023), the chargeback fee is $15. Please verify this is still current.

Based on:
• Chargeback Handling Guide — ⚠️ Last updated March 2023
```

---

### Mistake 3: Not Stating Assumptions

**Wrong:**
```
You can send up to $10,000 per week.

Based on: Account Limits FAQ
```

**Right:**
```
Premium verified accounts can send up to $10,000 per week.

Based on:
• Account Limits & Verification FAQ (updated October 2024) — Verification Tiers

I assumed you have Premium verification. If you have Basic or Enhanced, your limits are lower.
```

---

### Mistake 4: Citing Conflicting Sources Without Resolution

**Wrong:**
```
Refunds take 3-5 days (Refund Policy) or 5-10 days (FAQ).
```

**Right:**
```
Refunds take 3-5 business days to reach your card issuer according to the most recent policy. The total time including your bank's processing can be 5-10 days.

Based on:
• Refund Policy (updated January 2025) — explains 3-5 days to card issuer
• Common Payment Issues FAQ (updated January 2025) — notes additional bank processing time
```

---

*Version 1.0 | Last updated: February 1, 2026*
