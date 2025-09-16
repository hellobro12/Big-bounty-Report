# 🔍 Bug Bounty Report

This repository contains a collection of structured vulnerability reports based on real world scenarios practiced in controlled environments like DVWA.

---

## 📄 Reports

- [Reflected XSS – DVWA](./reflected-xss-dvwa-report.md)  
- [SQL Injection – Auth Bypass](./sqli-auth-bypass-report.md)

Each report includes:
- Summary of the vulnerability
- Steps to reproduce
- Impact analysis
- CVSS and OWASP risk rating
- Suggested mitigation

### 🔐 Subdomain Takeover - Mock Report

Added  mock bug bounty report demonstrating how subdomain takeover works.  

Includes:
- DNS misconfiguration walkthrough
- How attackers identify and exploit unclaimed subdomains 
- Sample bug bounty report with proof of concept  


# Vulnerability Topics

- **JWT and SSRF**
- **Stealing OAuth Access Token** 
- **Business Logic vulnerabilities**
  - High-level logic issues  
  - Excessive trust in client-side controls
- **Authentication Bypass via Encryption Oracle**
- **Race Condition**
  - Limit overrun race conditions
  - Multi-endpoint race conditions
  - Exploiting time-sensitive vulnerabilities
- **GraphQL**
  - Accessing private GraphQL post
  - Accidental exposure of private GraphQL field
  - Bypassing GraphQL Brute Force Protections
  - Performing CSRF Exploits Over GraphQL
- **SQL Injection**
  - SQL Injection Vulnerability in WHERE Clause Allowing Retrieval of Hidden Data
  - Exploiting Cache Server Normalization for Web Cache Deception
  - SQLi – get DB version (Oracle)
  - SQLi – get DB version (MySQL/MSSQL)
  - Non-Oracle DB schema extraction, Oracle DB schema extraction, Determine column count, Find text column, Retrieve usernames/passwords
  - Error-based Blind SQLi, Time-based Blind SQLi, Time-based Data Extraction
  - Union attacks to get multiple values, blind SQL injection with conditional responses, and visible error-based SQL injection, filter bypass via XML encoding.
- **NoSQL**
  - Detecting NoSQL injection
  - Exploiting NoSQL injection to extract data
- **API Documentation**
  - Exploiting an API endpoint using documentation
  - Finding and exploiting an unused API endpoint
  - Exploiting server-side parameter pollution in a REST URL
- **LLM API**
  - Exploiting LLM APIs with excessive agency
  - Exploiting vulnerabilities in LLM APIs
  - Indirect Prompt Injection
  - Exploiting XSS through  LLM Chat and Product Reviews
- **Web Cache**
  - Web Cache Deception via Path Mapping
  - Exploiting Path Delimiter for Web Cache Deception
  - Exploiting Origin Server Normalization for Web Cache Deception
  - Exploiting Cache Server Normalization for Web Cache 
  - Web Cache Deception – exact match
- **Cross Site Scripting**
  - Reflected XSS, Stored XSS, DOM XSS using document.write with location.search.
  - DOM XSS in jQuery href (location.search), innerHTML (location.search), jQuery selector (hashchange)
  - Stored XSS into onclick event, Stored XSS into anchor href attribute (double quotes HTML-encoded), Reflected XSS into a JavaScript string (angle brackets in HTML-encoded)
  - Stored DOM XSS, Reflected XSS with Most Tags/Attributes Blocked, HTML Context with All Tags Blocked Except Custom Ones.
  - Reflected XSS with SVG markup allowed, in canonical `<link>` tag, in a JavaScript string with single quote/backslash escaped
  - Reflected XSS in JavaScript string, Stored XSS in onclick event and  XSS to bypass CSRF defenses.
  - Reflected XSS with event handlers and href attributes blocked, in a JavaScript URL with some characters blocked
  - Reflected XSS protected by CSP, with CSP bypass
  - Reflected XSS with AngularJS sandbox escape without strings, sandbox escape and CSP.
  - DOM XSS in document.write inside `<select>`, AngularJS DOM XSS with encoded characters, Reflected DOM XSS via eval().

- **CSRF**
  - CSRF vulnerability with no defenses, where token validation depend on request method, token being present.
  - CSRF where token is not tied to user session, tied to non session cookie.
  - SameSite Lax bypass via method override, SameSite Strict bypass via client-side redirect.
  - CSRF where Referer validation depends on header being present.

   




 

