# Chargeback Handling Guide
**Document ID:** PROC-CHG-001  
**Last Updated:** March 15, 2023  
**Owner:** Risk & Chargeback Team  
**Status:** ⚠️ NEEDS REVIEW - OUTDATED

## Overview
This guide explains how GothPay handles chargebacks - when a user disputes a charge directly with their bank or credit card company instead of through GothPay's dispute process.

**IMPORTANT:** Users should always dispute transactions through GothPay first, not their bank. Bank chargebacks result in fees and potential account restrictions.

---

## What is a Chargeback?

A chargeback occurs when a user contacts their bank or credit card issuer to reverse a transaction, rather than going through GothPay's dispute process.

Common chargeback reasons:
- Fraud/unauthorized transaction
- Product not received
- Product not as described
- Duplicate charge
- Processing error

---

## Chargeback Fees

**When User Files Chargeback:**
- **Chargeback fee:** $15 per chargeback
- **Additional fees:** If dispute ruled in user's favor, fee may be refunded
- **Account review:** Multiple chargebacks trigger account review

**Fee Responsibility:**
The user who filed the chargeback is responsible for the $15 fee, even if they win the dispute.

---

## Chargeback Process

### Timeline

**Day 1:** Bank notifies GothPay of chargeback
- Provisional credit issued to user by their bank immediately
- GothPay debits user's account for chargeback amount
- Merchant/recipient notified (if applicable)

**Days 2-10:** Evidence Collection
- User's bank requests evidence from user
- GothPay compiles counter-evidence
- Both submitted to card network (Visa/Mastercard)

**Days 11-45:** Card Network Review
- Visa or Mastercard reviews evidence
- Makes binding decision
- Rarely overturned

**Days 46-60:** Resolution
- If user wins: User keeps provisional credit, GothPay absorbs loss
- If GothPay wins: User must repay bank, GothPay recovers funds
- Decision is final (very limited appeal options)

### User's GothPay Account During Chargeback

**Immediate Actions:**
- Chargeback amount debited from GothPay balance
- If insufficient balance, account goes negative
- $15 chargeback fee assessed
- Sending privileges may be suspended until resolved

**Negative Balance:**
User must bring account to $0+ to restore full functionality:
- Add funds via bank transfer or debit card
- Receive payments (applied to negative balance automatically)
- Account remains restricted until balance positive

---

## Evidence Requirements

### What GothPay Submits to Card Network

For unauthorized transaction chargebacks:
- Login history (IP addresses, devices, timestamps)
- 2FA records (if enabled)
- Communication between user and GothPay
- Previous successful transactions from same device/location

For "goods not received" chargebacks:
- Merchant delivery confirmation
- Tracking information
- Communication between buyer and seller
- Terms of sale/purchase agreement

For "not as described" chargebacks:
- Product listing screenshots
- Merchant descriptions
- Photos provided by merchant
- Return policy information

---

## Why Users Should NOT File Chargebacks

### Problems with Chargebacks:

**1. Fees**
- $15 chargeback fee (non-refundable even if you win)
- Potential interest/fees from bank

**2. Account Restrictions**
- Sending suspended during investigation
- May be locked if multiple chargebacks
- Can result in permanent account closure

**3. Longer Resolution Time**
- GothPay disputes: 10-15 business days
- Chargebacks: 45-90 days typically

**4. Limited Communication**
- GothPay has limited ability to help once bank involved
- Cannot expedite or influence card network decision

**5. Damages Relationship**
- Merchants may refuse future transactions
- May be reported to chargeback monitoring services
- Can affect ability to use other payment services

### The Right Way: GothPay's Dispute Process

**Benefits:**
- No fees for filing dispute
- Faster resolution (usually 10-15 days)
- GothPay mediates between parties
- More nuanced understanding of P2P vs. merchant transactions
- Appeals process available

**How to Start:**
1. Open transaction in app
2. Tap "Report a Problem"
3. Select dispute reason
4. Provide evidence
5. GothPay investigates

---

## Chargeback Prevention

### For Users Sending Money:

**Before Sending:**
- Verify recipient identity (double-check username/email/phone)
- Only send to people you know and trust
- Use GothPay's Purchase Protection when buying goods (if available)
- Save communication/receipts

**Red Flags (Possible Scams):**
- Recipient pressures you to send quickly
- Deal seems too good to be true
- Seller has no reviews or history
- Requests payment as "friends & family" for business transaction

### For Merchants/Recipients:

**Reduce Chargeback Risk:**
- Provide tracking information for shipped items
- Respond quickly to buyer questions/concerns
- Clearly describe products/services
- Have fair return policy
- Communicate proactively about delays

---

## Types of Chargebacks

### Fraud Chargebacks (Unauthorized)

**User Claims:**
"I didn't make this transaction" or "Someone else used my account"

**GothPay's Defense:**
- Login matched user's typical pattern
- 2FA was completed (if enabled)
- Device was previously trusted
- Transaction consistent with user history

