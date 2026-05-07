# Security Incident Report

## Section 1: Identify the Network Protocol Involved

The network protocols identified during the investigation were DNS and HTTP.

DNS was used when the browser requested the IP addresses for yummyrecipesforme.com and greatrecipesforme.com from the DNS server.

HTTP was used when the browser requested webpages and downloaded the malicious file from the compromised website.

---

## Section 2: Document the Incident

A former employee executed a brute force attack against the administrator account for yummyrecipesforme.com by repeatedly attempting known default passwords until the correct password was identified.

After gaining administrative access, the attacker modified the website source code by embedding malicious JavaScript. The script prompted website visitors to download and run an executable file disguised as a browser update.

When users executed the file, their browsers were redirected from yummyrecipesforme.com to greatrecipesforme.com, which contained malware.

Customers reported suspicious behavior after visiting the website, including unexpected file downloads, browser redirects, and reduced computer performance.

Cybersecurity analysts created a sandbox environment and used tcpdump to analyze network traffic. The investigation confirmed DNS requests, HTTP requests, malware downloads, and malicious browser redirection activity.

The investigation determined that the website had been successfully compromised due to weak password security and the absence of brute force protections.

---

## Section 3: Recommend One Remediation

One effective security measure is enforcing multi-factor authentication (MFA) for administrative accounts.

MFA adds an additional layer of security beyond passwords by requiring users to verify their identity using another authentication method, such as a mobile authentication code or security token.

Even if an attacker successfully guesses a password during a brute force attack, MFA can help prevent unauthorized access to the account.
