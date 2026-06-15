---
name: "Incident Response & DFIR Retainer"
domain: Security
tags: [incident-response, dfir, forensics, retainer, containment]
pricing:
  bronze: 1500
  silver: 3000
  gold: 6000
unit: per-month/retainer
sla:
  bronze: { availability: "24/7", response: "4h", resolution_p1: "24h", resolution_p2: "72h" }
  silver: { availability: "24/7", response: "2h", resolution_p1: "12h", resolution_p2: "48h" }
  gold:   { availability: "24/7", response: "30m", resolution_p1: "4h", resolution_p2: "24h" }
---

## Overview
The Incident Response & DFIR Retainer provides mid-market organizations with 24/7 on-call access to a trained incident response team capable of full digital forensics and incident response (DFIR) engagements. The service covers the full IR lifecycle — from initial triage and containment through forensic evidence preservation, root-cause analysis, and post-incident reporting — without requiring customers to maintain in-house DFIR expertise. Ransomware, supply-chain compromise, and insider-threat scenarios are covered by pre-developed playbooks.

## What's Included
- 24/7 on-call IR retainer with guaranteed response SLA (see tiers above)
- Initial triage and containment: network isolation, credential revocation, attacker eviction
- Forensic evidence preservation: disk images, memory captures, log snapshots for regulatory and legal hold
- Malware analysis and IOC identification with actionable indicator feeds
- Ransomware-specific response playbooks: negotiation guidance, decryption validation, recovery sequencing
- Law enforcement coordination and documentation support (NCSC, BSI, national CERTs)
- Post-incident report: executive summary, technical timeline, root-cause finding, remediation recommendations
- Annual IR simulation / tabletop exercise (Gold tier: also quarterly)

## What's Not Included
- Ongoing managed detection (requires [[SIEM]] or [[Endpoint_Detection_and_Response]])
- Legal or insurance claim representation
- Public relations / crisis communications management
- Remediation project delivery beyond written recommendations (available as a separate engagement)
- Hardware acquisition or replacement costs during recovery

## Dependencies
- [[SIEM]] — SIEM telemetry significantly accelerates triage; IR team requires read access to SIEM during an active incident
- [[Endpoint_Detection_and_Response]] — EDR telemetry and isolation capability are used for containment actions
- [[Backup_and_DR]] — Recovery timeline depends on backup integrity and DR readiness
