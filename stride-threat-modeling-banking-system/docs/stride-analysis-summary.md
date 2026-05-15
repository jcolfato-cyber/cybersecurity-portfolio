# STRIDE Threat Analysis Summary

## Overview

This document summarizes the STRIDE threat modeling assessment conducted for the Interest-Free Online Banking System using OWASP Threat Dragon.

The project focused on identifying potential cybersecurity threats affecting authentication, transaction processing, customer data protection, and overall system reliability within an online banking environment.

The STRIDE methodology was used to categorize threats into:

- Spoofing
- Tampering
- Repudiation
- Information Disclosure
- Denial of Service
- Elevation of Privilege

---

## System Components Analysed

The threat model included the following components:

- Customer
- Web Browser
- Online Banking Web Application
- Authentication Service
- Customer Banking Database
- SMS OTP Provider

The architecture also included:

- Internet Trust Boundary
- Internal Secure Network Boundary
- Encrypted communication flows
- Authentication and verification processes

---

## Key Threats Identified

### 1. Credential Spoofing

Attackers may impersonate legitimate users using stolen credentials, phishing attacks, or session hijacking techniques.

**Risk Level:** High

**Mitigations:**

- Multi-Factor Authentication (MFA)
- Strong password policies
- Account lockout controls
- Login anomaly detection

---

### 2. Automated Transaction Abuse

Attackers may exploit banking workflows using automated scripts or bots to abuse transaction processes.

**Risk Level:** High

**Mitigations:**

- Rate limiting
- CAPTCHA protection
- Behavioural monitoring
- Transaction validation controls

---

### 3. Transaction Repudiation

Users may deny performing transactions if proper audit logging and transaction tracking mechanisms are not implemented.

**Risk Level:** Medium

**Mitigations:**

- Centralized audit logging
- Timestamped transaction records
- Secure transaction verification
- SIEM monitoring solutions

---

### 4. Data Interception Attack

Sensitive banking information may be intercepted during transmission through insecure communication channels.

**Risk Level:** High

**Mitigations:**

- HTTPS/TLS encryption
- Certificate validation
- Secure session management
- Token expiration and rotation

---

### 5. Database Scraping and Information Disclosure

Attackers may attempt to extract sensitive customer information from the banking database through automated queries or unauthorized access.

**Risk Level:** High

**Mitigations:**

- Role-Based Access Control (RBAC)
- Database encryption
- Query monitoring
- Least privilege access enforcement

---

### 6. Denial of Service (DoS)

Attackers may overwhelm the application or authentication service with excessive requests, affecting service availability.

**Risk Level:** Critical

**Mitigations:**

- Load balancing
- Traffic filtering
- Request throttling
- DDoS mitigation controls
- Continuous monitoring

---

## Security Recommendations

Based on the STRIDE analysis, the following security improvements are recommended:

- Enforce Multi-Factor Authentication across all customer accounts
- Secure all communication channels using HTTPS/TLS
- Apply Role-Based Access Control and least privilege principles
- Enable centralized logging and monitoring
- Implement anti-automation protections such as CAPTCHA and rate limiting
- Perform continuous vulnerability assessments and patch management
- Introduce DDoS mitigation and resilience controls

---

## Conclusion

The STRIDE threat model provided a structured approach for identifying security risks affecting the online banking platform.

The assessment demonstrated how authentication systems, application logic, communication channels, and databases can be exposed to cybersecurity threats if appropriate controls are not implemented.

Applying the recommended mitigations significantly improves confidentiality, integrity, availability, and accountability within the banking environment while supporting secure and reliable financial operations.
