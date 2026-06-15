---
name: "Collaboration Services"
domain: Workplace
tags: [collaboration, teams, video-conferencing, chat, sharepoint]
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
Collaboration Services manages the platforms and policies that enable employees to communicate, share information, and work together effectively — whether in the office, remote, or across organizational boundaries. For mid-market organizations standardized on Microsoft 365 or Google Workspace, the service ensures that Teams, SharePoint, video conferencing, and shared storage are correctly configured, governed, and performing reliably, rather than growing into an ungoverned sprawl of abandoned channels and orphaned shared drives.

## What's Included
- Microsoft Teams or Google Meet tenant configuration, policy management, and user provisioning
- SharePoint Online or Google Drive sharing policy governance: external sharing controls, sensitivity labels, and DLP policy enforcement
- Video conferencing platform management: room account provisioning, meeting policy configuration, and quality troubleshooting
- Persistent chat platform governance: channel naming standards, retention policies, and guest access controls
- Collaboration platform performance monitoring and proactive alerting on service degradation
- User and admin support for collaboration tool issues within defined response SLAs
- Quarterly platform governance review: inactive teams/sites cleanup, external membership audit, and policy alignment check

## What's Not Included
- Unified Communications infrastructure (IP-PBX, SIP trunking, on-premises telephony)
- Collaboration platform licensing procurement and subscription management
- Custom application or bot development for Teams or Workspace
- Audio-visual hardware management for conference rooms
- End-user adoption training and change management (covered under [[Awareness_Training]])

## Dependencies
- [[Productivity]] — collaboration services are layered on top of the productivity suite managed under this service
- [[Identity_Access_Management]] — user provisioning and guest access controls rely on the identity directory and SSO
- [[Mail_Security]] — collaboration platforms are subject to the same data loss prevention policies as email
- [[Awareness_Training]] — end-user training on secure collaboration practices is delivered through the training service
