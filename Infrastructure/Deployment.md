---
name: "Infrastructure Deployment"
domain: Infrastructure
tags: [deployment, provisioning, automation, onboarding, lifecycle]
pricing:
  bronze: 18
  silver: 26
  gold: 36
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Infrastructure Deployment manages the end-to-end provisioning of servers, virtual machines, and cloud infrastructure — from image preparation and network integration to handoff into production monitoring. For mid-market organizations that provision new capacity in response to growth or M&A activity, a repeatable, automated deployment pipeline dramatically reduces the time from order to operational and eliminates the configuration inconsistencies that stem from manual builds.

## What's Included
- Standardized server and VM provisioning using approved golden images and infrastructure-as-code templates
- Network integration: VLAN assignment, IP allocation, DNS registration, and firewall rule creation
- Operating system installation, initial hardening, and agent deployment (monitoring, endpoint protection)
- Cloud IaaS resource provisioning for approved cloud platforms (compute, storage, networking)
- Deployment pipeline documentation and runbook maintenance
- Post-deployment validation testing and handoff checklist sign-off
- Decommissioning procedures including secure data erasure and asset retirement records

## What's Not Included
- Physical hardware procurement, rack installation, or data-center colocation management
- Application installation and configuration beyond OS-level agents
- Custom infrastructure-as-code module development for bespoke architectures
- Database provisioning or administration
- End-user device (workstation/laptop) deployment (covered under [[Configuration_Management]])

## Dependencies
- [[Configuration_Management]] — deployed systems are immediately enrolled into configuration management baselines
- [[Monitoring]] — monitoring agents are installed and configured as part of every deployment
- [[Patch_Management]] — newly deployed systems enter the patch management cycle immediately post-handoff
- [[IT_Asset_Management]] — all deployed assets are registered in the asset management system
