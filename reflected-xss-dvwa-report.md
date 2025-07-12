# 🐞 Bug Bounty Report – Reflected XSS in DVWA Contact Form
## 🔍 Summary

An attacker can inject malicious JavaScript code into the DVWA contact form input, which is reflected in the response without proper sanitization. This allows arbitrary script execution in the victim’s browser.

## 🧪 Steps to Reproduce

1. Navigate to: `http://localhost/dvwa/vulnerabilities/xss_r/`
2. In the input field, enter the following payload:
   ```html
   <script>alert('XSS')</script>

## 💥 Impact

This vulnerability allows an attacker to execute arbitrary JavaScript in the victim’s browser. If a logged-in user is tricked into clicking a malicious link, the attacker can:

- Steal session cookies
- Perform actions on behalf of the user (e.g., change settings)
- Redirect the user to malicious sites
- Deface the site or deliver malware

This type of vulnerability can lead to full account compromise if session cookies are not protected.

## 📊 Severity: CVSS Score

Using CVSS v3.1, the vulnerability scores as follows:

- **Attack Vector**: Network (0.85)  
- **Attack Complexity**: Low (0.77)  
- **Privileges Required**: None (0.85)  
- **User Interaction**: Required (0.62)  
- **Scope**: Unchanged (0.00)  
- **Impact (CIA)**: Medium  

**Final Score**: 6.1 (Medium Severity)  
[Scored using CVSS Calculator](https://www.first.org/cvss/calculator/3.1)

## ⚖️ Severity: OWASP Risk Rating

| Category        | Value    |
| --------------- | -------- |
| **Likelihood**  | High     |
| **Impact**      | Medium   |
| **Risk Rating** | **High** |

The attack is easy to exploit and common on many forms. The potential impact is significant if session data or credentials are stolen.

## 🛠️ Mitigation

To prevent Reflected XSS vulnerabilities:

- **Sanitize** all user input using a proper encoding library.
- **Escape output** in HTML context (`< > " ' /`) using context-aware escaping.
- Use **Content Security Policy (CSP)** headers to limit what scripts can run.
- Apply **input validation** and reject unexpected data types or symbols.

## 📸 Evidence

### 🔐 Payload Used:
```html
<script>alert('XSS')</script>

