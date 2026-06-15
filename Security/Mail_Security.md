---
name: "Mail Security"
domain: Security
tags: [email, phishing, antispam, sandboxing, dmarc]
pricing:
  bronze: 20
  silver: 28
  gold: 38
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Mail Security provides multi-layered protection for inbound and outbound email, combining anti-phishing, anti-spam, malware detection, and attachment sandboxing to stop the attack vector responsible for over 90% of ransomware incidents. For mid-market organizations, the service goes beyond basic spam filtering by implementing full email authentication (SPF, DKIM, DMARC) and detonating suspicious attachments in an isolated environment before they reach user inboxes.

## What's Included
- Inbound email filtering: anti-spam, anti-phishing, and anti-malware with machine-learning-based detection
- Attachment sandboxing: detonation of suspicious files in an isolated environment before delivery
- URL rewriting and time-of-click protection against delayed-activation malicious links
- Outbound email scanning for data loss prevention (DLP) and malware propagation prevention
- SPF, DKIM, and DMARC policy management with monitoring and reporting on authentication failures
- Impersonation and business email compromise (BEC) detection using display-name and domain-lookalike analysis
- Quarantine management portal with end-user and admin release workflows

## What's Not Included
- Email archiving and e-discovery services
- Secure email encryption for end-to-end encrypted message delivery to external recipients
- Microsoft 365 or Google Workspace tenant administration (covered under [[Productivity]])
- End-user phishing simulation and training campaigns (covered under [[Awareness_Training]])
- S/MIME certificate management for individual users

## Dependencies
- [[DNS]] — SPF, DKIM, and DMARC records are managed as part of DNS zone administration
- [[Awareness_Training]] — mail security findings (phishing rates, user clicks) inform training content targeting
- [[SIEM]] — mail security events are forwarded to SIEM for correlation with other threat indicators
- [[Productivity]] — mail security integrates with the productivity suite's mail platform APIs
