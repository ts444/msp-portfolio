---
name: "IT Knowledge Management"
domain: Governance
tags: [knowledge-management, documentation, runbooks, kb, itsm]
pricing:
  bronze: 15
  silver: 20
  gold: 28
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
IT Knowledge Management builds and maintains the structured documentation library that enables consistent, efficient IT operations — from technician runbooks and troubleshooting guides to user-facing how-to articles and vendor configuration references. For mid-market organizations where institutional knowledge often resides with one or two key individuals, a governed knowledge base reduces dependency on specific staff, accelerates incident resolution, and shortens onboarding time for new team members.

## What's Included
- Knowledge base platform administration and taxonomy management
- Runbook authoring and maintenance for all recurring operational procedures within the managed service scope
- Known error database (KEDB) maintenance linking recurring incidents to documented workarounds and fixes
- User-facing self-service knowledge articles for common IT requests and issues
- Knowledge article quality review cycle: accuracy, completeness, and last-reviewed-date governance
- Knowledge gap identification from incident and problem records, with article creation assignments
- Knowledge base access reporting and search analytics to identify gaps in self-service coverage

## What's Not Included
- Business process documentation outside the IT domain
- Training content development or e-learning course authoring (covered under [[Awareness_Training]])
- Policy and procedure documentation for regulatory compliance frameworks (covered under [[IT_Risk_Management]])
- Software development documentation (API references, architecture decision records)
- Video-based tutorial production

## Dependencies
- [[IT_Change_Management]] — change records trigger knowledge article updates when procedures are modified
- [[IT_Project_Management]] — project deliverables include knowledge transfer documentation as a standard exit criterion
- [[Monitoring]] — resolved incidents and their root causes are sourced to enrich the KEDB
- [[Deployment]] — deployment runbooks are maintained as part of the knowledge management library
