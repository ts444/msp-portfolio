---
name: "Business Continuity"
domain: Security
tags: [business-continuity, bcp, containment, remediation, resilience]
pricing:
  bronze: 25
  silver: 33
  gold: 40
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Business Continuity provides the planning, testing, and active response capabilities that keep a mid-market organization operational during and after a significant IT disruption — whether caused by a ransomware attack, infrastructure failure, or natural disaster. The service encompasses both proactive BCP maintenance and reactive containment and remediation support, ensuring that when an incident occurs the response is organized, documented, and practiced rather than improvised under pressure.

## What's Included
- Business Continuity Plan (BCP) development and annual review aligned to the organization's critical process inventory
- Business Impact Analysis (BIA) to identify recovery time objectives (RTO) and recovery point objectives (RPO) per system
- Tabletop exercise facilitation (minimum annual) to validate plan effectiveness with key stakeholders
- Incident containment support: network isolation, credential reset coordination, and threat actor eviction procedures
- Post-incident remediation coordination: clean system restoration, data integrity validation, and lessons-learned documentation
- Communication plan templates for internal and external stakeholder notification during incidents
- Integration with Backup & DR recovery procedures for IT system restoration sequencing

## What's Not Included
- Physical site recovery, alternative workspace provisioning, or facilities management
- Cyber insurance claims management or legal counsel coordination
- Full-scope digital forensics and incident response (DFIR) retainer services
- 24/7 staffed incident response retainer (available as a separate engagement)
- Business process re-engineering or non-IT operational continuity planning

## Dependencies
- [[Backup_and_DR]] — BCP recovery procedures depend on tested backup and disaster recovery capabilities
- [[SIEM]] — incident detection and timeline reconstruction rely on SIEM data during active incidents
- [[Identity_Access_Management]] — credential reset and account remediation are coordinated through IAM
- [[IT_Change_Management]] — remediation activities are tracked as emergency changes for audit purposes
