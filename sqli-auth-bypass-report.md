# 🔓 SQL Injection in DVWA Login Form Bypasses Authentication

## 🔍 Summary

The login form in DVWA's SQL Injection module is vulnerable to SQL injection. By manipulating the input, an attacker can bypass authentication and log in as any user without valid credentials. This exposes sensitive user information and protected application functionality.


## 💥 Impact

This vulnerability allows an attacker to bypass login authentication entirely, gaining access to sensitive areas of the application without valid credentials. An attacker could impersonate users, view confidential data, or perform unauthorized actions. If administrative functions are exposed, it may lead to full system compromise.


## 📊 Severity: CVSS Score

**CVSS v3.1 Base Score**: **9.1 (Critical)**

**Metrics:**
- Attack Vector: Network
- Attack Complexity: Low
- Privileges Required: None
- User Interaction: None
- Scope: Unchanged
- Confidentiality: High
- Integrity: High
- Availability: Low

Final Score: 9.1 (Critical)
Scored using the [CVSS Calculator](https://www.first.org/cvss/calculator/3.1)

## ⚖️ Severity: OWASP Risk Rating

| Category        | Value    |
| --------------- | -------- |
| **Likelihood**  | High     |
| **Impact**      | High     |
| **Risk Rating** | **Critical** |

The vulnerability is extremely easy to exploit and allows unauthorized access to sensitive data and functionality. The risk is considered critical due to the potential for complete authentication bypass and privilege escalation.
