# GothPay Knowledge Base - Document Catalog

This knowledge base contains documentation for GothPay, a conceptual consumer payment application. These documents serve as the source material for the AI-powered customer support assistant.

## Document Inventory

### Official Policies (HIGH TRUST)

1. **Refund Policy** (`01-refund-policy.md`)
   - Document ID: POL-REF-001
   - Last Updated: January 15, 2025
   - Status: Active
   - Covers: Refund eligibility, processing timelines, merchant vs. P2P payments

2. **Unauthorized Transaction Policy** (`02-unauthorized-transaction-policy.md`)
   - Document ID: POL-UNT-002
   - Last Updated: December 10, 2024
   - Status: Active
   - Covers: Fraud reporting, account takeover, identity theft, zero liability protection

3. **Account Security & Verification Policy** (`03-account-security-verification-policy.md`)
   - Document ID: POL-SEC-003
   - Last Updated: January 20, 2025
   - Status: Active
   - Covers: Identity verification levels, security features, password requirements, 2FA

### Process Runbooks (HIGH TRUST)

4. **Payment Declined Troubleshooting Guide** (`04-payment-declined-troubleshooting.md`)
   - Document ID: PROC-DEC-001
   - Last Updated: November 18, 2024
   - Status: Active
   - Covers: Common decline reasons, decision trees, troubleshooting steps

5. **Dispute Resolution Process** (`05-dispute-resolution-process.md`)
   - Document ID: PROC-DIS-001
   - Last Updated: December 5, 2024
   - Status: Active
   - Covers: P2P disputes, escalation process, evidence collection, appeals

### FAQ Documents (MEDIUM TRUST)

6. **Common Payment Issues FAQ** (`06-common-payment-issues-faq.md`)
   - Document ID: FAQ-PAY-001
   - Last Updated: January 22, 2025
   - Status: Active
   - Covers: Quick answers to frequent questions about payments, fees, limits, refunds

7. **Account Limits & Verification FAQ** (`07-account-limits-verification-faq.md`)
   - Document ID: FAQ-VER-002
   - Last Updated: October 12, 2024
   - Status: Active
   - Covers: Verification tiers, limits, ID requirements, tax reporting

### Special Status Documents

8. **Chargeback Handling Guide** (`08-chargeback-handling-outdated.md`)
   - Document ID: PROC-CHG-001
   - Last Updated: March 15, 2023
   - Status: ⚠️ OUTDATED - NEEDS REVIEW
   - Covers: Chargeback process, fees, why users should avoid chargebacks
   - **Note:** Information may be outdated. Use with caution. Verify current policy with team.

9. **International Payment Policy** (`09-international-payment-policy.md`)
   - Document ID: POL-INTL-001
   - Last Updated: January 18, 2025
   - Status: Active
   - Covers: Geographic restrictions, U.S. territories, travel limitations, future expansion

10. **Cryptocurrency Payment Beta Program** (`10-cryptocurrency-beta-conflicting.md`)
    - Document ID: BETA-CRYPTO-001
    - Last Updated: January 25, 2025
    - Status: ⚠️ BETA - Limited Availability
    - Covers: Crypto buying/selling, wallet management, tax implications
    - **Note:** CONFLICTS with standard refund/dispute policies. Crypto transactions are NOT refundable.

## Document Trust Levels

### HIGH TRUST - Authoritative Sources
Use for definitive answers:
- Official policies (POL-*)
- Process runbooks (PROC-*)
- Recently updated documents (within 6 months)

### MEDIUM TRUST - Quick Reference
Use for general guidance:
- FAQ documents
- May not cover all edge cases
- Good for common questions

### LOW TRUST - Use with Caution
Verify before citing:
- Outdated documents (older than 12 months)
- Beta/experimental features
- Documents marked with ⚠️ warnings

## Source Quality Rubric

| Source Type | When to Cite | When NOT to Cite |
|-------------|--------------|------------------|
| Official Policies | Always (for policy questions) | For technical troubleshooting |
| Runbooks | Always (for process questions) | For policy interpretation |
| FAQs | Quick answers, common issues | Complex disputes, edge cases |
| Outdated Docs | Only with freshness warning | When current info is critical |
| Beta Docs | Only for beta participants | For standard account features |

