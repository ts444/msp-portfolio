---
name: "Attack Surface Management"
domain: Security
tags: [asm, exposure-management, external-attack-surface, asset-discovery, risk]
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
Attack Surface Management provides continuous discovery and risk assessment of the customer's external-facing digital footprint — domains, IP ranges, exposed services, cloud assets, and third-party exposures — from the perspective of an attacker. The service extends into Exposure Management, correlating external attack surface findings with internal vulnerability and configuration data to prioritize remediation based on actual exploitability rather than theoretical severity scores.

## What's Included
- Continuous external asset discovery covering domains, subdomains, IP addresses, and cloud-hosted resources
- Exposure Management: correlation of external findings with internal vulnerability scan data to identify high-impact remediation priorities
- Identification of shadow IT assets, misconfigured cloud storage, and unintended internet-facing services
- Certificate expiry monitoring and alerting for all discovered external TLS endpoints
- Leaked credential monitoring across paste sites and breach databases associated with the customer's domains
- Monthly attack surface trend report with new asset discovery, resolved exposures, and risk-score changes
- Remediation guidance and ticketing integration for discovered exposures

## What's Not Included
- Active penetration testing or exploitation of discovered vulnerabilities
- Dark web monitoring beyond credential and domain-related intelligence (covered under [[Threat_Intelligence]])
- Third-party supply chain risk assessment for vendor security posture
- Internal network asset discovery (covered under [[Vulnerability_Management]])
- Brand impersonation takedown services

## Dependencies
- [[Vulnerability_Management]] — external attack surface findings are correlated with internal scan data for Exposure Management prioritization
- [[DNS]] — DNS zone visibility is required to validate discovered subdomains and external records
- [[Secret_Management]] — certificate expiry findings from ASM trigger renewal workflows in secret management
- [[SIEM]] — high-severity exposure discoveries are ingested as risk events in the SIEM
