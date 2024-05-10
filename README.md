**Ethical Hacking Technical Report**
**Client:** https://www.soundstripe.com/

**Date:** May 10, 2024

**Prepared by:** Rabino, John Renel, Evallar, John Carlo C.

**Executive Summary:**
Soundstripe's technical findings from the ethical hacking assessment are presented in this report. The evaluation's goal was to find weaknesses in the company's systems, apps, and network infrastructure. Critical and high-risk flaws were found using a variety of testing approaches, such as vulnerability scanning and penetration testing. Together with practical suggestions for correction, this study offers thorough explanations of these findings. 

**Vulnerability Summary:**
1. Network Infrastructure: 
**Critical:** Remote Code Execution vulnerability (CVE-XXXX-XXXX) in the Apache Struts framework (version X.X.X) running on server-01.soundstripe.com, allowing an attacker to execute arbitrary code remotely.
**High:**Misconfigured firewall rules permitting unrestricted access from external IP ranges to sensitive internal services (e.g., SSH, RDP) on server-02.soundstripe.com.

2. Web Applications:
**Critical:** SQL Injection vulnerability in the login form of Soundstripe WebApp, potentially enabling an attacker to extract sensitive data from the database.
**High:** Cross-Site Scripting (XSS) vulnerability in Soundstripe WebApp, allowing attackers to execute malicious scripts in users' browsers.

3. Operating System:
**Critical:** Outdated and unpatched operating systems (Windows Server 2008 R2) on critical servers server-03.soundstripe.com, exposing them to known exploits and malware.
**High:** Weak password policies on domain user accounts, facilitating brute-force attacks and unauthorized access.

4. Wireless Networks:
**Critical:** Weak encryption (WEP) used in wireless networks, allowing attackers to intercept and decrypt wireless traffic, exposing sensitive data.

5. Social Engineering:
**High:** Several employees fell victim to phishing emails, providing credentials and sensitive information in response.

**Recommendations**
1. Network Infrastructure:
-   To address the Remote Code Execution vulnerability, Apache Struts should be patched to the most recent version right away. 
- In order to restrict access using the least privilege concept, review and change your firewall rules.

2. Web Applications:
- -   Conduct a thorough code review and implement input validation to prevent SQL Injection and XSS attacks.
- -   Implement security headers (e.g., Content Security Policy) to mitigate XSS vulnerabilities.

3. Operating Systems:
- -   Develop a patch management process to regularly update and secure operating systems against known vulnerabilities. 
- -   Enforce strong password policies and consider implementing multi-factor authentication for domain user accounts.

4. Wireless Networks:
-   Upgrade wireless network encryption to WPA2 or WPA3 to ensure confidentiality and integrity of wireless communications.

5. Social Engineering:
-   Conduct regular security awareness training for employees to educate them about the risks of phishing attacks and how to identify and report suspicious emails.

**Conclusion:**
The infrastructure and apps of Soundstripe have various critical vulnerabilities and security issues that are brought to light by the ethical hacking assessment's conclusions. Soundstripe may greatly improve its security posture and lower the risk of cyberattacks and data breaches by putting the suggested repair measures into practice.

Signature:
 Rabino, John Renel
 Evallar, John Carlo C.
