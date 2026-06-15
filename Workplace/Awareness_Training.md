---
name: "Security Awareness Training"
domain: Workplace
tags: [security-awareness, phishing-simulation, training, human-risk, compliance]
pricing:
  bronze: 15
  silver: 22
  gold: 30
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Security Awareness Training reduces human-layer risk by delivering role-appropriate security education and realistic phishing simulations that measurably change employee behavior over time. For mid-market organizations where a single clicked link can trigger a ransomware incident, the service creates a security-conscious culture through short, frequent training modules and data-driven coaching interventions — not just the annual checkbox exercise required for compliance.

## What's Included
- Monthly security awareness training module delivery covering current threat topics (phishing, social engineering, password hygiene, data handling)
- Quarterly simulated phishing campaigns targeting all employees, with difficulty progression over time
- Targeted remediation training auto-assigned to employees who fail phishing simulations
- Role-based training tracks: elevated-risk roles (finance, HR, executives) receive additional targeted content
- Training completion and phishing click-rate reporting for compliance evidence and trend analysis
- New-hire onboarding security training enrollment within the first week of employment
- Annual training calendar planning aligned to the threat intelligence landscape and compliance requirements

## What's Not Included
- In-person security awareness workshops or live instructor-led training sessions
- Physical social engineering exercises (tailgating tests, vishing campaigns) — available as a separate engagement
- Regulatory compliance training for non-security topics (GDPR, HR compliance, anti-bribery)
- Custom e-learning content development beyond the standard catalog customization
- Dark web credential monitoring for employee accounts (covered under [[Threat_Intelligence]])

## Dependencies
- [[Mail_Security]] — phishing simulation campaigns are coordinated with mail security to ensure simulated emails are delivered unfiltered
- [[Identity_Access_Management]] — employee directory integration drives automatic enrollment and completion tracking
- [[Threat_Intelligence]] — current threat intelligence informs training content prioritization and phishing simulation scenarios
- [[IT_Risk_Management]] — human-risk metrics from training and simulations feed the IT risk register
