---
name: "Wireless Network Management"
domain: Network
tags: [wifi, wireless, wlan, access-point, ssid]
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
Wireless Network Management delivers reliable, secure, and high-density Wi-Fi coverage across office sites by taking ownership of access point configuration, SSID policy, RF optimization, and ongoing performance oversight. Mid-market organizations with open-plan offices and high device counts benefit from proactive channel management and capacity planning, preventing the slow degradation in wireless performance that often goes undetected until users complain.

## What's Included
- SSID design and segmentation (corporate, guest, IoT) with VLAN tagging and appropriate security profiles
- Access point firmware management and scheduled updates with tested rollback capability
- RF channel planning and automatic channel and power optimization
- Wireless controller or cloud management platform administration
- Rogue access point detection and alerting
- Wireless coverage and signal strength reporting with remediation recommendations
- Guest captive portal configuration and acceptable-use policy enforcement

## What's Not Included
- Physical access point installation, cabling, or mounting (requires a separate professional services engagement)
- Dedicated wireless intrusion prevention system (WIPS) as a security control (covered under [[Network_Access_Control]])
- Cellular or private LTE/5G network design and management
- Outdoor or campus-wide mesh deployments beyond standard office environments
- End-user device Wi-Fi adapter driver troubleshooting

## Dependencies
- [[Interconnection]] — wireless VLANs are trunked into the switching layer and routed through the core network
- [[Network_Access_Control]] — device authentication and posture checks apply to wireless-connected endpoints
- [[DNS]] — wireless clients depend on DNS resolution managed under the DNS service
- [[Monitoring]] — access point availability and client association metrics feed the central monitoring platform
