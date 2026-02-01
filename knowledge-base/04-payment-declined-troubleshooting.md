# Payment Declined Troubleshooting Guide
**Document ID:** PROC-DEC-001  
**Last Updated:** November 18, 2024  
**Owner:** Customer Support Operations  
**Status:** Active

## Overview
This runbook helps support agents and users diagnose and resolve declined payment issues. Follow decision trees based on decline reason to resolve issues quickly.

## Common Decline Reasons & Solutions

### 1. Insufficient Funds

**Decline Message:** "Payment declined: insufficient funds"

**What This Means:**
- User's bank account or card doesn't have enough money to cover the payment
- Includes the payment amount PLUS GothPay fees (if applicable)

**Troubleshooting Steps:**

**Step 1: Verify Available Balance**
- Ask user to check their bank/card balance
- Remind them to account for pending transactions not yet reflected in balance
- GothPay fees: Standard transactions are free; instant transfers are 1.5%

**Step 2: Check for Holds**
- Bank may have placed hold on funds (hotel/rental car deposits, pending transactions)
- These holds temporarily reduce available balance
- Solution: Wait for holds to clear (typically 3-7 days) or use different payment method

**Step 3: Alternative Payment Methods**
- Try different linked card or bank account
- Add funds to GothPay balance first, then send payment
- Ask sender to fund GothPay balance via debit card (instant) or bank transfer (1-3 days)

**Prevention:**
- Enable low balance alerts in bank app
- Keep buffer amount in account for fees and pending transactions
- Use GothPay balance for better payment control

---

### 2. Card Declined by Bank

**Decline Message:** "Payment declined by your bank" or "Card authorization failed"

**What This Means:**
- User's bank or card issuer blocked the transaction
- GothPay successfully sent the request, but bank said "no"

**Troubleshooting Steps:**

**Step 1: Contact Bank/Card Issuer**
This is ALWAYS the first step for bank declines.
- Call number on back of card
- Tell them: "I'm trying to make a payment through GothPay and it was declined. Can you approve this merchant?"
- Common reasons banks decline: new merchant, unusual amount, geographic location, fraud prevention

**Step 2: Common Bank-Side Issues**

**Expired Card:**
- Check expiration date on card
- Update card info in GothPay if expired
- May need to wait for new card to arrive

**International Transaction Block:**
- Some banks block international transactions by default
- GothPay processes some payments through international processors
- Bank must enable international transactions or authorize GothPay specifically

**Daily/Monthly Limit Exceeded:**
- Many cards have transaction limits (e.g., $1,000/day, $5,000/month)
- User must wait until limit resets or request temporary increase from bank
- Split payment across multiple days if possible

**Fraud Prevention Block:**
- Bank's automated fraud system flagged transaction as suspicious
- Common triggers: large amount, new merchant, late-night transaction
- Bank can whitelist GothPay or approve specific transaction

**Step 3: Alternative Solutions**
- Try different card from different bank
- Use bank account (ACH) instead of debit/credit card
- Fund GothPay balance first via approved payment method, then send

**GothPay Cannot Fix:**
- Bank declines are entirely controlled by the bank
- GothPay has no ability to override or influence bank's decision
- User MUST contact their bank to resolve

---

### 3. Card Information Incorrect

**Decline Message:** "Invalid card number" or "Card verification failed"

**What This Means:**
- Card number, expiration date, CVV, or ZIP code entered incorrectly
- Card information doesn't match bank's records

**Troubleshooting Steps:**

**Step 1: Verify Card Details**
Ask user to double-check:
- **Card number**: All 15-16 digits, no spaces or dashes
- **Expiration date**: MM/YY format, not MM/DD/YY
- **CVV**: 3-digit code on back (Amex: 4 digits on front)
- **Billing ZIP code**: Must match what's on file with card issuer

**Step 2: Common Entry Errors**
- Typing 'O' (letter) instead of '0' (zero)
- Transposing digits (1234 instead of 1243)
- Using old ZIP code if recently moved
- Entering shipping address ZIP instead of billing address ZIP

**Step 3: Update Card in GothPay**
If card details have changed:
- Remove old card from GothPay
- Add card again with current information
- Verify with small test transaction

**Still Not Working?**
- Card may be deactivated/closed by bank
- Card might be reported lost/stolen
- User should contact bank to verify card status

---

### 4. Account Verification Required

**Decline Message:** "Complete account verification to continue" or "Payment limit reached"

