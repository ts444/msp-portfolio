---
name: "Remote Access Management"
domain: Infrastructure
tags: [remote-access, vpn, zero-trust, mfa, ztna]
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
Remote Access Management delivers secure, scalable connectivity for employees, contractors, and third-party vendors who need access to internal systems from outside the corporate network. The service supports both traditional SSL/IPsec client VPN and modern Zero Trust Network Access (ZTNA) approaches, enforcing MFA, device posture checks, and least-privilege access policies that keep remote work productive without expanding the attack surface.

## What's Included
- Client VPN gateway management (SSL/IPsec) with split-tunneling and full-tunnel policy options
- Zero Trust Network Access (ZTNA) policy configuration and user-to-application access segmentation
- Multi-factor authentication enforcement for all remote access sessions
- Device posture validation before granting access (OS patch level, endpoint protection status)
- User access provisioning, modification, and deprovisioning tied to HR lifecycle events
- Third-party and vendor access management with time-limited, audited session controls
- Remote access usage reporting and anomalous login alerting

## What's Not Included
- Site-to-site VPN tunnels between fixed locations (covered under [[Site_to_Site_VPN]])
- Identity provider administration and directory management (covered under [[Identity_Access_Management]])
- End-user VPN client installation and personal device support
- Remote desktop infrastructure provisioning (VDI, DaaS platforms)
- Physical access control systems or badge management

## Dependencies
- [[Identity_Access_Management]] — user identities and group memberships govern remote access entitlements
- [[Site_to_Site_VPN]] — remote access gateways and site VPN tunnels share edge infrastructure
- [[Network_Access_Control]] — device posture results from NAC inform remote access admission decisions
- [[Monitoring]] — gateway availability and failed authentication events are monitored centrally
