# Brute Force Attack Investigation

## Overview
This project analyzes a cybersecurity incident involving a brute force attack against the website yummyrecipesforme.com.

The investigation focuses on malicious website modification, malware delivery, browser redirection behavior, and network protocol analysis using tcpdump.

## Objective
- Identify network protocols involved in the attack
- Document the security incident
- Analyze the impact of the compromise
- Recommend remediation measures to prevent future attacks

## Attack Summary
A former employee successfully performed a brute force attack against the website administrator account by guessing the default password. After gaining access, malicious JavaScript code was added to the website to trick users into downloading malware.

Visitors who downloaded the file were redirected to a fake website containing malware.

## Protocols Identified
- DNS
- HTTP
- TCP/IP

## Key Findings
- Default administrator password was compromised
- Website source code was modified
- Malware download prompts were embedded into the website
- Visitors were redirected to a malicious website
- DNS and HTTP traffic confirmed malicious redirection activity

## Project Structure
- security-incident-report.md
- protocol-analysis.md
- findings.md
- recommendations.md

## Outcome
The investigation confirmed that the website was compromised through a brute force attack and malicious JavaScript injection, resulting in malware distribution and browser redirection.

## References

- [Security Incident Report Template](docs/security-incident-report-template.pdf)

- [Tcpdump Traffic Log](docs/tcpdump-log.pdf)

- [Supporting Materials](docs/supporting-materials.pdf)
