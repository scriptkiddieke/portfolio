# 100-Day Junior Pentester Transformation Roadmap

## Executive Overview

This roadmap transforms you from foundational knowledge to junior pentester readiness in 14 weeks. You'll progress from reconnaissance fundamentals through manual testing to real bug submissions, building both technical skills and a professional portfolio.

**Target Outcomes:**
- 25-35 labs/boxes completed
- 3-5 valid bug reports submitted
- Portfolio with 10+ writeups
- Interview-ready GitHub repository
- Practical web & infrastructure testing skills

---

## Weekly Roadmap Overview

| Week | Phase | Core Focus | Key Deliverables |
|------|-------|------------|------------------|
| 1-2 | Foundation | Web fundamentals, HTTP deep dive, recon basics | HTTP proxy proficiency, subdomain enumeration portfolio |
| 3-4 | Web Testing I | OWASP Top 10 (Injection, XSS, Auth) | 5 OWASP Juice Shop flags, first practice report |
| 5-6 | Web Testing II | IDOR, SSRF, business logic, API testing | 3 TryHackMe web rooms, API testing checklist |
| 7-8 | Infrastructure | Network scanning, Linux privilege escalation | 2 HTB Easy boxes, privesc methodology doc |
| 9-10 | Integration | Full engagement simulation, report writing | 2 complete mock assessments with reports |
| 11-12 | Real Targets | Bug bounty recon, triage programs, first submissions | 2-3 bug submissions (any severity) |
| 13-14 | Polish | Portfolio refinement, interview prep, advanced topics | GitHub repo live, resume finalized, 10 writeups |

---

## Detailed Weekly Breakdown

### **WEEK 1: Web Fundamentals & HTTP Mastery**

**Learning Goals:**
- Understand HTTP request/response cycle deeply
- Master Burp Suite/OWASP ZAP proxy tools
- Perform basic reconnaissance on web targets

**Daily Tasks:**

**Day 1** (2.5hr) / (4hr variant)
- *Read:* OWASP Testing Guide v4 - Introduction to Web Testing (1hr)
- *Lab:* Install Burp Suite Community, complete FoxyProxy setup (0.5hr)
- *Practice:* TryHackMe "HTTP in Detail" room (1hr) / (+2hr: Start "Web Fundamentals" path)
- *Note:* Document all HTTP methods and status codes in your notes

**Day 2** (2.5hr) / (4hr)
- *Lab:* Set up OWASP Juice Shop locally via Docker (0.5hr)
- *Practice:* Intercept and modify 10 different requests in Juice Shop (1hr)
- *Reading:* PortSwigger Web Security Academy - "How to use Burp Suite" (1hr)
- *(4hr):* Complete PortSwigger Academy "HTTP Request Smuggling" reading module

**Day 3** (2.5hr) / (4hr)
- *Lab:* TryHackMe "Burp Suite Basics" room (1.5hr)
- *Practice:* Install and configure OWASP ZAP, compare with Burp (1hr)
- *(4hr):* Complete TryHackMe "Burp Suite Repeater" room

**Day 4** (2.5hr) / (4hr)
- *Recon:* Install subfinder, amass, assetfinder tools (0.5hr)
- *Practice:* Perform subdomain enumeration on 3 bug bounty programs from Chaos dataset (1hr)
- *Documentation:* Create recon methodology template (1hr)
- *(4hr):* Add httpx, nuclei to toolkit and scan discovered subdomains

**Day 5** (2.5hr) / (4hr)
- *Lab:* TryHackMe "Passive Reconnaissance" room (1hr)
- *Practice:* Google dorking - find 10 interesting findings on test sites (1hr)
- *Tool practice:* waybackurls + filtering with grep (0.5hr)
- *(4hr):* Complete TryHackMe "Active Reconnaissance" room

**Weekend Day 6** (5hr) / (6hr)
- *Major Lab:* TryHackMe "Content Discovery" room (2hr)
- *Practice:* Run ffuf/dirsearch on 5 different practice targets (2hr)
- *Documentation:* Write your first recon methodology writeup (1hr)
- *(6hr):* Start building automated recon bash script

**Weekend Day 7** (5hr) / (6hr)
- *Review:* Consolidate week's notes, create HTTP reference sheet (1hr)
- *Practice:* Complete PortSwigger Academy "HTTP" labs (all free ones) (3hr)
- *Portfolio:* Set up GitHub repo structure for documentation (1hr)
- *(6hr):* Write detailed HTTP deep-dive blog post for portfolio

**Week 1 Measurable Outcomes:**
✓ Can intercept, read, and modify HTTP traffic fluently
✓ Performed subdomain enumeration on 5+ targets
✓ GitHub repo initialized with first writeup
✓ Personal recon methodology documented

---

### **WEEK 2: Advanced Recon & Information Gathering**

**Learning Goals:**
- Master reconnaissance automation
- Understand DNS, TLS/SSL fingerprinting
- Build repeatable recon workflows

**Day 8** (2.5hr) / (4hr)
- *Reading:* "The Bug Hunter's Methodology" by Jason Haddix (watch conference talk) (1hr)
- *Practice:* Map out full attack surface for 2 bug bounty programs (1.5hr)
- *(4hr):* Document findings in Notion/Obsidian recon tracker

**Day 9** (2.5hr) / (4hr)
- *Tool practice:* nmap fundamentals - scan types, timing, NSE scripts (1hr)
- *Lab:* TryHackMe "Nmap" room (1.5hr)
- *(4hr):* Complete "Nmap Live Host Discovery" + "Nmap Basic Port Scans" rooms

**Day 10** (2.5hr) / (4hr)
- *Lab:* TryHackMe "Shodan.io" room (1hr)
- *Practice:* Use Shodan, Censys to find interesting targets (legal hunting) (1hr)
- *Documentation:* Add OSINT sources to recon methodology (0.5hr)
- *(4hr):* Explore certificate transparency logs (crt.sh) + automation

**Day 11** (2.5hr) / (4hr)
- *Practice:* Build Python script to automate subdomain enumeration + httpx (2hr)
- *Version control:* Push script to GitHub with README (0.5hr)
- *(4hr):* Add Slack/Discord notification to script for automation

**Day 12** (2.5hr) / (4hr)
- *Lab:* TryHackMe "Google Dorking" room (1hr)
- *Practice:* GitHub dorking - find API keys in test repos (use dork collections) (1hr)
- *Reading:* HackerOne disclosed reports - reconnaissance-based bugs (0.5hr)
- *(4hr):* Build custom Google Dork list for your target types

**Weekend Day 13** (5hr) / (6hr)
- *Major Project:* Choose 1 VDP program, perform complete reconnaissance (3hr)
- *Documentation:* Create detailed recon report with findings (2hr)
- *(6hr):* Submit VDP report or publish sanitized version as writeup

**Weekend Day 14** (5hr) / (6hr)
- *Lab:* HackTheBox "Lame" (retired, easy) - focus on enumeration process (4hr)
- *Writeup:* Document methodology, not just flags (1hr)
- *(6hr):* Complete additional HTB "Legacy" box

**Week 2 Measurable Outcomes:**
✓ Custom recon automation script in GitHub
✓ 1 complete recon engagement documented
✓ 2 HTB boxes or equivalent labs completed
✓ Understanding of external attack surface mapping

---

### **WEEK 3: OWASP Top 10 - Injection Vulnerabilities**

**Learning Goals:**
- Identify SQL injection manually (no SQLmap initially)
- Understand command injection contexts
- Practice XSS (reflected, stored, DOM-based)

**Day 15** (2.5hr) / (4hr)
- *Reading:* PortSwigger Academy - "SQL Injection" theory (1hr)
- *Lab:* PortSwigger "SQL injection vulnerability in WHERE clause" (1hr)
- *Practice:* OWASP Juice Shop - find first SQLi flag (0.5hr)
- *(4hr):* Complete 3 more PortSwigger SQLi labs

**Day 16** (2.5hr) / (4hr)
- *Lab:* PortSwigger "Blind SQL injection" labs (2hr)
- *Practice:* DVWA (Damn Vulnerable Web App) SQLi module - all levels (0.5hr)
- *(4hr):* Explore time-based and boolean SQLi manually

**Day 17** (2.5hr) / (4hr)
- *Lab:* TryHackMe "SQL Injection" room (1.5hr)
- *Practice:* Write Python script to detect basic SQLi (1hr)
- *(4hr):* Add error-based SQLi detection to script

**Day 18** (2.5hr) / (4hr)
- *Reading:* Command injection theory - OS command separators (0.5hr)
- *Lab:* PortSwigger "OS command injection" labs (all) (1.5hr)
- *Practice:* DVWA Command Injection module (0.5hr)
- *(4hr):* Find command injection in Juice Shop (use hints if stuck >1hr)

**Day 19** (2.5hr) / (4hr)
- *Reading:* OWASP XSS guide + filter bypass techniques (1hr)
- *Lab:* PortSwigger "Reflected XSS" labs (1.5hr)
- *(4hr):* Complete "Stored XSS" and "DOM XSS" lab sections

**Weekend Day 20** (5hr) / (6hr)
- *Major Lab:* TryHackMe "OWASP Top 10" room (complete Injection sections) (3hr)
- *Practice:* OWASP Juice Shop - find 5 flags related to injection (2hr)
- *(6hr):* Write detailed XSS payload cheat sheet for portfolio

**Weekend Day 21** (5hr) / (6hr)
- *Practice:* PentesterLab "From SQL Injection to Shell" (web for pentester exercises) (3hr)
- *Documentation:* Write your first vulnerability report (practice format) (1hr)
- *Review:* Create personal injection vulnerability checklist (1hr)
- *(6hr):* Attempt TryHackMe "Injection" room with writeup

