Task 2: Phishing Email Analysis

🎯 Objective
Analyze a suspicious email and identify phishing indicators like spoofed email, fake links, and urgent tone.

🧰 Tools Used
- VirusTotal (for phishing link scan)
- MXToolbox (for email header analysis)
- Manual inspection of body content

📋 Summary

I analyzed a fake Netflix email that asked the user to resubscribe.  
It used a spoofed sender, fake domain, phishing link, and urgent language.  
Header analysis using MXToolbox revealed a forged domain and SPF failure.

✅ Learning Outcome

- How to spot phishing emails
- Use of tools like VirusTotal & MXToolbox
- Importance of header inspection & social engineering awareness

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🛡️ Phishing Email Analysis Report

📩 Sample Phishing Email

From: "Netflix Billing Team" <billing@netflix.com>  
Subject: Action Required: Netflix Subscription Cancelled

Dear Customer,  
We regret to inform you that your Netflix subscription has been cancelled due to a failed payment method.  
Please resubscribe by clicking below:

👉 [https://netflix-resubscribe.ga/verify](https://netflix-resubscribe.ga/verify)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🚨 Phishing Indicators Found

1. **Spoofed Email Domain**  
   - Sender shows as `netflix.com`, but reply-to domain is `netflix-resubscribe.ga` (a fake domain).

2. **Suspicious Link**  
   - Link looks like "netflix.com" but goes to `.ga` domain.

3. **Urgent Tone**  
   - “Your account will be closed in 24 hours” creates pressure.

4. **Generic Greeting**  
   - No name used, says “Dear Customer”.

5. **VirusTotal Result**  
   - 1 engine (Trustwave) flagged the link as suspicious  
   - Screenshot saved: `Screenshot-2025-06-24-211231.png`

6. **MXToolbox Header Result**  
   - Fake server IP: `203.0.113.99`  
   - SPF fail, spam score: 8.1  
   - Screenshot saved: `mx_toolbox_result.png`  
   - Optional screen recording: `Screen Recording 2025-06-24 213422.mp4`

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

 Learnings

- Even real-looking emails can be fake
- Tools like VirusTotal and MXToolbox are essential
- Email headers reveal hidden technical proof of phishing
