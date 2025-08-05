# 🛡️ Cybersecurity Internship Task 2 – Phishing Email Analysis

**👨‍💻 Intern:** Koyyana Jai Durga Venkata Sai Ram  
**📅 Task:** 2 – Analyze a Phishing Email Sample  
**🏢 Internship:** Elevate Labs – Cybersecurity

---

## 📧 Sample Phishing Email Used
Content extracted from a publicly available PayPal-themed phishing attempt (included in `phishing-email.txt`).

---

## 🔍 Phishing Indicators (Based on Hints/Mini Guide)

### 1. Sample Email
✔️ Realistic phishing email used targeting PayPal users.

### 2. Spoofed Sender Address
- **Email**: `services@paypal-accounts.com`
- **Actual PayPal Domain**: `paypal.com`
- 🛑 The domain is spoofed using a lookalike pattern.

### 3. Email Header Analysis (Customized Simulation)
The email header was customized to simulate delivery to `alex@flux.com` to create a realistic phishing analysis scenario. Below are the simulated header results:

```
Delivered-To: alex@flux.com
Return-Path: <services@paypal-accounts.com>
Received: from phishing-mailer.fakehost.ru ([198.51.100.23])
        by mail.example.com with ESMTP id 9sdf9sd8f7sdf
        for <alex@flux.com>; Tue, 04 Aug 2025 11:15:00 +0530
Received-SPF: fail (example.com: domain of services@paypal-accounts.com does not designate 198.51.100.23 as permitted sender) client-ip=198.51.100.23;
Authentication-Results: mail.example.com;
        spf=fail smtp.mailfrom=services@paypal-accounts.com;
        dkim=fail header.d=paypal-accounts.com;
        dmarc=fail header.from=paypal-accounts.com
```

✔️ SPF, DKIM, and DMARC validation failed, indicating a spoofed and unauthenticated sender.

### 4. Suspicious Links or Attachments
- Button: **Confirm Your Information**
- Likely leads to a phishing page impersonating PayPal.

### 5. Urgent/Threatening Language
- “Your account will be permanently disabled”
- “You have 24 hours to solve the problem”

### 6. Mismatched URLs
- Display text appears legitimate but likely redirects to a malicious site.

### 7. Spelling/Grammar Issues
- Minor awkward grammar: “confirm all of your account details…”

### 8. Summary of Phishing Traits

| Indicator                     | Present | Notes |
|------------------------------|---------|-------|
| Spoofed sender               | ✅ Yes  | Fake domain |
| Email header issues          | ✅ Yes  | SPF/DKIM fail |
| Suspicious links             | ✅ Yes  | Button present |
| Urgent language              | ✅ Yes  | Fear-based tactics |
| Mismatched URLs              | ✅ Yes  | Link likely masked |
| Spelling/grammar issues      | ✅ Minor | Some awkward phrasing |
| Social engineering tactics   | ✅ Yes  | Uses fear & urgency |

---

## 🛠 Tools Suggested
- [Google Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/)
- [VirusTotal](https://www.virustotal.com/)
- [URLVoid](https://www.urlvoid.com/)

---

## 📂 Repository Structure

```
📁 elevate-task2-phishing-analysis
├── README.md
├── phishing-email.txt
├── simulated-email-header.txt
```

---

## ✅ Outcome
Learned to analyze phishing emails by identifying spoofing, social engineering, and technical red flags using both visual inspection and header analysis techniques.
