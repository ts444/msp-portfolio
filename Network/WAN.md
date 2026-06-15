---
name: "WAN Management"
domain: Network
tags: [wan, isp, broadband, failover, connectivity]
pricing:
  bronze: 15
  silver: 22
  gold: 32
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
WAN Management covers end-to-end oversight of all internet and wide-area network connections, including primary ISP links, backup internet circuits, and the failover logic between them. For mid-market organizations operating across multiple sites, the service eliminates single points of failure and ensures ISP-side issues are detected, escalated, and — where possible — automatically mitigated before users notice an outage.

## What's Included
- Management and monitoring of primary ISP connections at all covered sites
- Configuration and automated failover for backup internet connections (LTE/5G, secondary broadband)
- ISP incident coordination: opening, tracking, and escalating provider tickets on the customer's behalf
- Circuit performance baselining and monthly SLA compliance reporting against ISP commitments
- Edge router and CPE configuration management for WAN-facing interfaces
- Bandwidth utilization trend analysis with capacity planning recommendations
- Change-controlled updates to WAN routing and failover policies

## What's Not Included
- ISP contract negotiation, procurement, or billing management
- Physical installation of new WAN circuits or CPE hardware
- Internal LAN switching and routing (covered under [[Interconnection]])
- SD-WAN policy optimization and application-aware routing (covered under [[Interconnection]])
- Satellite or maritime connectivity solutions

## Dependencies
- [[Interconnection]] — WAN circuits terminate into the switching and routing layer managed under this service
- [[Site_to_Site_VPN]] — VPN tunnels depend on healthy WAN circuits for tunnel establishment and stability
- [[Network_Performance]] — WAN link quality metrics are consumed by performance management workflows
- [[Monitoring]] — circuit up/down and latency alerts integrate with the central monitoring platform