## Freshness Guidelines

**Up-to-date (< 3 months):**
- Cite without warning
- High confidence

**Moderately Fresh (3-12 months):**
- Cite with "Last updated [date]"
- Medium confidence

**Outdated (12+ months):**
- Cite with "⚠️ Last updated [date]. Verify this is still current."
- Low confidence

**Deprecated/Obsolete:**
- Do not cite
- Suggest user contact support for current information

## Document Relationships

### Cross-References

**Refund Policy** relates to:
- Unauthorized Transaction Policy (fraud vs. merchant disputes)
- Dispute Resolution Process (escalation)
- Payment Declined Guide (failed payments)

**Unauthorized Transaction Policy** relates to:
- Account Security Policy (prevention)
- Dispute Resolution Process (investigation)

**Payment Declined Guide** relates to:
- Account Security Policy (verification requirements)
- Account Limits FAQ (verification levels)

**Cryptocurrency Beta** conflicts with:
- Refund Policy (crypto NOT refundable)
- Dispute Resolution (crypto NOT disputable)
- Unauthorized Transaction Policy (limited fraud protection)

## Known Gaps & Conflicts

### Gaps in Coverage
- **Cryptocurrency for non-beta users**: Standard policies don't address crypto
- **Chargeback updates**: Outdated doc needs current information
- **Business accounts**: Only briefly mentioned, not fully documented

### Policy Conflicts
- **Crypto vs. Standard Payments**: Crypto has NO refund/dispute protection
  - Resolution: When answering crypto questions, explicitly state crypto exceptions
  - Always cite BETA-CRYPTO-001 for crypto-specific queries

- **Chargeback fees**: Outdated doc says $15, may have changed
  - Resolution: Flag as potentially outdated, recommend verifying with support

### Ambiguities
- **"Account in good standing"**: Defined differently across documents
- **International military**: Some contradiction between International Policy and verification docs
- **Beta eligibility**: Cryptocurrency beta mentions "Premium" but doesn't clearly define

## Search Strategy Recommendations

### For Common Questions:
1. Check FAQ documents first (faster, simpler answers)
2. If FAQ doesn't fully answer, check official policies
3. If still unclear, check process runbooks

### For Disputes/Fraud:
1. Start with Unauthorized Transaction Policy (if fraud)
2. Or Refund Policy (if merchant issue)
3. Then Dispute Resolution Process (for escalation/process)

### For Account Issues:
1. Account Security & Verification Policy (for verification)
2. Account Limits FAQ (for quick reference)
3. Payment Declined Guide (for troubleshooting)

### For Edge Cases:
1. Check if special status document exists (crypto, international, etc.)
2. Verify document is current
3. Note any conflicts with standard policies

## AI Assistant Guidelines

### Response Structure Recommendations

Use this structure when answering questions:

```
[Direct answer to question in 1-2 sentences]

[How to do this / Steps if applicable]

[Important limitations or exceptions]

Based on:
• [Doc title] (updated [date]) — [relevant section]

[Any assumptions made or clarifications needed]
```

### Citation Best Practices

**DO:**
- Cite specific sections, not entire documents
- Note document update date for context
- Flag outdated information with warnings
- Acknowledge when sources conflict

**DON'T:**
- Quote long passages (paraphrase instead)
- Cite document IDs (users don't care)
- Assume documents are current without checking date
- Ignore conflicts between documents

### Handling Uncertainty

**If information is unclear:**
- State what IS clear from sources
- Note what's missing or ambiguous
- Suggest contacting support for specifics

**If sources conflict:**
- Acknowledge the conflict
- Present both perspectives
- Recommend which is more likely current (usually most recent)

**If information is outdated:**
- Provide the outdated info with clear warning
- Suggest verifying with support
- Don't present as current fact

## Maintenance Notes

### Update Schedule
- Official policies: Reviewed quarterly
- Process runbooks: Reviewed bi-annually  
- FAQs: Updated as needed (based on support trends)

### Requesting Updates
- Document errors: documentation@gothpay.com
- Policy changes: policy@gothpay.com
- FAQ additions: support@gothpay.com

---

*This catalog last updated: January 25, 2025*
