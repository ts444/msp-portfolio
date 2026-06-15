---
name: "IT Change Management"
domain: Governance
tags: [change-management, itsm, cab, risk-assessment, change-control]
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
IT Change Management provides the structured process and tooling that ensures all changes to the managed IT environment are assessed for risk, approved by the appropriate authority, scheduled to minimize business impact, and reviewed after implementation. For mid-market organizations, a well-run change process is the single most effective control for reducing self-inflicted outages — the majority of production incidents have a recent unauthorized or untested change as root cause.

## What's Included
- Change request intake, categorization (standard, normal, emergency), and risk assessment workflow
- Change Advisory Board (CAB) coordination: agenda management, risk review, and approval records
- Change scheduling with maintenance window governance and stakeholder communication
- Pre-change and post-change implementation plans and rollback procedure documentation requirements
- Emergency change fast-track process with retroactive risk documentation
- Change success rate reporting and post-implementation review (PIR) tracking
- Integration with monitoring platform to suppress alerts during approved maintenance windows

## What's Not Included
- ITSM platform procurement, licensing, or initial implementation
- Release management and software deployment pipeline governance
- Configuration item (CI) relationship mapping in the CMDB (covered under [[Configuration_Management]])
- Business process change management or organizational change management consulting
- Project portfolio governance (covered under [[IT_Project_Management]])

## Dependencies
- [[Configuration_Management]] — changes to configuration items are linked to approved change records
- [[Monitoring]] — approved maintenance windows suppress monitoring alerts through ITSM integration
- [[IT_Risk_Management]] — high-risk changes reference the risk register and may require risk owner sign-off
- [[IT_Asset_Management]] — affected assets are identified from the asset inventory when raising change requests
