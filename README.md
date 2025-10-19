# Week 5 — Web Attacks: SQL Injection, Subdomain Discovery & CTF Practice

*Status:* Lab / authorized practice only — all testing performed in controlled environments (CTFs, intentionally vulnerable apps, or labs).

---

## Summary
Week 5 focused on web-attack fundamentals and hands-on labs. I practiced *SQL injection techniques*, subdomain discovery, and CTF-style challenges to deepen my ability to discover and safely validate web vulnerabilities.

---

## Key Topics Covered
- SQL Injection basics and enumeration (login bypass, UNION-based enumeration, ORDER BY for column discovery, database fingerprinting)
- Subdomain discovery with *Sublist3r* and content discovery/fuzzing with *ffuf*
- Practical labs and CTF practice (OverTheWire Natas levels; CTF-style flag capture)
- Tools: *Burp Suite, **sqlmap* (lab use only), *Sublist3r, **ffuf, **Kali Linux*

---

## Labs Completed / Evidence
- Multiple SQLi practice labs (enumeration, column discovery, DB version fingerprinting) — documented with notes and screenshots.  
- Subdomain and content discovery exercises using Sublist3r and ffuf.  
- OverTheWire Natas — captured flags through authorized CTF challenges.

*Screenshots included*
- week5-sqli-enum.png — example of lab evidence (sanitized).  
- week5-ffuf-subdomains.png — ffuf / Sublist3r output snapshot.  
- week5-natas-flags.png — proof of flags captured in CTF (lab-only).  
- week5-notes-terminal.png — terminal showing commands & output (for reproducibility).

---

## Tools & Environment
- Kali Linux (VM)  
- Burp Suite Community Edition  
- Sublist3r, ffuf  
- sqlmap (used only in lab contexts)  
- Local vulnerable apps / CTF platforms (Natas, Juice Shop, DVWA, PortSwigger Academy)

---

## Learning Outcomes
- Confidently enumerate SQL injection vectors and determine column counts and DB type via non-destructive techniques in labs.  
- Use automated and manual discovery tools to find public-facing subdomains and hidden endpoints.  
- Apply CTF methodology: discover → enumerate → validate → document.  
- Improved reporting: capture proof, write sanitized findings, and recommend remediation.

---

## Remediation & Defensive Notes
- Use parameterized queries / prepared statements and ORM safe APIs.  
- Apply strict input validation and output encoding.  
- Implement least-privilege DB accounts and disable dangerous DB features.  
- Monitor and alert on abnormal DB queries/transaction patterns.  
- Harden public-facing web services; remove unnecessary endpoints and restrict subdomain exposure.

---

## How to reproduce (safe, high-level)
1. Create an isolated lab (Juice Shop, DVWA, WebGoat, or PortSwigger labs).  
2. Use discovery tools (Sublist3r/ffuf) against lab domain/subdomain.  
3. Observe and document responses; do not test on live/production systems without permission.  

---

## Next steps
- Deepen SQLi skills with PortSwigger SQL labs and Juice Shop scenarios.  
- Practice safe reporting and remediation writeups.  
- Start integrating findings into a public portfolio with sanitized case studies.

---

> *Note:* All materials here are for learn
