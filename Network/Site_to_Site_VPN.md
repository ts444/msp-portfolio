---
name: "Site-to-Site VPN"
domain: Network
tags: [vpn, connectivity, encryption, tunneling, branch-office]
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
Site-to-Site VPN establishes encrypted, policy-controlled tunnels between headquarters, branch offices, and cloud environments, giving mid-market organizations a cost-effective alternative to private MPLS circuits without sacrificing security or reliability. The service covers the full tunnel lifecycle — design, deployment, monitoring, and failover — so internal teams can focus on business outcomes rather than connectivity troubleshooting.

## What's Included
- Design and deployment of IPsec/IKEv2 or SSL-based site-to-site tunnels
- Redundant tunnel configuration with automatic failover between primary and secondary paths
- Encryption policy management (cipher suites, key rotation, PFS enforcement)
- Continuous tunnel health monitoring with proactive alerting on degradation or drops
- Firewall rule management scoped to VPN traffic flows
- Quarterly tunnel configuration review and certificate renewal management
- Documentation of all tunnel endpoints, routing, and policy settings

## What's Not Included
- Client-based remote-access VPN for individual users (covered under [[Remote_Access_Management]])
- Physical WAN circuit provisioning or ISP contract management (covered under [[WAN]])
- SD-WAN overlay configuration and application-aware routing (covered under [[Interconnection]])
- Third-party vendor network integration beyond standard IPsec interoperability
- VPN concentrator hardware procurement or data-center colocation

## Dependencies
- [[WAN]] — underlying internet circuits must be operational for tunnel establishment
- [[Interconnection]] — routing policies and SD-WAN overlays interact with VPN tunnel paths
- [[Monitoring]] — tunnel availability metrics feed into the infrastructure monitoring platform
- [[Network_Access_Control]] — VPN-admitted traffic is subject to NAC policy enforcement
