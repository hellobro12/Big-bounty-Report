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
- Tools used: `dig`, `subjack`, manual GitHub setup

### Progress

1. Completed a few authentication-related labs in PortSwigger using Burp Suite.  
2. Completed an assignment report on the DVWA machine with three attacks:  
   - Brute Force  
   - Command Injection  
   - File Upload

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
- **Web Cache**
  - Web Cache Deception via Path Mapping



 