**Outcome:**
- If fraud confirmed: User wins, GothPay refunds
- If user authorized: GothPay wins, user repays bank

### Merchant Chargebacks (Service Dispute)

**User Claims:**
"I paid for X but didn't receive it" or "Product not as described"

**GothPay's Defense:**
- Merchant provided tracking showing delivery
- User acknowledged receipt
- Product matched description in listing
- User didn't attempt to resolve with merchant first

**Outcome:**
- Depends heavily on evidence quality
- Card networks favor consumers typically

### Processing Error Chargebacks

**User Claims:**
"I was charged twice" or "Amount was wrong"

**GothPay's Defense:**
- Transaction records show single charge
- Amount matched user authorization
- User clicked "confirm" on correct amount

**Outcome:**
- If genuine duplicate: User wins
- If user error: GothPay wins

---

## Account Actions for Excessive Chargebacks

### Warning Threshold: 2 chargebacks in 6 months
- Email warning sent
- Account reviewed for fraud patterns
- May require additional verification

### Restriction Threshold: 3 chargebacks in 6 months
- Sending privileges suspended 30 days
- Must complete verification call
- May require ID re-verification

### Closure Threshold: 4+ chargebacks in 6 months
- Account permanently closed
- Final balance returned via check (minus fees)
- Cannot create new GothPay account
- Reported to chargeback monitoring services (ChexSystems, etc.)

### Exceptions:
- Chargebacks won by user (proven fraud) don't count toward thresholds
- Chargebacks initiated by bank (not user) may not count
- Account in good standing for 12+ months: counter resets

---

## Chargeback vs. Dispute: Decision Tree

```
Problem with transaction?
│
├─ Is it unauthorized (fraud/account takeover)?
│  ├─ Yes → File report with GothPay immediately (Unauthorized Transaction Policy)
│  │        Also consider reporting to bank if large amount
│  └─ No → Continue
│
├─ Is it a merchant issue (didn't receive item, wrong item, etc.)?
│  ├─ Yes → File dispute with GothPay first (Refund Policy)
│  │        Only go to bank if GothPay dispute fails
│  └─ No → Continue
│
├─ Is it a P2P payment you regret or want back?
│  ├─ Yes → Contact recipient directly (GothPay cannot reverse)
│  │        Chargebacks will NOT work for authorized P2P payments
│  └─ No → Continue
│
└─ Processing error (duplicate charge, wrong amount)?
   └─ Contact GothPay support → Easy fix, no dispute needed
```

---

## Special Scenarios

### User Files Chargeback After GothPay Dispute Denied

**What Happens:**
- User can file chargeback even after losing GothPay dispute
- GothPay submits evidence including dispute decision
- Card network rarely overturns GothPay's decision
- User still charged $15 chargeback fee
- May be seen as abuse of chargeback system

**Recommendation:**
Use GothPay's appeals process instead of chargeback.

### Bank Files Chargeback on Behalf of User (Bank-Initiated)

**What Happens:**
- Sometimes banks automatically file chargebacks for fraud alerts
- User may not have requested it
- User still responsible for chargeback fee
- User should contact bank to explain/cancel if transaction was legitimate

### Chargeback for Subscription Payment

**Special Rules:**
- Must cancel subscription first before disputing charges
- Cannot chargeback future payments without canceling
- If subscription not easily cancelable, stronger chargeback case

---

## FAQs

**Q: Can I file a chargeback instead of a GothPay dispute?**
A: You CAN, but you SHOULDN'T. GothPay disputes are faster, free, and won't risk your account.

**Q: Will filing a chargeback get me banned?**
A: Not for one chargeback if legitimate. Multiple chargebacks (3+) may result in account closure.

**Q: What if GothPay denied my dispute but I still think I'm right?**
A: File an appeal with GothPay first. If appeal denied and you believe you have strong case, chargeback is option but comes with risks.

**Q: How long do I have to file a chargeback?**
A: Card networks allow 60-120 days from transaction date (varies by card type and reason).

**Q: Can merchants dispute chargebacks?**
A: Yes. Merchants can submit evidence through GothPay. Card network decides final outcome.

**Q: If I win a chargeback, do I get the $15 fee back?**
A: No. Chargeback fee is separate processing fee, non-refundable.

---

## Contact Information

**Chargeback Questions:**
- Email: chargebacks@gothpay.com
- Phone: 1-800-GOTH-PAY (ask for Chargeback Team)

**Dispute Instead:**
- In-app: Transaction > Report Problem
- Email: disputes@gothpay.com

---

**Related Policies:**
- Refund Policy (POL-REF-001)
- Unauthorized Transaction Policy (POL-UNT-002)
- Dispute Resolution Process (PROC-DIS-001)

---
*⚠️ This document needs review and updating. Last updated March 2023.*  
*For most current information, consult with Chargeback Team Lead.*
