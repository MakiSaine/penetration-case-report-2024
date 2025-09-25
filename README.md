# Penetration Case 2024

This repository documents a complete penetration test performed on a deliberately vulnerable web application.  
The target site is a real web application owned by my instructor and intentionally designed to be hacked for training purposes.  

This report was originally created as part of a required assignment, but it has since been reviewed, refined, and formatted into a professional case to showcase methodology, exploitation steps, and security recommendations.

---

## Problem Statement

Modern web applications are common attack targets.  
This project explores how vulnerabilities such as SQL Injection, XSS, and weak authentication can be discovered and exploited in a controlled environment, and how organizations can mitigate such risks before real attackers take advantage of them.

---

## Read the Full Report

📄 **Full Report PDF:**  
[View Full Report](docs/technical-vulnerability-assessment-2024-NO.pdf)

<p><strong><em><span style="color:red">
Note: This report is written in Norwegian.<br>
PS: The PDF opens directly in GitHub’s built-in viewer for easy reading, no download required.
</span></em></strong></p>

---

## Objectives

- Map the attack surface through reconnaissance  
- Identify and exploit vulnerabilities (SQLi, XSS, weak session handling)  
- Demonstrate proof-of-concept exploitation in a safe environment  
- Recommend mitigations based on OWASP Top 10 and NIST CSF  
- Produce clear and professional documentation with evidence  

---

## Methodology

- **Reconnaissance:** Collected information about open ports, login pages, and technologies used  
- **Scanning & Enumeration:** Manual and automated testing (Burp Suite, Nikto)  
- **Exploitation:** Performed SQL Injection and XSS payloads to confirm impact  
- **Documentation:** Collected screenshots and detailed write-ups for each step  
- **Mitigation Recommendations:** Suggested fixes and best practices for secure deployment  

---

## Key Findings

- SQL Injection in login form enabled authentication bypass  
- Reflected XSS could execute attacker-controlled scripts  
- Weak session management risked session hijacking  
- Missing rate limiting allowed brute-force attempts  

---

## Recommended Mitigations

- Use parameterized queries and prepared statements to prevent SQLi  
- Validate and sanitize all user input and apply output encoding  
- Implement secure session management (HttpOnly, Secure flags, short session expiry)  
- Add account lockout or CAPTCHA after multiple failed login attempts  
- Keep all dependencies and web server software updated  

---

## Lessons Learned

This case demonstrated how small configuration mistakes can lead to critical vulnerabilities.  
Working with a real but safe-to-hack web application provided a realistic penetration testing experience and highlighted the importance of layered security and proper patch management.

---

*Created by **Mahamed Maki Saine** – Cybersecurity Enthusiast | Ethical Hacker | AI Learner*

