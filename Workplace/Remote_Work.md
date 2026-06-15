---
name: "Remote Work Enablement"
domain: Workplace
tags: [remote-work, hybrid, endpoint, ux, digital-workspace]
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
Remote Work Enablement ensures that employees working outside the office have a consistent, secure, and high-performance digital experience equivalent to working on-site. For mid-market organizations that have committed to hybrid or fully remote models, the service addresses the full stack of remote work dependencies — device management, secure connectivity, application access, and performance optimization — rather than treating remote access as an afterthought bolted onto an office-first infrastructure.

## What's Included
- Mobile Device Management (MDM) policy configuration and enforcement for corporate laptops and managed mobile devices
- Corporate device configuration profiles: application deployment, OS settings, and compliance policies via MDM
- Remote connectivity quality monitoring: VPN performance, cloud application latency, and ISP-side issue identification
- Home network troubleshooting guidance and ISP escalation support for employees with connectivity impacting productivity
- Remote desktop and virtual application access configuration for applications that cannot be delivered natively
- Remote endpoint support: remote diagnostics, software installation, and OS troubleshooting
- Remote worker onboarding kit: standardized device configuration, access provisioning, and connectivity validation checklist

## What's Not Included
- Hardware procurement, shipping, or physical setup of home office equipment
- BYOD (personally owned device) management and support
- Home network infrastructure management (routers, ISP contracts)
- VPN gateway and remote access infrastructure management (covered under [[Remote_Access_Management]])
- Virtual desktop infrastructure (VDI) platform provisioning and hypervisor management (covered under [[Virtualization]])

## Dependencies
- [[Remote_Access_Management]] — remote work connectivity depends on the VPN and ZTNA infrastructure managed by this service
- [[Identity_Access_Management]] — device compliance state and user identity govern conditional access to applications
- [[Endpoint_Detection_and_Response]] — EDR agent is required on all managed remote devices as part of the remote work standard
- [[Productivity]] — the productivity suite is the primary application layer consumed by remote workers
