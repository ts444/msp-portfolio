---
name: "End-of-Life Services Management"
domain: Security
tags: [eol, legacy, risk-management, lifecycle, compensating-controls]
pricing:
  bronze: 18
  silver: 26
  gold: 34
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
End-of-Life Services Management identifies, tracks, and mitigates the security and operational risks introduced by software and hardware that has reached end-of-support from its vendor. For mid-market organizations with organic IT growth, EOL systems accumulate quietly and become the highest-risk assets in the environment; this service provides structured discovery, risk documentation, compensating controls, and lifecycle roadmaps to systematically eliminate EOL exposure.

## What's Included
- Discovery and cataloging of all EOL operating systems, applications, and hardware within the managed environment
- Risk scoring of EOL assets based on exposure, criticality, and available exploit activity
- Compensating control design and implementation for EOL systems that cannot be immediately retired (network isolation, enhanced monitoring, application allowlisting)
- EOL roadmap development with upgrade or replacement timelines aligned to business constraints
- Vendor end-of-support date tracking with advance notice alerts (12-month and 6-month warnings)
- EOL exception documentation for cyber insurance and compliance audit purposes
- Quarterly EOL posture review with progress tracking against the remediation roadmap

## What's Not Included
- Hardware procurement or software licensing for replacement systems
- Migration project management for EOL system replacements (covered under [[IT_Project_Management]])
- Custom support contracts negotiated directly with vendors for extended EOL coverage
- OT/SCADA or industrial control system lifecycle management
- Application re-platforming or code modernization for custom-developed EOL software

## Dependencies
- [[IT_Asset_Management]] — EOL tracking is maintained as lifecycle attributes within the asset management inventory
- [[Vulnerability_Management]] — EOL systems are flagged as elevated risk in vulnerability prioritization workflows
- [[Device_Hardening]] — compensating controls for EOL systems follow the hardening service's policy framework
- [[Microsegmentation]] — network isolation of EOL systems is implemented through the microsegmentation service
