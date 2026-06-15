---
name: "Network Access Control (NAC)"
domain: Security
tags: [nac, 802.1x, posture, zero-trust, network-admission]
pricing:
  bronze: 20
  silver: 28
  gold: 38
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Network Access Control enforces identity- and posture-based admission decisions for every device connecting to the wired and wireless network, ensuring that only known, compliant endpoints gain access to production resources. For mid-market organizations hosting a mix of corporate laptops, BYOD devices, and IoT equipment, NAC is the enforcement point that prevents unmanaged or compromised devices from communicating freely on the internal network.

## What's Included
- 802.1X authentication enforcement for wired and wireless network access using certificates or credentials
- Device posture assessment at connection time (OS version, patch level, endpoint protection status)
- Dynamic VLAN assignment based on device identity, posture result, and user role
- Guest and BYOD network onboarding with captive portal and time-limited access policies
- IoT device profiling and segmentation into dedicated restricted VLANs
- Rogue device detection and automated quarantine for unrecognized endpoints
- NAC policy reporting: authenticated devices, posture failures, VLAN assignments, and access exceptions

## What's Not Included
- Remote access VPN admission control (covered under [[Remote_Access_Management]])
- Zero Trust Network Access (ZTNA) for application-layer access (covered under [[Remote_Access_Management]])
- Physical port security enforcement on unmanaged switches outside the service scope
- MDM enrollment for mobile devices as a standalone service
- IoT device firmware management or vulnerability assessment

## Dependencies
- [[Identity_Access_Management]] — user and device identities from the directory are used for 802.1X authentication decisions
- [[Wireless]] — NAC enforces posture and VLAN assignment for wireless-connected devices
- [[Interconnection]] — dynamic VLAN assignment is implemented through the switching layer managed by this service
- [[Endpoint_Detection_and_Response]] — EDR agent presence and health status is a posture check input for NAC decisions
