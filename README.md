# 📧 Phishing Email Detection & Awareness Report  
## Cyber Security Internship – Future Interns (2026)

---------------------------------------------------------------------

## 🎯 Objective

This project simulates a corporate phishing investigation engagement.

The goal was to:
- Analyze phishing email samples
- Identify technical and psychological attack indicators
- Classify email risk (Safe / Phishing)
- Provide clear awareness guidance for employees

---------------------------------------------------------------------

## 📊 Executive Summary

Total Emails Analyzed: 3
- Phishing: 2
- Legitimate: 1

Primary attack techniques observed:
- Domain spoofing (typosquatting)
- Urgency-based manipulation
- Fake verification links
- Email authentication failures (SPF/DKIM/DMARC)

Overall Observation:
Phishing attacks exploit human psychology more than technical vulnerabilities.

=====================================================================

🔹 CASE 01 – PAYPAL VERIFICATION (PHISHING – HIGH RISK)

---------------------------------------------------------------------

📧 Phishing Email Sample

Subject: 🚨 Urgent: Account Access Limited Until Verification
From: support@paypa1.com
To: rohithrachapudi@gmail.com

Dear Rachapudi Rohith,

We’ve detected unusual activity on your PayPal account.

Please verify your details immediately:
https://paypal.com-update@is.gd/kU2qKS

Failure to complete within 24 hours may result in suspension.

Regards,
PayPal Account Security Team

---------------------------------------------------------------------

🧠 Red Flags in Email Body

- Fake sender domain (paypa1.com instead of paypal.com)
- URL shortener masking real destination
- Urgency and fear-based messaging
- Brand impersonation

---------------------------------------------------------------------

📨 Header Analysis (Simulated)

Return-Path: <support@paypa1.com>
Received-SPF: fail
Authentication-Results:
    spf=fail;
    dkim=none;
    dmarc=fail

---------------------------------------------------------------------

🚩 Header Red Flags

- SPF authentication failed
- No DKIM signature
- DMARC validation failed
- Sender domain not authorized

---------------------------------------------------------------------

🛡 Final Classification: PHISHING (HIGH CONFIDENCE)

=====================================================================

🔹 CASE 02 – MICROSOFT PASSWORD EXPIRATION (PHISHING – HIGH RISK)

---------------------------------------------------------------------

📧 Phishing Email Sample

Subject: ⚠️ Password Expiration Notice – Action Required
From: security@micr0soft-support.com

Dear User,

Your Microsoft password will expire due to unusual sign-in attempts.

Verify your account within 12 hours:
https://micr0soft-login-security.com/verify

Microsoft Security Team

---------------------------------------------------------------------

🧠 Red Flags in Email Body

- Domain manipulation (micr0soft)
- Fake login page link
- Artificial urgency (12-hour deadline)
- Generic greeting

---------------------------------------------------------------------

📨 Header Analysis (Simulated)

Return-Path: <security@micr0soft-support.com>
Received-SPF: fail
Authentication-Results:
    spf=fail;
    dkim=none;
    dmarc=fail

---------------------------------------------------------------------

🚩 Header Red Flags

- Spoofed sender domain
- SPF failed
- DKIM missing
- DMARC failed

---------------------------------------------------------------------

🛡 Final Classification: PHISHING (HIGH CONFIDENCE)

=====================================================================

🔹 CASE 03 – PAYPAL MONTHLY STATEMENT (LEGITIMATE – SAFE)

---------------------------------------------------------------------

📧 Legitimate Email Sample

Subject: Your Monthly Account Statement – February 2026
From: no-reply@paypal.com

Dear Rohith Rachapudi,

Your monthly PayPal statement is now available.

Access your account securely:
https://www.paypal.com/

Thank you for using PayPal.

---------------------------------------------------------------------

🧠 Indicators Observed

- Correct official domain
- HTTPS official link
- Personalized greeting
- Professional tone

---------------------------------------------------------------------

📨 Header Analysis (Simulated)

Received-SPF: pass
dkim=pass
dmarc=pass

---------------------------------------------------------------------

🚩 Header Review

- SPF authentication passed
- DKIM signature valid
- DMARC validation successful

---------------------------------------------------------------------

🛡 Final Classification: LEGITIMATE (SAFE)

=====================================================================

## 🛡 Common Phishing Indicators Identified

- Slight domain variations (1 instead of l, 0 instead of o)
- Threat of suspension or lock
- Short verification deadlines
- Suspicious login URLs
- Authentication failures

---------------------------------------------------------------------

## 🏢 Business Impact

If users fall victim:
- Credential theft
- Account takeover
- Financial fraud
- Data leakage
- Reputational damage

Phishing targets human trust and urgency.

---------------------------------------------------------------------

## 📘 Employee Awareness Guidelines

DO:
- Verify sender domain carefully
- Hover over links before clicking
- Access accounts directly via official websites
- Report suspicious emails

DO NOT:
- Click urgent verification links
- Share passwords or OTPs
- Trust emails creating panic
- Ignore authentication warnings

---------------------------------------------------------------------

## 🛠 Tools Used

- Public phishing email samples (educational datasets)
- Google Message Header Analyzer
- MXToolbox Email Header Analyzer
- Manual domain inspection
- Browser analysis tools

---------------------------------------------------------------------

## ⚖ Ethical Note

All email samples were analyzed in a controlled environment.
No malicious links were accessed.
No exploitation was performed.

=====================================================================

Final Assessment:
Phishing remains one of the most effective social engineering threats.
User awareness combined with proper SPF/DKIM/DMARC implementation is critical for mitigation.