**Week 3 Measurable Outcomes:**
✓ Can identify and exploit basic SQLi, command injection, XSS
✓ 10+ PortSwigger Academy labs completed
✓ 5 OWASP Juice Shop flags captured
✓ First practice vulnerability report written

---

### **WEEK 4: Authentication & Authorization Flaws**

**Learning Goals:**
- Identify broken authentication mechanisms
- Test for IDOR vulnerabilities
- Understand session management issues

**Day 22** (2.5hr) / (4hr)
- *Reading:* OWASP Authentication Cheat Sheet (1hr)
- *Lab:* PortSwigger "Authentication vulnerabilities" labs (1.5hr)
- *(4hr):* Complete all password-based authentication labs

**Day 23** (2.5hr) / (4hr)
- *Practice:* Test for username enumeration in 3 practice apps (1hr)
- *Lab:* PortSwigger "Multi-factor authentication" bypass labs (1hr)
- *Documentation:* Authentication testing checklist (0.5hr)
- *(4hr):* DVWA "Brute Force" module (all security levels)

**Day 24** (2.5hr) / (4hr)
- *Reading:* IDOR vulnerability patterns (HackerOne reports) (1hr)
- *Lab:* PortSwigger "Access control vulnerabilities" (1.5hr)
- *(4hr):* Complete all horizontal/vertical privilege escalation labs

**Day 25** (2.5hr) / (4hr)
- *Practice:* OWASP Juice Shop - find 3 access control bugs (1.5hr)
- *Tool:* Learn Autorize/AuthMatrix Burp extensions (1hr)
- *(4hr):* Test for IDOR in WebGoat access control lessons

**Day 26** (2.5hr) / (4hr)
- *Lab:* TryHackMe "Authentication Bypass" room (1.5hr)
- *Practice:* Session token analysis - entropy, predictability (1hr)
- *(4hr):* Complete TryHackMe "OWASP Juice Shop" room

**Weekend Day 27** (5hr) / (6hr)
- *Major Lab:* HTB "Bastard" or similar box with auth bypass (4hr)
- *Writeup:* Document authentication testing methodology (1hr)
- *(6hr):* Additional HTB box or TryHackMe authentication path

**Weekend Day 28** (5hr) / (6hr)
- *Practice:* Create test plan for authentication testing (1hr)
- *Lab:* Complete remaining PortSwigger authentication labs (3hr)
- *Portfolio:* Write "Top 5 Authentication Bugs I've Found" blog post (practice) (1hr)
- *(6hr):* Review 20 HackerOne authentication bug reports

**Week 4 Measurable Outcomes:**
✓ Authentication/authorization testing methodology documented
✓ Can identify IDOR, broken auth, session issues
✓ 15+ PortSwigger labs completed (cumulative 25+)
✓ 1 HTB box completed with authentication focus

---

### **WEEK 5: Business Logic & SSRF**

**Learning Goals:**
- Identify business logic flaws
- Test for Server-Side Request Forgery
- Understand race conditions and payment logic bugs

**Day 29** (2.5hr) / (4hr)
- *Reading:* Business logic vulnerability patterns (1hr)
- *Lab:* PortSwigger "Business logic vulnerabilities" (all labs) (1.5hr)
- *(4hr):* OWASP Juice Shop - find 3 business logic bugs

**Day 30** (2.5hr) / (4hr)
- *Reading:* SSRF vulnerability guide (1hr)
- *Lab:* PortSwigger "SSRF" labs (basic + blind) (1.5hr)
- *(4hr):* Complete all SSRF labs including advanced

**Day 31** (2.5hr) / (4hr)
- *Practice:* Test for SSRF in known vulnerable apps (1hr)
- *Lab:* TryHackMe "SSRF" room (1hr)
- *Documentation:* SSRF payload cheat sheet (0.5hr)
- *(4hr):* Research cloud metadata endpoints (AWS, GCP, Azure)

**Day 32** (2.5hr) / (4hr)
- *Reading:* Race condition vulnerabilities in web apps (1hr)
- *Practice:* Use Burp Turbo Intruder for race condition testing (1hr)
- *Lab:* PortSwigger race condition labs (0.5hr)
- *(4hr):* OWASP Juice Shop - race condition challenges

**Day 33** (2.5hr) / (4hr)
- *Lab:* TryHackMe "Overpass" series (business logic focus) (2hr)
- *Review:* Analyze 10 business logic bugs on HackerOne (0.5hr)
- *(4hr):* Create business logic testing checklist

**Weekend Day 34** (5hr) / (6hr)
- *Major Lab:* HTB box with SSRF or business logic (4hr)
- *Alternative:* PentesterLab SSRF exercises (4hr)
- *Writeup:* Document findings (1hr)
- *(6hr):* Additional practice with cloud SSRF scenarios

**Weekend Day 35** (5hr) / (6hr)
- *Practice:* Full test of OWASP Juice Shop with business logic focus (3hr)
- *Documentation:* Write comprehensive business logic testing guide (2hr)
- *(6hr):* Build automated SSRF scanner script (Python)

**Week 5 Measurable Outcomes:**
✓ Can identify business logic flaws and SSRF
✓ Business logic testing methodology documented
✓ 30+ PortSwigger labs completed (cumulative)
✓ Understanding of race conditions and payment logic

---

### **WEEK 6: API Security & Modern Web**

**Learning Goals:**
- Test REST and GraphQL APIs
- Understand JWT vulnerabilities
- Practice API fuzzing and parameter tampering

**Day 36** (2.5hr) / (4hr)
- *Reading:* OWASP API Security Top 10 (1hr)
- *Tool:* Learn Postman for API testing (1hr)
- *Practice:* Explore crAPI (vulnerable API) (0.5hr)
- *(4hr):* Complete crAPI challenges 1-5

**Day 37** (2.5hr) / (4hr)
- *Lab:* PortSwigger "API testing" labs (1.5hr)
- *Practice:* JWT.io - analyze and manipulate tokens (1hr)
- *(4hr):* PortSwigger JWT attack labs (all)

**Day 38** (2.5hr) / (4hr)
- *Reading:* GraphQL security testing guide (1hr)
- *Lab:* TryHackMe "GraphQL" room (or DVWA GraphQL) (1.5hr)
- *(4hr):* Practice GraphQL introspection and injection

**Day 39** (2.5hr) / (4hr)
- *Practice:* API fuzzing with ffuf and custom wordlists (1.5hr)
- *Lab:* Test vAPI (vulnerable API) endpoints (1hr)
- *(4hr):* Build API testing checklist and automation script

**Day 40** (2.5hr) / (4hr)
- *Lab:* Complete remaining crAPI challenges (2hr)
- *Documentation:* API testing methodology (0.5hr)
- *(4hr):* Write API security writeup for portfolio

**Weekend Day 41** (5hr) / (6hr)
- *Major Lab:* HTB box with API component (4hr)
- *Alternative:* TryHackMe API Hacking path (4hr)
- *Writeup:* API testing engagement report (1hr)
- *(6hr):* Additional API security practice

**Weekend Day 42** (5hr) / (6hr)
- *Review:* Consolidate Weeks 1-6 notes (1hr)
- *Practice:* Comprehensive test of one web application (all techniques) (3hr)
- *Portfolio:* Update GitHub with all writeups, ensure 5+ published (1hr)
- *(6hr):* Create video walkthrough of one lab for portfolio

**Week 6 Measurable Outcomes:**
✓ Can test REST and GraphQL APIs
✓ Understanding of JWT vulnerabilities
✓ API testing methodology documented
✓ Portfolio has 5+ writeups on GitHub

**MID-POINT ASSESSMENT:**
- Labs completed: 15-20
- PortSwigger Academy: 35-40 labs
- GitHub writeups: 5-7
- Practice reports written: 2-3

---

### **WEEK 7: Infrastructure - Linux & Privilege Escalation**

**Learning Goals:**
- Master Linux privilege escalation techniques
- Understand common misconfigurations
- Practice enumeration automation

