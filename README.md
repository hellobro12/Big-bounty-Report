# 🔍 Bug Bounty Report

This repository contains a collection of structured vulnerability reports based on real-world scenarios practiced in controlled environments like DVWA.

---

## 📄 Reports

- [Reflected XSS – DVWA](./reflected-xss-dvwa-report.md)  
- [SQL Injection – Auth Bypass](./sqli-auth-bypass-report.md)

Each report includes:
- Summary of the vulnerability
- Steps to reproduce
- Impact analysis
- CVSS and OWASP risk ratings
- Suggested mitigations

### 🔐 Subdomain Takeover - Mock Report

Added  mock bug bounty report demonstrating how subdomain takeover works.  

Includes:
- DNS misconfiguration walkthrough
- How attackers identify and exploit unclaimed subdomains (GitHub-based)
- Sample bug bounty report with proof-of-concept  

## Labs

- **JWT and SSRF**
- **Stealing OAuth Access Token** (vulnerability)
- **CSRF** where token is duplicated
- **Business Logic vulnerabilities**
  - High-level logic issues  
  - Excessive trust in client-side controls
- **Authentication Bypass via Encryption Oracle**
- **Race Condition**
  - Lab: Limit overrun race conditions
  - Multi-endpoint race conditions
  - Exploiting time-sensitive vulnerabilities
- **GraphQL**
  - Accessing private GraphQL posts
  - Accidental exposure of private GraphQL fields
  - Bypassing GraphQL Brute Force Protections
  - Performing CSRF Exploits Over GraphQL
- **SQL Injection**
  - SQL Injection Vulnerability in WHERE Clause Allowing Retrieval of Hidden Data
  - Exploiting Cache Server Normalization for Web Cache Deception
  - SQLi – get DB version (Oracle)
  - SQLi – get DB version (MySQL/MSSQL)
  - Non-Oracle DB schema extraction, Oracle DB schema extraction, Determine column count, Find text column, Retrieve usernames/passwords
  - Error-based Blind SQLi, Time-based Blind SQLi, Time-based Data Extraction
  - Union attacks to get multiple values, blind SQL injection with conditional responses, and visible error-based SQL injection,filter bypass via XML encoding.
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
  - Exploiting XSS via LLM Chat and Product Reviews
- **Web Cache**
  - Web Cache Deception via Path Mapping
  - Exploiting Path Delimiters for Web Cache Deception
  - Exploiting Origin Server Normalization for Web Cache Deception
  - Exploiting Cache Server Normalization for Web Cache Deception
  - Web Cache Deception – exact match
- **Cross Site Scripting**
  - Reflected XSS, Stored XSS,DOM XSS using document.write with location.search.
  - DOM XSS in jQuery href (location.search), innerHTML (location.search), jQuery selector (hashchange)
   




 

