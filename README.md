# 📧 Phishing Email Detection & Awareness Report  
## Cyber Security Internship – Future Interns (2026)

---

## 🎯 Objective

This project simulates a corporate phishing investigation engagement.

The goal was to:

- Analyze phishing email samples
- Identify technical and psychological attack indicators
- Classify email risk (Safe / Phishing)
- Provide clear awareness guidance for employees

This task focuses on security awareness and risk communication.

---

# 📊 Executive Summary

Three email samples were analyzed:

| Category | Count |
|----------|-------|
| Phishing | 2 |
| Legitimate | 1 |

Primary phishing techniques identified:

- Domain spoofing (typosquatting)
- Urgency-based manipulation
- Fake verification links
- Email authentication failures (SPF/DKIM/DMARC)

Overall Observation:  
Phishing attacks primarily exploit human psychology rather than technical vulnerabilities.

---

# 🔍 Email Case Analysis

---

## 🔹 Case 01 – PayPal Account Verification (Phishing – High Risk)

**Sender:** support@paypa1.com  
**Subject:** Urgent: Account Access Limited  

### Indicators Identified:

- Domain spoofing (“paypa1” instead of “paypal”)
- Suspicious verification link
- Urgency and fear-based messaging
- SPF Fail / DKIM None / DMARC Fail

### Risk Explanation:

Attackers attempt to trick users into submitting credentials through fake verification portals.

### Final Classification:
**Phishing (High Confidence)**

---

## 🔹 Case 02 – Microsoft Password Expiration (Phishing – High Risk)

**Sender:** security@micr0soft-support.com  
**Subject:** Password Expiration Notice  

### Indicators Identified:

- “micr0soft” domain manipulation
- Fake login page link
- 12-hour urgency pressure
- Email authentication failures

### Risk Explanation:

The attacker aims to capture Microsoft account credentials using a cloned login page.

### Final Classification:
**Phishing (High Confidence)**

---

## 🔹 Case 03 – PayPal Monthly Statement (Legitimate – Safe)

**Sender:** no-reply@paypal.com  
**Subject:** Monthly Account Statement  

### Indicators Identified:

- Correct official domain
- HTTPS official link
- Personalized greeting
- SPF/DKIM/DMARC Pass

### Final Classification:
**Legitimate (Safe)**

---

# 🛡 Common Phishing Indicators

Across analyzed emails, common red flags included:

- Slight domain variations (1 instead of l, 0 instead of o)
- Threat of suspension or account lock
- Immediate action requests
- Short verification deadlines
- Suspicious login URLs
- Authentication failures

---

# 🏢 Business Impact

Successful phishing attacks may result in:

- Credential theft
- Financial fraud
- Account takeover
- Data leakage
- Reputational damage
- Compliance violations

Human error remains the primary attack vector.

---

# 📘 Employee Awareness Guidelines

## ✅ Do:

- Verify sender domain carefully
- Hover over links before clicking
- Access accounts directly through official websites
- Report suspicious emails to IT/Security

## ❌ Do Not:

- Click urgent verification links
- Share passwords or OTP codes
- Download unknown attachments
- Ignore authentication warnings

---

# 🛠 Tools Used

- Public phishing email examples (educational datasets)
- Google Message Header Analyzer
- MXToolbox Email Header Analyzer
- Manual domain inspection
- Browser security checks

---

# ⚖ Ethical Note

All email samples were analyzed in a controlled environment for internship purposes.

No malicious links were accessed.
No exploitation was performed.