**Day 43** (2.5hr) / (4hr)
- *Reading:* Linux privilege escalation methodology (g0tmi1k's guide) (1hr)
- *Practice:* Set up local Linux VM for testing (0.5hr)
- *Lab:* TryHackMe "Linux PrivEsc" room (1hr)
- *(4hr):* Complete full "Linux PrivEsc" room

**Day 44** (2.5hr) / (4hr)
- *Tool:* Learn LinPEAS, LinEnum enumeration scripts (1hr)
- *Lab:* TryHackMe "Linux PrivEsc Arena" (1.5hr)
- *(4hr):* Practice all SUID/SGID exploitation techniques

**Day 45** (2.5hr) / (4hr)
- *Practice:* Kernel exploits - when and how to use (1hr)
- *Lab:* Exploit cron jobs, PATH hijacking in practice VMs (1.5hr)
- *(4hr):* TryHackMe "Linux Privilege Escalation" advanced challenges

**Day 46** (2.5hr) / (4hr)
- *Lab:* HTB "Shocker" (easy retired box - shellshock) (2hr)
- *Writeup:* Document privilege escalation path (0.5hr)
- *(4hr):* Complete HTB "Bashed" box

**Day 47** (2.5hr) / (4hr)
- *Practice:* Sudo misconfigurations exploitation (GTFOBins) (1hr)
- *Lab:* TryHackMe "Sudo Security Bypass" room (1hr)
- *Documentation:* Linux privesc cheat sheet (0.5hr)
- *(4hr):* Practice NFS, LXD/Docker escape techniques

**Weekend Day 48** (5hr) / (6hr)
- *Major Lab:* HTB "Beep" or "Nibbles" (4hr)
- *Writeup:* Complete methodology documentation (1hr)
- *(6hr):* Additional HTB box with Linux focus

**Weekend Day 49** (5hr) / (6hr)
- *Practice:* Build automated privesc enumeration script (2hr)
- *Lab:* VulnHub boxes - at least 2 Linux machines (3hr)
- *(6hr):* Create video walkthrough of privilege escalation

**Week 7 Measurable Outcomes:**
✓ Linux privilege escalation methodology mastered
✓ 3-4 HTB/VulnHub boxes completed
✓ Custom enumeration script in GitHub
✓ Privesc cheat sheet documented

---

### **WEEK 8: Infrastructure - Windows & Active Directory Basics**

**Learning Goals:**
- Windows privilege escalation fundamentals
- Basic Active Directory enumeration
- Understanding Windows misconfigurations

**Day 50** (2.5hr) / (4hr)
- *Reading:* Windows privilege escalation guide (1hr)
- *Lab:* TryHackMe "Windows PrivEsc" room (1.5hr)
- *(4hr):* Complete full room including all vectors

**Day 51** (2.5hr) / (4hr)
- *Tool:* Learn WinPEAS, PowerUp enumeration (1hr)
- *Practice:* Windows service exploitation (1hr)
- *Lab:* Registry and file permission exploitation (0.5hr)
- *(4hr):* Practice unquoted service paths, DLL hijacking

**Day 52** (2.5hr) / (4hr)
- *Lab:* TryHackMe "Windows PrivEsc Arena" (2hr)
- *Documentation:* Windows privesc cheat sheet (0.5hr)
- *(4hr):* Complete TryHackMe "Steel Mountain" room

**Day 53** (2.5hr) / (4hr)
- *Reading:* Active Directory basics (1hr)
- *Lab:* TryHackMe "Active Directory Basics" room (1.5hr)
- *(4hr):* TryHackMe "Attacking Kerberos" room

**Day 54** (2.5hr) / (4hr)
- *Lab:* HTB "Devel" (easy Windows box) (2hr)
- *Writeup:* Document exploitation path (0.5hr)
- *(4hr):* Complete HTB "Optimum" or "Grandpa"

**Weekend Day 55** (5hr) / (6hr)
- *Major Lab:* HTB "Blue" (EternalBlue) (3hr)
- *Practice:* Windows enumeration on multiple VMs (2hr)
- *(6hr):* Additional Windows-focused HTB box

**Weekend Day 56** (5hr) / (6hr)
- *Lab:* TryHackMe "Attacktive Directory" full room (4hr)
- *Documentation:* Infrastructure testing methodology (1hr)
- *(6hr):* Create comprehensive infrastructure testing checklist

**Week 8 Measurable Outcomes:**
✓ Windows privilege escalation proficiency
✓ Basic AD enumeration skills
✓ 6-8 HTB/TryHackMe boxes completed (cumulative)
✓ Infrastructure methodology documented

---

### **WEEK 9: Integration - Full Engagement Simulation**

**Learning Goals:**
- Conduct complete assessments start-to-finish
- Write professional penetration test reports
- Practice time management and prioritization

**Day 57** (2.5hr) / (4hr)
- *Reading:* Professional pentest report templates (study 3 examples) (1hr)
- *Setup:* Choose target for mock assessment (TryHackMe network/room) (0.5hr)
- *Phase 1:* Reconnaissance and enumeration (1hr)
- *(4hr):* Complete recon, begin vulnerability assessment

**Day 58** (2.5hr) / (4hr)
- *Phase 2:* Vulnerability identification and exploitation (2hr)
- *Documentation:* Screenshot and note all findings (0.5hr)
- *(4hr):* Complete exploitation, begin post-exploitation

**Day 59** (2.5hr) / (4hr)
- *Phase 3:* Post-exploitation and privilege escalation (1.5hr)
- *Documentation:* Evidence collection (1hr)
- *(4hr):* Complete full attack chain documentation

**Day 60** (2.5hr) / (4hr)
- *Reporting:* Write executive summary (1hr)
- *Reporting:* Technical findings section (1.5hr)
- *(4hr):* Complete full professional report

**Day 61** (2.5hr) / (4hr)
- *Reporting:* Remediation recommendations (1hr)
- *Review:* Self-edit and improve report (1hr)
- *Portfolio:* Sanitize and add to GitHub (0.5hr)
- *(4hr):* Create presentation slides for findings

**Weekend Day 62** (5hr) / (6hr)
- *Second Mock Assessment:* Different target type (web vs. infrastructure) (4hr)
- *Fast reporting:* Complete report in 1 day (1hr)
- *(6hr):* Full assessment with detailed technical appendix

**Weekend Day 63** (5hr) / (6hr)
- *Practice:* TryHackMe "Holo" network (or similar multi-machine) (5hr)
- *(6hr):* Complete and document full network compromise

**Week 9 Measurable Outcomes:**
✓ 2 complete mock assessments with reports
✓ Professional report writing skills
✓ Portfolio has 2 full engagement writeups
✓ Time management for assessments practiced

---

### **WEEK 10: Report Writing & Advanced Topics**

**Learning Goals:**
- Refine technical writing
- Explore advanced vulnerability classes
- Prepare for real-world testing

**Day 64** (2.5hr) / (4hr)
- *Reading:* Study 5 HackerOne disclosed reports for writing style (1.5hr)
- *Practice:* Rewrite one of your reports based on learnings (1hr)
- *(4hr):* Create report template with automation (scripts)

**Day 65** (2.5hr) / (4hr)
- *Topic:* Server-Side Template Injection (SSTI) (1hr reading)
- *Lab:* PortSwigger SSTI labs (1.5hr)
- *(4hr):* TryHackMe rooms with SSTI

**Day 66** (2.5hr) / (4hr)
- *Topic:* XML External Entity (XXE) attacks (1hr reading)
- *Lab:* PortSwigger XXE labs (1.5hr)
- *(4hr):* Practice XXE out-of-band techniques

**Day 67** (2.5hr) / (4hr)
- *Topic:* Insecure Deserialization (1hr reading)
- *Lab:* PortSwigger deserialization labs (1.5hr)
- *(4hr):* Java/PHP deserialization practice

**Day 68** (2.5hr) / (4hr)
- *Topic:* CORS and WebSocket vulnerabilities (1hr)
- *Lab:* PortSwigger CORS and WebSocket labs (1.5hr)
- *(4hr):* Additional web cache vulnerabilities

**Weekend Day 69** (5hr) / (6hr)
- *Lab:* HTB "Beep" or similar box with multiple vectors (4hr)
- *Writeup:* Document all identified vulnerabilities (1hr)
- *(6hr):* Additional intermediate HTB box

**Weekend Day 70** (5hr) / (6hr)
- *Review:* Portfolio audit - ensure 8-10 writeups published (2hr)
- *Practice:* Complete any remaining PortSwigger Academy modules (3hr)
- *(6hr):* Build personal vulnerability testing checklist (comprehensive)

**Week 10 Measurable Outcomes:**
✓ Advanced vulnerability classes understood
✓ 50+ PortSwigger labs completed (cumulative)
✓ Portfolio has 8-10 quality writeups
✓ Report writing refined and professional

---

### **WEEK 11: Bug Bounty Preparation**

**Learning Goals:**
- Choose appropriate programs
- Understand scope and rules of engagement
- Perform real reconnaissance legally

**Day 71** (2.5hr) / (4hr)
- *Reading:* "Getting Started in Bug Bounty" guides (multiple sources) (1hr)
- *Research:* Identify 5 suitable programs (VDP or low competition) (1hr)
- *Setup:* Organize tooling for BB (Burp projects, notes system) (0.5hr)
- *(4hr):* Read program policies thoroughly for chosen targets

**Day 72** (2.5hr) / (4hr)
- *Recon:* Full reconnaissance on Program #1 (2hr)
- *Documentation:* Track all subdomains, endpoints, interesting findings (0.5hr)
- *(4hr):* Deep enumeration with all tools

**Day 73** (2.5hr) / (4hr)
- *Testing:* Begin manual testing on Program #1 (2hr)
- *Focus:* Low-hanging fruit (IDOR, XSS, open redirects) (0.5hr)
- *(4hr):* Comprehensive testing across attack surface

**Day 74** (2.5hr) / (4hr)
- *Recon:* Full reconnaissance on Program #2 (2hr)
- *Analysis:* Compare with Program #1 for learning (0.5hr)
- *(4hr):* Automated scanning + manual verification

**Day 75** (2.5hr) / (4hr)
- *Testing:* Manual testing on Program #2 (2hr)
- *Documentation:* Track findings (even duplicates/informational) (0.5hr)
- *(4hr):* Focus on one vulnerability class deeply

**Weekend Day 76** (5hr) / (6hr)
- *Recon + Testing:* Program #3 full assessment (4hr)
- *Review:* Analyze what you're finding vs. missing (1hr)
- *(6hr):* Test additional program or deeper testing

**Weekend Day 77** (5hr) / (6hr)
- *Practice:* Review last 50 disclosed reports for inspiration (2hr)
- *Testing:* Return to Program #1 with fresh perspective (3hr)
- *(6hr):* Focus on business logic and API endpoints

**Week 11 Measurable Outcomes:**
✓ 3 programs thoroughly tested
✓ Complete attack surface mapping for each
✓ At least 1-2 findings ready to report (any severity)
✓ Understanding of program triage preferences

---

### **WEEK 12: First Submissions**

**Learning Goals:**
- Submit first real bug reports
- Handle triaging process
- Deal with duplicates and rejections constructively

**Day 78** (2.5hr) / (4hr)
- *Preparation:* Review best finding from Week 11 (0.5hr)
- *Reporting:* Write first bug report (follow template) (1.5hr)
- *Submission:* Submit to Program #1 (0.5hr)
- *(4hr):* Prepare and submit second finding

**Day 79** (2.5hr) / (4hr)
- *Testing:* Continue testing Program #2 with focus (2hr)
- *Documentation:* Track new findings meticulously (0.5hr)
- *(4hr):* Deep dive into one attack vector (e.g., all API endpoints)

**Day 80** (2.5hr) / (4hr)
- *Reporting:* Write second bug report if finding is valid (1.5hr)
- *Research:* Study how to improve based on similar reports (1hr)
- *(4hr):* Submit second report, begin testing Program #3 deeply

**Day 81** (2.5hr) / (4hr)
- *Testing:* Focus on authentication/authorization in current programs (2hr)
- *Learning:* Review program responses to your reports (0.5hr)
- *(4hr):* Test newly discovered endpoints from recon

**Day 82** (2.5hr) / (4hr)
- *Recon:* Expand to Program #4 or #5 (1.5hr)
- *Testing:* Quick wins hunting (low-hanging fruit) (1hr)
- *(4hr):* Comprehensive testing of one application component

**Weekend Day 83** (5hr) / (6hr)
- *Major Testing:* Deep dive on most promising program (4hr)
- *Goal:* Find at least one medium severity issue (1hr documentation)
- *(6hr):* Test additional applications or programs

**Weekend Day 84** (5hr) / (6hr)
- *Reporting:* Write and submit third bug report (2hr)
- *Practice:* Test 2-3 additional programs for practice (3hr)
- *(6hr):* Create personal "lessons learned" document from submissions

**Week 12 Measurable Outcomes:**
✓ 2-3 bug reports submitted (any severity/status)
✓ Experience with triaging process
✓ 5+ programs tested total
✓ Resilience to duplicates/N/A responses developed

---

### **WEEK 13: Portfolio Building & Skill Refinement**

**Learning Goals:**
- Create professional GitHub portfolio
- Write compelling technical blog posts
- Prepare interview materials

**Day 85** (2.5hr) / (4hr)
- *Portfolio:* Audit all GitHub content for quality (1hr)
- *Writing:* Create README.md with professional summary (1hr)
- *Cleanup:* Ensure all writeups are well-formatted (0.5hr)
- *(4hr):* Add project descriptions, technologies used, outcomes

**Day 86** (2.5hr) / (4hr)
- *Writing:* "My First 100 Days in Bug Bounty" blog post (2hr)
- *Publishing:* Post to Medium/Dev.to (0.5hr)
- *(4hr):* Create second technical blog post on specific vulnerability

**Day 87** (2.5hr) / (4hr)
- *Resume:* Draft penetration tester resume (1.5hr)
- *Content:* Include labs completed, skills, portfolio link (1hr)
- *(4hr):* Create multiple versions (junior pentester, security analyst, etc.)

**Day 88** (2.5hr) / (4hr)
- *Practice:* Continue testing active programs (2hr)
- *Learning:* Review areas where you struggled most (0.5hr)
- *(4hr):* Deep practice in weakest area

**Day 89** (2.5hr) / (4hr)
- *Preparation:* Create interview talking points document (1hr)
- *Practice:* Mock interview questions (technical + behavioral) (1.5hr)
- *(4hr):* Record video explaining one vulnerability for portfolio

**Weekend Day 90** (5hr) / (6hr)
- *Lab Marathon:* Complete 2-3 remaining HTB boxes for portfolio (5hr)
- *(6hr):* Add writeups immediately to GitHub

**Weekend Day 91** (5hr) / (6hr)
- *Writeup Sprint:* Ensure 10+ quality writeups on GitHub (3hr)
- *LinkedIn:* Update profile with new skills and portfolio (1hr)
- *Networking:* Engage with infosec community (Twitter, Discord) (1hr)
- *(6hr):* Create portfolio website with highlights

**Week 13 Measurable Outcomes:**
✓ GitHub portfolio polished and professional
✓ Resume completed and tailored
✓ 10+ writeups published
✓ Interview materials prepared
✓ Blog posts published (1-2)

---

### **WEEK 14: Final Push & Advanced Preparation**

**Learning Goals:**
- Submit additional bug reports
- Master interview preparation
- Plan beyond Day 100

**Day 92** (2.5hr) / (4hr)
- *Testing:* Focus on quality over quantity in programs (2hr)
- *Review:* Check status of all submitted reports (0.5hr)
- *(4hr):* Test new program with fresh perspective

**Day 93** (2.5hr) / (4hr)
- *Lab:* Complete any remaining PortSwigger Academy modules (2hr)
- *Certification Research:* Explore PNPT, eJPT, or OSCP paths (0.5hr)
- *(4hr):* Practice lab if considering certification soon

**Day 94** (2.5hr) / (4hr)
- *Interview Prep:* Practice explaining technical concepts simply (1hr)
- *Preparation:* Create STAR method stories for behavioral questions (1hr)
- *Practice:* Record yourself answering common questions (0.5hr)
- *(4hr):* Mock interview with friend or mentor

**Day 95** (2.5hr) / (4hr)
- *Testing:* Submit final bug report if you have valid finding (1.5hr)
- *Documentation:* Ensure all testing is documented (1hr)
- *(4hr):* Deep testing session on best program

**Day 96** (2.5hr) / (4hr)
- *Review:* Complete metrics tracking (see progress tracker below) (1hr)
- *Planning:* Create Days 101-200 learning plan (1hr)
- *Reflection:* Journal on progress and challenges (0.5hr)
- *(4hr):* Build automation tools for future testing

**Weekend Day 97** (5hr) / (6hr)
- *Final Lab:* Choose challenging HTB box or TryHackMe network (4hr)
- *Writeup:* Complete detailed methodology documentation (1hr)
- *(6hr):* Additional advanced box (Medium difficulty)

**Weekend Day 98** (5hr) / (6hr)
- *Testing Marathon:* Full day testing real bug bounty programs (5hr)
- *(6hr):* Focus on finding one quality bug for portfolio

**Day 99** (2.5hr) / (4hr)
- *Portfolio Final Review:* Ensure everything is polished (1hr)
- *Applications:* Apply to 3-5 junior pentester positions (1.5hr)
- *(4hr):* Customize resumes/cover letters for each application

**Day 100** (2.5hr) / (4hr)
- *Celebration:* Review all accomplishments (0.5hr)
- *Planning:* Set 6-month and 1-year goals (1hr)
- *Community:* Share journey on Twitter/LinkedIn (0.5hr)
- *Testing:* Continue regular bug hunting (0.5hr)
- *(4hr):* Write comprehensive "100 Days" retrospective blog post

**Week 14 Measurable Outcomes:**
✓ All portfolio materials finalized
✓ Job applications submitted
✓ Clear post-100-day plan created
✓ 3-5 total bug submissions completed
✓ Interview-ready confidence

---

## Example Daily Schedules

### **Schedule A: 2.5 hours/weekday, 5 hours/weekend day**

**Weekday Structure:**
```
18:00-18:15 (15min): Review yesterday's notes, set today's goal
18:15-19:15 (60min): Primary learning/lab work (deep focus, no distractions)
19:15-19:30 (15min): Break - walk, stretch, hydrate
19:30-20:15 (45min): Practice/hands-on application
20:15-20:30 (15min): Document findings, update progress tracker
```

**Weekend Structure:**
```
10:00-10:15 (15min): Week review, set session goals
10:15-12:00 (105min): Deep lab work or HTB box
12:00-12:30 (30min): Break - meal, rest
12:30-13:45 (75min): Continuation or writeup
13:45-14:15 (30min): Documentation and portfolio updates
14:15-14:30 (15min): Plan next session
```

### **Schedule B: 4 hours/weekday, 6 hours/weekend day**

**Weekday Structure:**
```
18:00-18:15 (15min): Review and goal setting
18:15-19:30 (75min): Primary learning/reading/theory
19:30-19:45 (15min): Break
19:45-21:00 (75min): Hands-on labs/practice
21:00-21:15 (15min): Break
21:15-21:45 (30min): Additional practice or challenge problems
21:45-22:00 (15min): Documentation and review
```

**Weekend Structure:**
```
10:00-10:15 (15min): Session planning
10:15-12:15 (120min): Major lab/HTB box (uninterrupted)
12:15-13:00 (45min): Lunch break
13:00-14:30 (90min): Continuation, testing, or second lab
14:30-14:45 (15min): Break
14:45-15:45 (60min): Writeup and documentation
15:45-16:00 (15min): Review, update tracker, plan next week
```

---

## Templates & Checklists

### **Daily Progress Log Template**

```markdown
# Day X - [Date]

## Time Spent: [X hours]

## Goals for Today:
- [ ] Goal 1
- [ ] Goal 2
- [ ] Goal 3

## What I Learned:
- 

## Labs/Rooms Completed:
- 

## Challenges Faced:
- 

## How I Overcame Them:
- 

## Bugs/Findings:
- 

## Tomorrow's Focus:
- 

## Energy Level (1-10): 
## Confidence Level (1-10):
```

### **Bug Report Template**

```markdown
# [Vulnerability Type] in [Asset/Endpoint]

## Summary
[2-3 sentence overview of the vulnerability]

## Severity Assessment
**Severity:** [Low/Medium/High/Critical]
**CVSS Score:** [If applicable]
**Impact:** [Data exposure/Account takeover/etc.]
**Likelihood:** [Easy/Medium/Hard to exploit]

## Vulnerable Endpoint
- **URL:** https://target.com/vulnerable/endpoint
- **Parameter:** vulnerable_param
- **HTTP Method:** GET/POST
- **Authentication Required:** Yes/No

## Steps to Reproduce
1. Navigate to [URL]
2. Intercept request with Burp Suite
3. Modify [parameter] to [payload]
4. Send request and observe [result]
5. [Confirm impact]

## Proof of Concept
```http
[Include actual HTTP request/response]
```

[Include screenshots with sensitive data redacted]

## Impact
[Detailed explanation of what an attacker could achieve]
- Impact 1
- Impact 2
- Impact 3

## Suggested Remediation
1. [Specific fix recommendation]
2. [Additional security controls]
3. [Defense-in-depth measures]

## References
- [OWASP link]
- [CWE reference]
- [Similar disclosed reports]

## Your Environment
- Browser: [Chrome 118]
- OS: [Kali Linux 2023.3]
- Tools: [Burp Suite 2023.10.3]
```

### **Vulnerability Triage Checklist**

Before submitting a bug report, verify:

- [ ] **It's actually a vulnerability** (not intended functionality)
- [ ] **You can reproduce it reliably** (at least 3 times)
- [ ] **It's in scope** (check program policy)
- [ ] **You haven't modified data** (only read/view)
- [ ] **Impact is clearly demonstrable**
- [ ] **It's not a duplicate** (search previous reports)
- [ ] **You have clear PoC** (steps + screenshots/video)
- [ ] **Sensitive data is redacted** (passwords, PII, etc.)
- [ ] **Report is professional** (grammar, formatting)
- [ ] **Remediation suggestions included**

### **Web Application Testing Checklist**

```markdown
## Reconnaissance
- [ ] Subdomain enumeration (subfinder, amass, assetfinder)
- [ ] Port scanning (nmap, masscan)
- [ ] Directory/file discovery (ffuf, dirsearch, feroxbuster)
- [ ] JavaScript analysis (LinkFinder, SecretFinder)
- [ ] Wayback machine (waybackurls, gau)
- [ ] Google dorking
- [ ] GitHub/GitLab dorking
- [ ] Certificate transparency logs
- [ ] Shodan/Censys reconnaissance
- [ ] Technology fingerprinting (Wappalyzer, whatweb)

## Authentication & Session Management
- [ ] Username enumeration
- [ ] Weak password policy
- [ ] Brute force protection
- [ ] Password reset flaws
- [ ] Session fixation
- [ ] Session timeout
- [ ] Logout functionality
- [ ] Remember me functionality
- [ ] Multi-factor authentication bypass
- [ ] OAuth/SSO misconfigurations

## Authorization & Access Control
- [ ] Horizontal privilege escalation (IDOR)
- [ ] Vertical privilege escalation
- [ ] Forced browsing to admin functions
- [ ] Missing function-level access control
- [ ] Parameter manipulation
- [ ] Direct object references
- [ ] Role-based access control bypass

## Input Validation
- [ ] SQL injection (error-based, blind, time-based)
- [ ] Cross-Site Scripting (reflected, stored, DOM)
- [ ] Command injection (OS, code injection)
- [ ] XML External Entity (XXE)
- [ ] Server-Side Template Injection (SSTI)
- [ ] LDAP injection
- [ ] XPath injection
- [ ] File inclusion (LFI/RFI)
- [ ] Open redirect

## Business Logic
- [ ] Price/quantity manipulation
- [ ] Race conditions
- [ ] Workflow bypass
- [ ] Payment logic flaws
- [ ] Coupon/discount abuse
- [ ] Referral system abuse
- [ ] Registration workflow flaws
- [ ] Multi-step process bypass

## API Testing
- [ ] Endpoint enumeration
- [ ] Authentication bypass
- [ ] Excessive data exposure
- [ ] Mass assignment
- [ ] Rate limiting
- [ ] GraphQL introspection
- [ ] REST parameter pollution
- [ ] JWT vulnerabilities
- [ ] API versioning issues

## Server-Side Vulnerabilities
- [ ] Server-Side Request Forgery (SSRF)
- [ ] Remote Code Execution
- [ ] File upload vulnerabilities
- [ ] Insecure deserialization
- [ ] XXE injection
- [ ] XSLT injection
- [ ] Server-side includes

## Client-Side Vulnerabilities
- [ ] DOM-based XSS
- [ ] Cross-Site Request Forgery (CSRF)
- [ ] Clickjacking
- [ ] Cross-origin resource sharing (CORS)
- [ ] WebSocket vulnerabilities
- [ ] PostMessage vulnerabilities
- [ ] HTML5 security issues

## Information Disclosure
- [ ] Verbose error messages
- [ ] Debug/development features enabled
- [ ] Sensitive data in source code
- [ ] Backup/old files accessible
- [ ] .git folder exposure
- [ ] API keys in JavaScript
- [ ] Directory listing
- [ ] Comments revealing sensitive info

## Configuration & Deployment
- [ ] Default credentials
- [ ] Missing security headers
- [ ] TLS/SSL misconfigurations
- [ ] Subdomain takeover
- [ ] Cloud storage misconfigurations
- [ ] Content Security Policy bypass
- [ ] CORS misconfigurations
```

### **Infrastructure Testing Checklist**

```markdown
## Reconnaissance
- [ ] Network mapping (nmap -sn)
- [ ] Port scanning (nmap -sV -sC)
- [ ] Service enumeration
- [ ] Operating system detection
- [ ] Banner grabbing
- [ ] SNMP enumeration
- [ ] DNS enumeration
- [ ] SMB enumeration
- [ ] NFS shares enumeration

## Linux Privilege Escalation
- [ ] SUID/SGID binaries (find / -perm -4000 2>/dev/null)
- [ ] Sudo misconfigurations (sudo -l)
- [ ] Cron jobs (/etc/crontab, /var/spool/cron/)
- [ ] Writable /etc/passwd
- [ ] Kernel exploits (uname -a, searchsploit)
- [ ] Capabilities (getcap -r / 2>/dev/null)
- [ ] PATH hijacking
- [ ] LD_PRELOAD
- [ ] NFS no_root_squash
- [ ] Docker escape

## Windows Privilege Escalation
- [ ] Unquoted service paths
- [ ] Service misconfigurations
- [ ] Registry autoruns
- [ ] DLL hijacking
- [ ] Scheduled tasks
- [ ] AlwaysInstallElevated
- [ ] Token impersonation
- [ ] Kernel exploits
- [ ] Stored credentials
- [ ] Group Policy Preferences (GPP)

## Active Directory
- [ ] User enumeration
- [ ] Share enumeration
- [ ] Kerberoasting
- [ ] AS-REP roasting
- [ ] Password spraying
- [ ] GPO abuse
- [ ] Trust relationships
- [ ] Delegation issues
```

---

## Progress Tracking Table

```markdown
| Week | Focus Area | Labs Completed | Bugs Submitted | Bugs Accepted | Writeups | Notes |
|------|-----------|----------------|----------------|---------------|----------|-------|
| 1 | Web Fundamentals | TryHackMe HTTP, Burp Basics | 0 | 0 | 1 | HTTP mastery achieved |
| 2 | Recon | Nmap, Shodan, HTB Lame | 0 | 0 | 2 | Automation script built |
| 3 | OWASP Top 10 - Injection | 10x PortSwigger, Juice Shop | 0 | 0 | 1 | SQLi confidence high |
| 4 | Auth & Access Control | 15x PortSwigger, HTB Bastard | 0 | 0 | 1 | IDOR methodology solid |
| 5 | Business Logic & SSRF | PortSwigger SSRF, TryHackMe | 0 | 0 | 1 | SSRF payload cheat sheet |
| 6 | API Security | crAPI, vAPI, JWT labs | 0 | 0 | 2 | API testing confident |
| 7 | Linux PrivEsc | TryHackMe, HTB Shocker/Beep | 0 | 0 | 2 | 3 HTB boxes completed |
| 8 | Windows PrivEsc | TryHackMe, HTB Blue/Devel | 0 | 0 | 1 | AD basics understood |
| 9 | Full Engagement | 2 mock assessments | 0 | 0 | 2 | Professional reports |
| 10 | Advanced Topics | SSTI, XXE, Deserialization | 0 | 0 | 2 | Portfolio: 8 writeups |
| 11 | BB Preparation | 3 programs tested | 1 | 0 | 1 | First submission! |
| 12 | First Submissions | 5 programs tested | 3 | 1 | 1 | 1 accepted (low) |
| 13 | Portfolio Building | Resume, GitHub polish | 0 | 0 | 2 | 10 writeups total |
| 14 | Final Push | Advanced labs, applications | 1 | 0 | 1 | Job applications sent |
| **TOTAL** | | **25-35** | **4-5** | **1-3** | **20+** | |
```

**Metrics Key:**
- **Labs Completed:** TryHackMe rooms, HTB boxes, PortSwigger modules, practice apps
- **Bugs Submitted:** Total reports sent to bug bounty programs
- **Bugs Accepted:** Reports triaged as valid (any severity)
- **Writeups:** Published documentation (GitHub, blog posts)

---

## Realistic 100-Day KPIs

### **Technical Skills**
- ✅ **Labs/Boxes Completed:** 25-35 (HTB, TryHackMe, VulnHub combined)
- ✅ **PortSwigger Academy:** 50+ labs completed
- ✅ **OWASP Practice Apps:** 15+ flags (Juice Shop, WebGoat, DVWA, crAPI)
- ✅ **Vulnerabilities Practiced:** All OWASP Top 10 + 5 advanced classes

### **Bug Bounty**
- ✅ **Programs Tested:** 5-8 programs thoroughly
- ✅ **Bug Reports Submitted:** 3-5 (realistic for beginners)
- ✅ **Accepted Reports:** 1-3 (any severity, including informational)
- ✅ **Target Vulnerabilities:** Focus on IDOR, XSS, authentication flaws, info disclosure

### **Portfolio**
- ✅ **GitHub Writeups:** 10-15 quality technical writeups
- ✅ **Blog Posts:** 2-3 published articles
- ✅ **Professional Reports:** 2-3 complete penetration test reports
- ✅ **Resume:** Tailored for junior pentester roles

### **Realistic First Bug Targets**
1. **Information Disclosure** (low/medium severity)
   - Verbose error messages
   - Exposed sensitive endpoints
   - Debug information leakage

2. **Insecure Direct Object References (IDOR)** (medium/high severity)
   - User profile access
   - Document/file access
   - API endpoint manipulation

3. **Cross-Site Scripting (XSS)** (low/medium severity)
   - Reflected XSS in search parameters
   - Stored XSS in user inputs
   - DOM-based XSS

4. **Authentication/Authorization Flaws** (medium/high severity)
   - Password reset token issues
   - Account enumeration
   - Privilege escalation

5. **Open Redirects** (low severity - but easy to find)
   - URL parameter manipulation
   - OAuth redirect_uri issues

---

## Habit Stack & Discipline Framework

### **Daily Habits**

**Morning Routine (Optional - before work/study):**
```
☕ Coffee/Tea → 15min security news (Twitter, Reddit r/netsec)
```

**Evening Study Routine:**
```
🚪 Arrive at study space → Review yesterday's notes (5min)
📚 Set single clear goal → Deep work session (Pomodoro: 25min focus, 5min break)
📝 Document learning → Update progress tracker (5min)
🎯 Plan tomorrow → Quick review before bed
```

**Weekend Routine:**
```
🌅 Morning: Longer lab sessions (2-3 hours uninterrupted)
🍱 Midday: Break, reflect, light practice
📄 Afternoon: Documentation, writeups, portfolio work
```

### **Timeboxing Strategy**

- **Theory/Reading:** Never more than 60min without practice
- **Labs:** Timebox HTB boxes to 2-4 hours; flag if stuck >3 hours
- **Bug Hunting:** 1-hour focused sessions per target
- **Documentation:** Immediate (same day as work) - never skip!

### **Avoiding Burnout**

**Yellow Flags (Take a break):**
- Frustration lasting >30 minutes
- Skipping documentation for 2+ days
- Avoiding labs because "too hard"
- Comparing yourself negatively to others

**Reset Strategies:**
- **Micro-break:** 5-min walk, stretch, water
- **Macro-break:** Take full evening off, watch conference talks passively
- **Pivot:** Stuck on web? Do infrastructure. Stuck on labs? Do bug hunting.
- **Social:** Join Discord communities, ask questions, help others

**Weekly Retrospective (Sunday evening, 30min):**
```markdown
## Week [X] Retrospective

### What went well?
-

### What was challenging?
-

### What did I learn?
-

### What will I change next week?
-

### Energy level this week (1-10):
### Confidence level this week (1-10):
```

### **Maintaining Momentum**

**When Motivation is Low:**
1. **Do the minimum:** Just 30 minutes, just one room
2. **Easy win:** Repeat a solved lab, get the confidence boost
3. **Community:** Watch others' writeups, join live streams
4. **Remember why:** Review your Day 1 goals

**When You're Stuck:**
1. **15-minute rule:** Struggle for 15min, then check hint/writeup
2. **Learn from solutions:** Understanding > solving blind
3. **Document failures:** "What I tried and why it didn't work" is valuable
4. **Ask for help:** TryHackMe Discord, HTB forums, Twitter

**Celebration Milestones:**
- ✨ Every 5 labs completed → Treat yourself
- ✨ First bug submission → Share on Twitter
- ✨ First acceptance → Celebrate properly!
- ✨ Week 7 (halfway) → Review and reward
- ✨ Day 100 → Major celebration and reflection

---

## "What to Do If Stuck" Troubleshooting Guide

### **Stuck on a Lab/Box**

**Time-Based Approach:**
- **0-30 minutes:** Try everything you know, enumerate thoroughly
- **30-60 minutes:** Re-read room description, check for hints
- **60-90 minutes:** Google the specific service/technology vulnerability
- **90+ minutes:** Check writeup for just the next step, not full solution

**Specific Scenarios:**

**"Can't find anything to exploit"**
- → Go back to enumeration (80% of pentesting is recon)
- → Run LinPEAS/WinPEAS again, read output carefully
- → Check for hidden directories, backup files, comments in source

**"Exploit isn't working"**
- → Check your payload syntax carefully
- → Verify target architecture (x86 vs x64, Python version, etc.)
- → Try different exploit variants
- → Check if IDS/firewall is blocking

**"Privilege escalation stuck"**
- → Upload and run enumeration scripts
- → Check GTFOBins/LOLBAS for installed binaries
- → Verify file permissions carefully (ls -la)
- → Check running processes, scheduled tasks

### **Stuck on Bug Bounty**

**"Not finding anything"**
- → Expand reconnaissance (more subdomains, endpoints, parameters)
- → Test simpler vulnerability classes (IDOR, open redirects)
- → Read recent disclosed reports for inspiration
- → Try a different program or asset type

**"Everything is duplicate"**
- → Focus on less-tested areas (mobile apps, APIs, documentation sites)
- → Combine vulnerabilities for higher impact
- → Test business logic specific to that company
- → Check newly added scope items

**"Reports getting rejected"**
- → Re-read program policy carefully
- → Improve PoC quality (clearer steps, better screenshots)
- → Ensure impact is clearly demonstrated
- → Check if it's truly a security issue vs. design decision

### **Stuck on Understanding**

**"Concept doesn't make sense"**
- → Watch YouTube video explanations
- → Try hands-on practice first, theory second
- → Draw diagrams of the attack flow
- → Teach it to someone (rubber duck method)

**Resources for Unsticking:**
- **IppSec YouTube:** HTB box walkthroughs
- **John Hammond:** TryHackMe and CTF explanations
- **NahamSec/STÖK:** Bug bounty methodologies
- **PortSwigger Blog:** In-depth vulnerability explanations
- **HackTricks:** Comprehensive pentesting wiki

---

## Interview & Portfolio Talking Points

### **After 100 Days, You Can Say:**

**Technical Competencies:**
- "I've completed 30+ hands-on cybersecurity labs including HackTheBox, TryHackMe, and vulnerable web applications"
- "I can perform web application penetration testing including testing for OWASP Top 10 vulnerabilities"
- "I have practical experience with Burp Suite, nmap, metasploit, and various enumeration tools"
- "I've successfully identified and reported [X] security vulnerabilities through responsible disclosure"
- "I can perform Linux and Windows privilege escalation using manual techniques and enumeration scripts"

**Project Highlights:**
- "Built custom reconnaissance automation tools in Python, available on my GitHub"
- "Documented complete penetration testing methodologies in 10+ detailed writeups"
- "Wrote professional penetration test reports for simulated engagements"
- "Active contributor to bug bounty programs with [X] validated findings"

**Learning & Growth:**
- "Completed 100-day intensive self-study program covering web security, infrastructure testing, and bug bounty hunting"
- "Self-directed learner who can quickly adapt to new technologies and attack vectors"
- "Experienced in researching vulnerabilities, reading CVEs, and understanding exploit code"
- "Active in cybersecurity community through writeups, blog posts, and knowledge sharing"

### **Behavioral Interview Stories (STAR Method)**

**Story 1: Problem-Solving**
- **Situation:** While completing a HackTheBox machine, I was stuck for hours on privilege escalation
- **Task:** Needed to find a path from low-privileged user to root access
- **Action:** Went back to basics, re-ran enumeration scripts, checked every SUID binary, and discovered a custom application with exploitable permissions
- **Result:** Successfully rooted the machine and documented a complete methodology for others

**Story 2: Continuous Learning**
- **Situation:** Initially struggled with understanding SQL injection blind exploitation techniques
- **Task:** Needed to master this for both labs and real-world testing
- **Action:** Practiced on 15+ different labs, wrote custom Python scripts to automate detection, created comprehensive notes
- **Result:** Now confident in identifying and exploiting SQL injection in various contexts

**Story 3: Responsible Disclosure**
- **Situation:** Found a potential security vulnerability in a bug bounty program
- **Task:** Report it professionally and ensure it was properly communicated
- **Action:** Created detailed report with clear PoC, impact analysis, and remediation recommendations following industry standards
- **Result:** Vulnerability accepted and triaged [or "learned from rejection and improved reporting skills"]

### **GitHub Portfolio Checklist**

**Essential Elements:**
- ✅ Professional README with summary of skills and experience
- ✅ 10+ detailed writeups (HTB, TryHackMe, CTF challenges)
- ✅ Custom tools/scripts with documentation
- ✅ Methodology documents (recon, testing checklists)
- ✅ Sanitized penetration test reports (mock engagements)
- ✅ Blog posts or technical articles
- ✅ Clean commit history and organization
- ✅ License files and proper attributions

**README Template:**
```markdown
# [Your Name] - Cybersecurity Portfolio

## About Me
Junior penetration tester with hands-on experience in web application security, 
infrastructure testing, and responsible vulnerability disclosure. Completed 
intensive 100-day training program covering OWASP Top 10, privilege escalation, 
and bug bounty hunting.

## Skills
**Web Application Security:** SQL Injection, XSS, IDOR, SSRF, Authentication/Authorization flaws
**Infrastructure Testing:** Linux/Windows privilege escalation, Active Directory basics
**Tools:** Burp Suite, nmap, Metasploit, Python scripting, Bash automation
**Methodologies:** OWASP Testing Guide, Bug Bounty reconnaissance, Professional reporting

## Projects
### [Automated Recon Tool](link)
Python-based tool for subdomain enumeration and endpoint discovery...

### [Writeups](link)
15+ detailed technical writeups from HackTheBox, TryHackMe, and CTF challenges...

### [Vulnerability Reports](link)
Sanitized penetration testing reports from mock engagements...

## Certifications & Training
- [List any you've completed or are pursuing]

##Contact
- Email: [your.email@example.com]
- LinkedIn: [profile]
- Twitter: [@handle]
- Blog: [link]

## Bug Bounty Stats
- Programs Tested: 8
- Valid Reports Submitted: [X]
- Accepted Vulnerabilities: [X]
```

---

## Resume Blurb for Junior Pentester Role

### **1-Page Resume Section: Experience**

```
CYBERSECURITY PRACTITIONER | Self-Directed Learning Program
[Month Year] - Present

• Completed intensive 100-day penetration testing training program covering web 
  application security, infrastructure testing, and responsible vulnerability disclosure
  
• Performed security assessments on 30+ practice environments including HackTheBox, 
  TryHackMe, and purpose-built vulnerable applications (OWASP Juice Shop, DVWA, WebGoat)
  
• Identified and responsibly disclosed [X] security vulnerabilities through bug bounty 
  programs including [severity levels], demonstrating practical testing skills
  
• Developed custom Python automation tools for reconnaissance and vulnerability 
  detection, available on GitHub with 50+ stars
  
• Authored 15+ technical writeups documenting penetration testing methodologies, 
  tool usage, and exploitation techniques
  
• Proficient in vulnerability assessment tools: Burp Suite Professional workflows, 
  nmap NSE scripts, Metasploit framework, SQLMap, and various enumeration utilities
  
• Created professional penetration test reports following industry standards including 
  executive summaries, technical findings, CVSS scoring, and remediation recommendations
  
• Actively engaged with cybersecurity community through knowledge sharing, technical 
  blog posts, and participation in capture-the-flag competitions

Technical Competencies:
• Web Security: OWASP Top 10, API testing, authentication/authorization bypass, 
  business logic flaws, SSRF, XXE, deserialization
• Infrastructure: Linux/Windows privilege escalation, Active Directory enumeration, 
  network reconnaissance, service exploitation
• Programming: Python (scripting & automation), Bash, understanding of PHP/JavaScript 
  for code review
• Methodologies: OWASP Testing Guide, PTES, bug bounty reconnaissance frameworks
• Tools: Burp Suite, OWASP ZAP, nmap, Metasploit, Wireshark, subfinder, ffuf, 
  Bloodhound, Responder
```

### **Alternative: Skills-Based Format**

```
PENETRATION TESTING SKILLS

Web Application Security Testing
✓ Performed comprehensive security assessments on 20+ web applications
✓ Identified OWASP Top 10 vulnerabilities including SQL injection, XSS, IDOR, SSRF
✓ Proficient in Burp Suite Professional for proxy interception, scanning, and 
  exploitation
✓ API security testing including REST, GraphQL, JWT manipulation
✓ Completed 50+ PortSwigger Web Security Academy labs

Infrastructure & Network Security
✓ Conducted penetration tests on 15+ Linux/Windows systems
✓ Expertise in privilege escalation techniques (SUID, sudo, kernel exploits, 
  service misconfigurations)
✓ Network reconnaissance using nmap, masscan, service enumeration
✓ Basic Active Directory attack techniques (Kerberoasting, AS-REP roasting)
✓ Successfully compromised HackTheBox machines across difficulty levels

Responsible Vulnerability Disclosure
✓ Active bug bounty hunter with [X] valid vulnerability reports submitted
✓ Findings include [list severities/types if impressive]
✓ Professional report writing following industry disclosure standards
✓ Understanding of coordinated disclosure timelines and vendor communication

Automation & Tool Development
✓ Developed custom Python scripts for reconnaissance and exploitation
✓ Created Bash automation for enumeration workflows
✓ GitHub portfolio with documented tools and methodologies
✓ Code available at: github.com/[yourhandle]
```

---

## Safe & Legal Practice Targets

### **Always-Safe Practice Platforms**

**1. TryHackMe (tryhackme.com)**
- Beginner-friendly, guided learning paths
- Legal and safe, designed for practice
- Recommended rooms by week (listed in roadmap above)
- Subscription: ~$10/month

**2. HackTheBox (hackthebox.com)**
- Retired machines are free with VIP ($14/month)
- Active machines available (don't share solutions publicly)
- Starting Point for beginners
- Proof Labs (guided penetration testing)

**3. PortSwigger Web Security Academy (portswigger.net/web-security)**
- Completely FREE
- Best-in-class web security training
- Labs for every vulnerability type
- Certificate upon completion

**4. OWASP Purpose-Built Applications**
- **Juice Shop:** Modern web app (juice-shop.herokuapp.com or local Docker)
- **WebGoat:** Java-based lessons (run locally)
- **DVWA:** PHP/MySQL classic vulnerable app
- **Mutillidae:** OWASP Top 10 practice
- All designed for exploitation

**5. PentesterLab (pentesterlab.com)**
- Web for Pentester exercises
- From SQL Injection to Shell series
- Premium badge system
- Subscription: ~$20/month

**6. Vulnerable APIs**
- **crAPI:** Completely Ridiculous API (github.com/OWASP/crAPI)
- **vAPI:** Vulnerable Adversely Programmed Interface
- **Damn Vulnerable GraphQL Application**
- **DVWS:** Damn Vulnerable Web Services

**7. VulnHub (vulnhub.com)**
- Free vulnerable VM downloads
- Various difficulty levels
- Offline practice available
- Community writeups allowed

**8. CTF Platforms**
- **PicoCTF:** Beginner-friendly CTF
- **OverTheWire:** Wargames (Bandit for Linux basics)
- **CTFtime.org:** Find ongoing competitions
- **Root-Me:** Challenges across all categories

### **Bug Bounty Programs - Beginner Friendly**

**Vulnerability Disclosure Programs (VDPs) - No Rewards, Low Pressure:**
- Test without bounty pressure
- Focus on learning, not earnings
- Examples available on HackerOne/Bugcrowd filtered by VDP

**Programs Known for Beginner-Friendly Triage:**
- Research platforms using "New Programs" filter
- Look for:
  - Large attack surface (many subdomains/assets)
  - Public disclosure of past reports
  - Active and responsive security team
  - Clear scope and rules

**Research Before Testing:**
1. Read program policy completely (3+ times)
2. Check scope carefully (what's in, what's out)
3. Review disclosed reports to understand what they accept
4. Start with less-tested assets (documentation sites, mobile apps)
5. NEVER test production data, payment systems, or user accounts without explicit permission

**Red Flags - Avoid These Programs Initially:**
- Very high minimum severity requirements
- "Duplicate city" reputation
- Slow response times (check comments)
- Aggressive "out of scope" interpretations
- Limited scope with few assets

### **Responsible Disclosure Timeline**

```
Day 0: Vulnerability discovered
Day 0-1: Verify vulnerability, create PoC, write initial report
Day 1: Submit report to program
Day 1-7: Program triages (typical response time)
Day 7-30: Back-and-forth clarification if needed
Day 30-90: Vendor develops and deploys fix
Day 90+: Public disclosure (if approved by program)

⚠️ NEVER disclose publicly before vendor approval
⚠️ Follow the program's disclosure policy
⚠️ If no response after 90 days, follow coordinated disclosure best practices
```

---

## Advanced Tips for Success

### **Mindset Shifts for Junior Pentesters**

1. **Documentation is as important as discovery**
   - If you didn't document it, it didn't happen
   - Future you will thank past you for good notes
   - Your writeups are your portfolio

2. **Enumeration is 80% of the work**
   - When stuck, enumerate more
   - Slow down, be thorough
   - Automated tools miss things

3. **Understand the "why," not just the "how"**
   - Don't just run exploit code
   - Understand the vulnerability class
   - This knowledge transfers across targets

4. **Every "failure" is learning**
   - Duplicates teach you what's already known
   - N/A reports teach you scope interpretation
   - Informational findings teach you risk assessment

5. **Community over competition**
   - Help others when you can
   - Ask questions without shame
   - Share knowledge generously

### **Common Beginner Mistakes to Avoid**

❌ **Skipping basics to chase advanced topics**
→ Master fundamentals first; advanced topics build on them

❌ **Only practicing, never documenting**
→ Balance is 60% practice, 40% documentation

❌ **Tool dependency without understanding**
→ Learn manual exploitation before automation

❌ **Testing without reading scope carefully**
→ Always read program policy 3+ times

❌ **Giving up after first rejection**
→ Bug bounty is a numbers game; persistence wins

❌ **Comparing your progress to others**
→ Everyone's journey is different; focus on your growth

❌ **Neglecting soft skills (communication, reporting)**
→ Technical skills + communication = hire-able candidate

❌ **Burning out by never taking breaks**
→ Sustainable pace beats sprint-and-crash

### **Networking & Community Engagement**

**Twitter (X) Strategy:**
- Follow: @NahamSec, @STÖK, @jhaddix, @TomNomNom, @zseano, @InsiderPhD
- Tweet your progress, writeups, tools
- Engage authentically (comment, retweet, help others)
- Use hashtags: #bugbounty #cybersecurity #infosec #100daysofhacking

**Discord Servers to Join:**
- TryHackMe Official
- HackTheBox Official
- NahamSec Discord
- The Cyber Mentor Discord
- BugBountyWorld

**Reddit Communities:**
- r/netsec (news and research)
- r/HowToHack (learning resources)
- r/bugbounty (discussions and tips)
- r/AskNetsec (questions)

**Blogging Platforms:**
- Medium (largest audience)
- Dev.to (developer-focused)
- HashNode (technical content)
- Personal GitHub Pages (full control)

### **Building Your Brand (Optional but Helpful)**

- Choose consistent handle across platforms
- Create professional profile picture
- Write bio that clearly states "aspiring pentester" or "junior security researcher"
- Link all your platforms (Twitter → GitHub → Blog → LinkedIn)
- Share progress consistently (not just wins, but learning moments)
- Help others in community (answer questions, share resources)

---

## Post-100-Day Roadmap

### **Days 101-200: Consolidation & Specialization**

**Continue Bug Bounty Hunting (50% of time)**
- Test 2-3 programs consistently
- Focus on finding medium/high severity bugs
- Develop signature methodology
- Goal: 5+ additional accepted reports

**Pursue Certification (25% of time)**
- **eJPT** (eLearnSecurity Junior Penetration Tester) - Beginner-friendly
- **PNPT** (Practical Network Penetration Tester) - Affordable, practical
- **OSCP** (Offensive Security Certified Professional) - Industry gold standard

**Specialize in One Area (25% of time)**
Options:
- **Web Application Security** (API security, modern frameworks)
- **Mobile Application Security** (Android/iOS testing)
- **Cloud Security** (AWS/Azure/GCP pentesting)
- **Active Directory / Red Teaming**
- **Thick Client / Desktop Application Security**

### **6-Month Goals**
- 10+ accepted bug bounty reports
- First paid bounty (even if small)
- 1 certification earned
- 20+ quality writeups
- Contributing to open-source security tools
- Speaking at local meetup or conference (optional)

### **1-Year Goals**
- Junior pentester job secured OR consistent bug bounty income
- 2-3 certifications
- Specialized expertise in one security domain
- Mentoring others starting their journey
- Created at least one popular tool/resource

---

## Key Resources Library

### **Essential Bookmarks**

**Learning Platforms:**
- PortSwigger Web Security Academy: https://portswigger.net/web-security
- OWASP Testing Guide: https://owasp.org/www-project-web-security-testing-guide/
- HackTricks: https://book.hacktricks.xyz/
- PayloadsAllTheThings: https://github.com/swisskyrepo/PayloadsAllTheThings

**Bug Bounty:**
- HackerOne Public Disclosures: https://hackerone.com/hacktivity
- Bugcrowd Public Disclosures: https://bugcrowd.com/programs
- Chaos Project (scope): https://chaos.projectdiscovery.io/

**Tools & Automation:**
- SecLists (wordlists): https://github.com/danielmiessler/SecLists
- GTFOBins (privilege escalation): https://gtfobins.github.io/
- LOLBAS (Windows binaries): https://lolbas-project.github.io/

**YouTube Channels:**
- IppSec (HTB walkthroughs)
- John Hammond (CTF & pentesting)
- LiveOverflow (deep technical content)
- The Cyber Mentor (courses & pentesting)
- NahamSec (bug bounty)
- STÖK (bug bounty lifestyle)
- InsiderPhD (beginner bug bounty)

**Blogs to Follow:**
- PortSwigger Research Blog
- Bishop Fox's Cybersecurity Style Guide
- Detectify Labs
- Orange Tsai's Blog
- James Kettle (albinowax)

**Books (Optional - After Day 100):**
- "The Web Application Hacker's Handbook" - Stuttard & Pinto (classic)
- "Real-World Bug Hunting" - Peter Yaworski (bug bounty)
- "The Hacker Playbook 3" - Peter Kim (pentesting)
- "RTFM: Red Team Field Manual" - Ben Clark (reference)

---

## Emergency Contacts & Support

### **When You Need Help**

**Technical Questions:**
- TryHackMe Discord - Specific room help
- HackTheBox Forums - No spoilers for active machines
- r/AskNetsec - General security questions
- InfoSec Prep Discord - Community support

**Mental Health & Burnout:**
- Take breaks without guilt
- Remember: This is a marathon, not a sprint
- Imposter syndrome is normal and temporary
- Your worth ≠ your bug bounty acceptances

**Ethical Concerns:**
- When in doubt about legality: DON'T TEST
- Read program policies carefully
- NEVER test outside authorized scope
- If unsure, ask program before testing

**Career Advice:**
- r/cybersecurity Career Megathread
- LinkedIn cybersecurity groups
- Local BSides/OWASP chapters
- Security meetups (meetup.com)

---

## Final Checklist - Day 100 Review

### **Technical Achievements**
- [ ] Completed 25+ labs/boxes
- [ ] Submitted 3+ bug reports
- [ ] Proficient in Burp Suite/web testing
- [ ] Can perform basic privilege escalation
- [ ] Understanding of OWASP Top 10
- [ ] Created custom tools/scripts
- [ ] 50+ PortSwigger Academy labs

### **Portfolio Completeness**
- [ ] GitHub profile professional and organized
- [ ] 10+ detailed writeups published
- [ ] Resume tailored for junior pentester roles
- [ ] LinkedIn profile updated
- [ ] At least 1 blog post published
- [ ] Professional bio written
- [ ] Contact information accessible

### **Soft Skills**
- [ ] Can explain technical concepts clearly
- [ ] Write professional reports
- [ ] Comfortable with responsible disclosure process
- [ ] Engaged with cybersecurity community
- [ ] Developed consistent study habits
- [ ] Created sustainable learning routine

### **Career Readiness**
- [ ] Resume ready to send
- [ ] Portfolio link-ready
- [ ] Interview talking points prepared
- [ ] Applied to 3+ junior positions (or ready to)
- [ ] Clear 6-month plan created
- [ ] Identified specialization interest

### **Mindset & Habits**
- [ ] Comfortable with being stuck and problem-solving
- [ ] Documentation is automatic habit
- [ ] Can maintain focus for 2+ hours
- [ ] Weekly retrospectives in place
- [ ] Healthy relationship with breaks
- [ ] Excited about continuous learning

---

## Troubleshooting Common Concerns

### **"I'm behind schedule"**
✅ **Solution:** This is normal. Focus on understanding over speed.
- Adjust roadmap: extend weeks that need more time
- Quality > quantity: better to master one topic than rush three
- Some people need 120-150 days - that's perfectly fine

### **"I haven't found any bugs yet"**
✅ **Solution:** Bug bounty success takes time.
- Average is 3-6 months before first acceptance
- Focus on less-tested assets (APIs, mobile, docs sites)
- Lower expectations: info/low severity is still success
- Consider VDP programs for learning without pressure

### **"I'm not smart enough for this"**
✅ **Solution:** This is imposter syndrome, not reality.
- Everyone feels this way starting out
- Skills are built, not innate
- You've already learned complex topics (Linux, TCP/IP, programming)
- Review Day 1 vs. Day 100 - you've grown enormously

### **"I can't afford paid platforms"**
✅ **Solution:** Free resources are abundant.
- PortSwigger Academy (completely free, world-class)
- TryHackMe free rooms (substantial content)
- VulnHub (free VMs)
- OWASP apps (free)
- HTB free tier + retired machines
- YouTube walkthroughs (IppSec, John Hammond)

### **"Should I start applying for jobs?"**
✅ **Decision Matrix:**

**Apply NOW if:**
- Portfolio has 8+ quality writeups
- You're comfortable explaining OWASP Top 10
- Resume demonstrates hands-on practice
- You can discuss your learning journey confidently

**Wait a bit if:**
- Portfolio feels empty (<5 writeups)
- You struggle to explain basic concepts
- Haven't completed any full assessments
- Still very uncomfortable with testing methodology

**Remember:** Some companies hire for potential + enthusiasm over experience.

---

## Your Daily Mantra (Save This)

**Print this. Put it above your desk. Read it daily.**

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│  "I am building expertise one hour at a time.              │
│   Every enumeration teaches me. Every failure sharpens me. │
│   I am becoming the pentester I will be proud to be."      │
│                                                             │
│  Today's focus: [WRITE YOUR SINGLE GOAL HERE]             │
│                                                             │
│  Consistency beats intensity. Progress beats perfection.    │
│  I document, therefore I grow.                             │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## Closing Motivation

You are about to embark on a transformative journey. In 100 days, you won't just have new skills—you'll have a new way of seeing technology, understanding systems, and solving problems. 

The path will be challenging. You'll feel stuck. You'll feel stupid. You'll question whether you're cut out for this. **These feelings are not stop signs—they're mile markers on the road to mastery.**

Every expert pentester you admire started exactly where you are now: confused, overwhelmed, and uncertain. The only difference between them and you is **they kept showing up.** They documented their confusion. They practiced through frustration. They submitted reports despite fear of rejection.

This roadmap is your guide, not your prison. Adjust it as needed. Take breaks when necessary. Celebrate small wins. Help others when you can. Build in public. Share your journey.

**100 days from now, you won't be perfect. But you'll be formidable.**

Now close this document, open Day 1's tasks, and begin.

Your future self is counting on you to start today.

---

**🚀 Begin Day 1 now. Document everything. Trust the process. You've got this.**

---

*Remember: The best time to start was yesterday. The second best time is now. Stop reading. Start doing. Day 1 awaits.*
