---
name: "Threat Intelligence"
domain: Security
tags: [threat-intelligence, cti, ioc, darkweb, threat-feeds]
pricing:
  bronze: 22
  silver: 30
  gold: 40
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Threat Intelligence operationalizes curated, context-rich intelligence about adversaries, campaigns, and indicators of compromise (IOCs) that are relevant to the customer's industry and technology stack. Rather than drowning the security team in raw feed data, the service delivers finished intelligence — analyst-validated IOCs fed into detection tools, sector-specific threat briefings, and early warning of emerging threats — so that defenses are continuously updated to reflect the current threat landscape rather than yesterday's attacks.

## What's Included
- Curated IOC feed management: ingestion, validation, deduplication, and distribution to SIEM, DNS filtering, and endpoint protection platforms
- Sector-specific threat briefings (monthly) covering active threat actors, campaigns, and TTPs relevant to the customer's industry
- Dark web monitoring for the customer's brand name, domains, and leaked employee credentials
- Emerging threat early warning notifications when high-impact vulnerabilities or campaigns are actively exploited
- Threat actor profiling aligned to the customer's technology stack and geographic exposure
- Intelligence-driven detection rule updates coordinated with the SIEM service
- Quarterly threat landscape review aligned to the customer's risk register

## What's Not Included
- Active threat hunting engagements within the customer's environment (covered under [[SIEM]])
- Incident response or forensic investigation services
- Threat intelligence platform (TIP) development or self-hosted infrastructure management
- Legal or law enforcement engagement for attribution purposes
- Physical threat or executive protection intelligence

## Dependencies
- [[SIEM]] — validated IOCs and detection rules are distributed to the SIEM for active correlation
- [[Attack_Surface_Management]] — external exposure findings are enriched with threat actor targeting intelligence
- [[DNS]] — malicious domain IOCs are applied as blocks in the protective DNS filtering service
- [[Endpoint_Detection_and_Response]] — threat actor TTPs inform EDR detection logic updates
