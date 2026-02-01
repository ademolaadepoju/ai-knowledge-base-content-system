# Account Security & Verification Policy
**Document ID:** POL-SEC-003  
**Last Updated:** January 20, 2025  
**Owner:** Security & Compliance Team  
**Status:** Active

## Overview
This policy outlines GothPay's account security requirements, identity verification procedures, and best practices to protect user accounts from unauthorized access.

## Account Creation & Verification

### Required Information for Account Creation
All new users must provide:
- **Full legal name**: As it appears on government ID
- **Email address**: Must be verified via confirmation link
- **Phone number**: Must be verified via SMS code
- **Date of birth**: To verify user is 18+ years old
- **Residential address**: For compliance and security purposes

### Identity Verification Levels

**Level 1: Basic Verification (Required for All Accounts)**
- Email and phone verification completed
- Name and date of birth provided
- Limits: $500/week sending, $1,000/week receiving

**Level 2: Enhanced Verification**
- Government-issued ID uploaded (driver's license, passport, state ID)
- Selfie verification (liveness check)
- Address confirmation (utility bill or bank statement)
- Limits: $3,000/week sending, $10,000/week receiving

**Level 3: Premium Verification (Business & High-Volume Users)**
- All Level 2 requirements
- SSN or EIN verification
- Bank account verification (micro-deposits)
- Video verification call (for accounts over $50k annual volume)
- Limits: $10,000/week sending, unlimited receiving

### Document Requirements

**Acceptable Government IDs:**
- U.S. driver's license (all states)
- U.S. passport or passport card
- State-issued ID card
- Permanent resident card (Green Card)
- Military ID

**NOT Acceptable:**
- Student IDs
- Work badges
- Birth certificates
- Social Security cards alone
- Expired documents (must be current)

**Address Verification Documents:**
- Utility bill (electric, water, gas) from last 60 days
- Bank or credit card statement from last 60 days
- Mortgage statement or lease agreement
- Government correspondence (IRS, DMV, etc.)

## Security Features

### Mandatory Security (All Users)
- **Password requirements**: Minimum 12 characters, mix of uppercase, lowercase, numbers, symbols
- **Email verification**: Must click link in verification email
- **Phone verification**: Must enter SMS code
- **Device registration**: Each new device requires approval

### Strongly Recommended (Opt-Out Available)
- **2-Factor Authentication (2FA)**: SMS or authenticator app code required for login
- **Biometric login**: Fingerprint or Face ID on supported devices
- **Transaction notifications**: Instant alerts for all payments
- **Login alerts**: Email notification for new device logins

### Optional Advanced Features
- **Security key**: Hardware security key (YubiKey, etc.) for highest security
- **Trusted contacts**: Designate emergency contacts who can help recover account
- **Geographic restrictions**: Limit account access to specific countries/regions
- **Transaction limits**: Set custom daily/weekly spending limits below account maximums

## Login & Access Security

### Password Requirements
- Minimum 12 characters
- At least one uppercase letter
- At least one lowercase letter  
- At least one number
- At least one special character (!@#$%^&*)
- Cannot contain username or email
- Cannot be a previously used password
- Must be changed every 180 days (optional for users with 2FA enabled)

### Password Reset Process

**Standard Reset:**
1. Click "Forgot Password" on login screen
2. Enter email or phone number
3. Receive verification code via email/SMS
4. Enter code and create new password
5. All devices logged out (must log back in)

**Enhanced Security Reset (If Suspicious Activity Detected):**
1. Standard steps 1-3 above
2. Answer security questions
3. Upload photo of government ID
4. Receive verification call from GothPay (phone verification)
5. Wait 24-48 hours for manual review before reset approved

### 2-Factor Authentication (2FA)

**Setup Process:**
- Enable in Settings > Security > 2-Factor Authentication
- Choose method: SMS codes or authenticator app (Authy, Google Authenticator)
- Enter phone number (for SMS) or scan QR code (for app)
- Verify with test code
- Save backup codes (8 single-use codes for emergencies)

**When 2FA is Required:**
- Every login from new device
- Every login from new location (different city/state)
- After password reset
- When accessing sensitive account settings
- Large transactions (over $1,000)

**Backup Access:**
- **Backup codes**: 8 codes provided at 2FA setup, each usable once
- **Recovery email**: Secondary email that can receive codes if primary unavailable
- **Support verification**: Call support with government ID for manual verification (2-3 business days)

### Biometric Authentication

**Supported Methods:**
- Fingerprint (TouchID, in-display sensors)
- Face recognition (FaceID, facial unlock)
- Iris scanning (select Samsung devices)

**How It Works:**
- Biometric data stored locally on device (never sent to GothPay servers)
- Replaces password entry after initial device login
- Can be disabled anytime in Settings
- Falls back to password if biometric fails 3 times

## Device Management

### Registered Devices
- Users can view all devices with account access in Settings > Devices
- Each device shows: device name, type, last login date, location
- Users can remotely log out or remove devices

### New Device Approval

**When Adding New Device:**
1. Enter email and password
2. Receive "New Device Login" notification on existing trusted device
3. Approve or deny the new device from trusted device
4. If approved, new device becomes trusted
5. If denied, new device blocked and security alert triggered

**If No Existing Trusted Device Available:**
- Must verify via 2FA (SMS or authenticator app)
- Additional email verification required
- 24-hour restriction on sending money from new device

### Lost or Stolen Device

**Immediate Actions:**
1. Use "Lock Account" from another device or web browser
2. Or call GothPay support: 1-800-GOTH-PAY
3. Change password from secure device
4. Remove stolen device from registered devices list

**GothPay's Automatic Protections:**
- All transactions from that device frozen
- Additional verification required for any account changes
- Fraud monitoring increased for 90 days
- User cannot re-add same device without photo ID verification

## Suspicious Activity Detection

### What Triggers Security Alerts

**Login Anomalies:**
- Login from new country
- Login from unusual IP address (VPN, proxy, Tor)
- Multiple failed login attempts (5+ within 1 hour)
- Login from two distant locations in short time (impossible travel)

**Transaction Patterns:**
- Sudden large transaction (10x user's average)
- Rapid sequence of transactions (10+ within 10 minutes)
- First-time transaction to new recipient over $500
- Transaction immediately after password change

**Account Changes:**
- Email or phone number changed
- Bank account or card added
- Shipping address changed
- Security settings downgraded (2FA disabled)

### Automatic Security Responses

**Low Risk (Monitor Only):**
- Email notification to user
- No account restrictions
- Transaction proceeds normally

**Medium Risk (Additional Verification):**
- SMS or email verification code required
- Transaction held for 15-30 minutes
- User must confirm transaction via notification

**High Risk (Temporary Hold):**
- Transaction blocked immediately
- Account sending privileges suspended 24-48 hours
- Must contact support with ID verification to restore access
- Comprehensive account review initiated

## Account Recovery

### Locked Account Recovery

**If User Locked Own Account (Security Precaution):**
- Unlock immediately via 2FA or email verification
- No waiting period
- Full access restored instantly

**If GothPay Locked Account (Fraud Suspicion):**
- Must submit identity verification documents
- Possible phone or video call with verification team
- 1-3 business day review period
- May require additional security measures before restoration

### Forgotten Email/Phone (No Access to 2FA)

**Recovery Process:**
1. Contact support via phone: 1-800-GOTH-PAY
2. Verify identity with:
   - Full name, date of birth, address
   - Last 4 digits of linked bank account or card
   - Recent transaction details
   - Answers to security questions
3. Upload government-issued photo ID
4. Wait 3-5 business days for manual verification
5. Receive temporary access code via phone call to verified number on ID
6. Must update email/phone immediately upon login

### Compromised Account (Unauthorized Access Suspected)
- See **Unauthorized Transaction Policy** (POL-UNT-002) for full procedures
- Immediate account lock
- Fraud investigation initiated
- New security requirements before access restored

## Privacy & Data Protection

### Information GothPay Stores
- Personal information (name, DOB, address, SSN)
- Government ID images (encrypted)
- Transaction history
- Device information and login history
- IP addresses and location data
- Communication preferences

### How Information is Protected
- **Encryption**: All data encrypted at rest and in transit (256-bit AES)
- **Access controls**: Strict employee access limits (need-to-know basis)
- **Audit logs**: All data access logged and reviewed
- **Third-party security**: Annual penetration testing and security audits
- **Compliance**: PCI-DSS, SOC 2, GDPR compliant

### User Data Rights
- **Access**: Request copy of all data GothPay has about you
- **Correction**: Update or correct inaccurate information
- **Deletion**: Request account and data deletion (30-day process)
- **Portability**: Download transaction history and account data
- **Opt-out**: Limit marketing communications and data sharing

## Compliance & Legal Requirements

### Know Your Customer (KYC)
GothPay is required by federal law to:
- Verify identity of all account holders
- Monitor transactions for suspicious activity
- Report certain transactions to FinCEN (Financial Crimes Enforcement Network)
- Maintain records for 5 years

### Anti-Money Laundering (AML)
Transactions may be flagged and investigated if:
- Total monthly volume exceeds $10,000
- Pattern consistent with structuring (avoiding reporting thresholds)
- Transactions to/from high-risk countries
- Customer refuses to provide required information

### Suspicious Activity Reporting (SAR)
GothPay files SARs with federal authorities for:
- Suspected fraud or identity theft
- Transactions with no apparent business purpose
- Customer behavior consistent with money laundering
- Attempted transactions to sanctioned individuals/countries

**Important**: GothPay cannot inform users when a SAR is filed (federal law prohibition)

## Account Closure & Suspension

### Voluntary Account Closure
- User can close account anytime in Settings
- Must withdraw or transfer all funds first
- Outstanding disputes must be resolved
- Account data retained 5 years for compliance
- Can reopen within 90 days; after 90 days must create new account

### Involuntary Suspension or Closure

**Reasons GothPay May Suspend/Close Account:**
- Terms of Service violation
- Fraudulent activity
- AML/compliance concerns
- Excessive chargebacks or disputes
- Abusive behavior toward support staff
- Using account for prohibited businesses (gambling, adult content, etc.)

**User Rights:**
- Email notification with reason for closure (if legally permissible)
- 30 days to withdraw funds
- Option to appeal decision
- Refund of any negative balance not due to fraud

## Related Policies
- See **Unauthorized Transaction Policy** (POL-UNT-002) for fraud reporting
- See **Refund Policy** (POL-REF-001) for transaction disputes
- See **Dispute Resolution Process** (PROC-DIS-001) for appeals

---
*Security questions? Contact security@gothpay.com | Emergency fraud line: 1-800-GOTH-911*
