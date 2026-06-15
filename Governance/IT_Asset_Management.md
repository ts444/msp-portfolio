---
name: "IT Asset Management"
domain: Governance
tags: [asset-management, itam, cmdb, lifecycle, inventory]
pricing:
  bronze: 18
  silver: 26
  gold: 35
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
IT Asset Management provides full lifecycle visibility and governance for all hardware and software assets — from procurement and deployment through to secure decommissioning — ensuring mid-market organizations know what they own, where it is, who is responsible for it, and when it needs to be replaced or renewed. A maintained asset inventory is the foundation that makes every other IT service more effective, from vulnerability prioritization to license compliance and EOL risk management.

## What's Included
- Hardware asset inventory covering servers, network devices, workstations, and peripherals with automated discovery reconciliation
- Software asset inventory including installed applications, versions, and license entitlement tracking
- Full asset lifecycle management: procurement registration, deployment tracking, owner assignment, and secure disposal records
- License compliance reporting: consumed versus entitled seats for major software titles
- Contract and warranty tracking with renewal alerts (90-day and 30-day advance notice)
- Asset criticality classification used by vulnerability management and risk management services
- Annual asset audit with physical reconciliation and disposal certificate review

## What's Not Included
- Software procurement, purchasing, or vendor contract negotiation
- Software license optimization consulting or true-up negotiation with vendors
- Financial asset valuation or depreciation accounting (for ERP/finance teams)
- Mobile device management (MDM) enrollment and policy enforcement
- Cloud SaaS subscription management and optimization

## Dependencies
- [[Deployment]] — all newly deployed assets are registered in the asset inventory at provisioning time
- [[Configuration_Management]] — the CMDB and asset inventory are synchronized for configuration item tracking
- [[EOL_Services]] — end-of-support dates tracked in the asset inventory trigger EOL risk management workflows
- [[IT_Change_Management]] — asset changes (moves, adds, decommissions) are tracked through the change management process