**What This Means:**
- User's account verification level is too low for transaction amount
- User has reached weekly sending limit for their verification level

**Verification Levels & Limits:**

| Level | Requirements | Weekly Sending Limit |
|-------|-------------|---------------------|
| Basic | Email + Phone | $500 |
| Enhanced | + Government ID + Selfie | $3,000 |
| Premium | + SSN/EIN + Bank Verification | $10,000 |

**Troubleshooting Steps:**

**Step 1: Check Current Verification Level**
- Settings > Account > Verification Status
- Shows current level and weekly amount used

**Step 2: Upgrade Verification**

**To Enhanced (Most Common):**
1. Go to Settings > Account > Verify Identity
2. Upload clear photo of government-issued ID (driver's license, passport)
3. Take selfie following on-screen instructions (must be well-lit, no glasses/hats)
4. Enter home address
5. Submit for review (usually approved within 2 hours, up to 24 hours)

**To Premium (High-Volume Users):**
1. Complete Enhanced verification first
2. Provide SSN or EIN (for business accounts)
3. Verify bank account via micro-deposits (2 small deposits, confirm amounts)
4. May require video verification call for accounts with high volume history
5. Review takes 2-3 business days

**Step 3: Weekly Limit Reset**
- Limits reset every Monday at 12:00 AM Pacific Time
- Shows reset date in Settings > Account > Limits
- Cannot be accelerated; must wait for reset or upgrade verification

**Temporary Workaround:**
- Split payment across multiple weeks
- Ask sender to use different payment app for amount exceeding limit
- Use bank transfer (ACH) which has higher limits than card payments

---

### 5. Recipient Account Issues

**Decline Message:** "Cannot send to this recipient" or "Recipient account restricted"

**What This Means:**
- Recipient's GothPay account has issues preventing them from receiving money
- Nothing wrong with sender's account

**Troubleshooting Steps:**

**Step 1: Verify Recipient Information**
- Confirm correct email, phone number, or $GothTag
- Typos are common (extra character, wrong domain)
- Try searching recipient by name to confirm identity

**Step 2: Common Recipient Issues**

**Recipient Account Not Verified:**
- Recipient must verify their email/phone to receive payments
- They'll get notification to complete verification
- Payment held in pending status until verification completed
- Expires after 30 days if not claimed

**Recipient Account Suspended:**
- Recipient violated Terms of Service
- Recipient account flagged for fraud
- Recipient has negative balance or unresolved dispute
- Sender must use different payment method or contact recipient to resolve

**Recipient Blocked Sender:**
- Recipient can block specific users from sending them money
- Privacy feature to prevent unwanted payments
- Sender will NOT be told they were blocked (shows generic error)
- Must contact recipient outside GothPay to resolve

**Recipient At Receiving Limit:**
- Basic accounts: $1,000/week receiving limit
- Enhanced accounts: $10,000/week receiving limit
- Premium accounts: Unlimited receiving
- Recipient must upgrade verification or wait for limit reset

**Step 3: Alternative Solutions**
- Ask recipient to upgrade their account verification
- Wait for recipient's weekly limit to reset (Mondays 12 AM PT)
- Send via different payment method (bank transfer, check, cash app)
- Split payment across multiple weeks

---

### 6. Geographic or Regional Restrictions

**Decline Message:** "Payment not available in this region" or "International payments blocked"

**What This Means:**
- GothPay has restrictions on certain countries, states, or territories
- Sender or recipient location triggers geographic block

**Supported Regions:**
- **United States**: All 50 states ✓
- **U.S. Territories**: Puerto Rico ✓, U.S. Virgin Islands ✓, Guam ✓
- **International**: NOT currently supported ✗

**Troubleshooting Steps:**

**Step 1: Verify Location**
- Check sender's billing address and IP location
- Check recipient's registered account address
- Both must be in supported regions

**Step 2: VPN/Proxy Detection**
- GothPay blocks payments when VPN or proxy detected
- Prevents location spoofing for fraud prevention
- User must disable VPN/proxy and retry
- Use device's actual cellular or WiFi connection

**Step 3: International Transfers**
If either party is international:
- GothPay does NOT support international transfers currently
- Alternative: TransferWise, Western Union, PayPal (international), wire transfer
- Cannot circumvent this restriction; it's a regulatory limitation

**State-Specific Issues:**
Some states have additional money transmission requirements:
- Account verification may take longer in certain states
- Higher verification requirements in: NY, CA, TX
- Not an error; additional compliance needed

---

### 7. Fraud Prevention Block

**Decline Message:** "Transaction flagged for review" or "Payment temporarily blocked"

**What This Means:**
- GothPay's fraud detection system flagged transaction as potentially risky
- Automatic security measure to protect user's account

**Common Triggers:**
- First large payment (e.g., first time sending $500+)
- Payment immediately after password reset
- Payment to new recipient user hasn't paid before
- Unusual time (e.g., 3 AM when user typically uses app during day)
- Login from new location/device before payment

**Troubleshooting Steps:**

**Step 1: Verify Transaction Legitimacy**
Ask user:
- Do you recognize this transaction?
- Is this someone you know and intend to pay?
- Are you being pressured or scammed?

**Red Flags for Scams:**
- Recipient claims to be from IRS, Social Security, tech support
- Payment for "prize" or "lottery" winnings
- Romance scam (met online, never in person)
- Job scam (overpayment, asked to send money back)
- Rental scam (wiring deposit before seeing property)

**Step 2: Security Verification**
User must verify identity to proceed:
- Respond to email or SMS verification code
- May require answering security questions
- Possible photo ID upload for high-risk transactions
- Video call verification for amounts over $5,000

**Step 3: Review Period**
- Low risk: 15-30 minutes, automatic approval after verification
- Medium risk: 1-2 hours, manual review
- High risk: 24-48 hours, comprehensive fraud investigation
- User can cancel payment during review period

**Cannot Be Bypassed:**
- Fraud blocks are mandatory for account safety
- No way to "fast track" or override
- Even verified users subject to fraud monitoring
- Protects user from unauthorized access and scams

---

### 8. Technical Errors

**Decline Message:** "Payment failed - please try again" or "System error"

**What This Means:**
- Temporary technical issue with GothPay, bank connection, or payment processor
- Not a problem with user's account or payment method

**Troubleshooting Steps:**

**Step 1: Basic Troubleshooting**
- Wait 5-10 minutes and try again
- Check GothPay status page: status.gothpay.com
- Update to latest app version (may fix bugs)
- Try from different device (computer vs. phone)

**Step 2: Clear App Cache**

**iOS:**
- Delete and reinstall GothPay app
- Log back in
- Try payment again

**Android:**
- Settings > Apps > GothPay > Storage > Clear Cache
- Clear Data (will need to log in again)
- Try payment again

**Web Browser:**
- Clear browser cookies and cache
- Try different browser (Chrome, Safari, Firefox)
- Disable browser extensions that might interfere
- Try incognito/private mode

**Step 3: Check System Status**
Visit status.gothpay.com for:
- Current outages or incidents
- Scheduled maintenance windows
- Known issues and estimated resolution times
- Subscribe to status updates

**Step 4: Contact Support**
If still failing after troubleshooting:
- Provide transaction details (date/time, amount, recipient)
- Include error message screenshot
- Mention troubleshooting steps already attempted
- Support will investigate backend logs

---

## Quick Decision Tree

```
Payment Declined
│
├─ "Insufficient funds" → Check balance, try different payment method
├─ "Declined by bank" → Contact bank to approve GothPay
├─ "Invalid card" → Verify card number, expiration, CVV, ZIP
├─ "Verification required" → Upgrade account verification level
├─ "Recipient issue" → Ask recipient to check their account status
├─ "Region restricted" → Confirm both parties in supported location
├─ "Flagged for review" → Verify identity, wait for review period
└─ "Technical error" → Wait and retry, check status page, clear cache
```

## Escalation Guidelines

### When to Escalate to Tier 2 Support
- Multiple troubleshooting attempts failed (3+)
- User completed all requested steps but still declined
- Suspected platform-wide issue affecting multiple users
- Transaction amount over $10,000
- VIP or business account holder

### When to Escalate to Fraud Team
- User suspects unauthorized access during declined payment
- Decline occurred during suspected account takeover
- User reports being scammed or pressured to make payment
- Payment to/from sanctioned individual or country

### When to Refer to Bank
- Any decline with "contact your bank" message
- Bank-side fraud holds
- Card issuer blocking specific merchant
- User needs to update information with bank (address, limits)

## Related Documentation
- See **Account Security & Verification Policy** (POL-SEC-003) for verification requirements
- See **Unauthorized Transaction Policy** (POL-UNT-002) for fraud reporting
- See **Refund Policy** (POL-REF-001) for post-payment issues

---
*For immediate payment help: Live chat 24/7 or call 1-800-GOTH-PAY*
