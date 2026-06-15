---
name: "Macrosegmentation"
domain: Security
tags: [macrosegmentation, firewall, dmz, network-zones, perimeter]
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
Macrosegmentation defines and enforces the high-level security zone boundaries between the internet, DMZ, internal networks, and restricted environments using next-generation firewall policies and network ACLs. For mid-market organizations, well-governed macrosegmentation forms the foundation of a defense-in-depth architecture, ensuring that a breach in one zone cannot propagate unchecked into business-critical systems.

## What's Included
- Security zone architecture design: internet-facing, DMZ, internal, restricted, and management zones
- Next-generation firewall (NGFW) policy management for inter-zone traffic control
- Application-layer inspection policy configuration (application identification, SSL inspection)
- Ingress and egress filtering policies with explicit deny-all defaults and documented permit rules
- Firewall rule lifecycle management: quarterly rule review, unused rule cleanup, and shadow rule detection
- NAT and PAT policy management for internet-facing services
- Change-controlled firewall rule modifications with pre-change impact assessment

## What's Not Included
- Workload-to-workload east-west traffic control within a security zone (covered under [[Microsegmentation]])
- Web application firewall (WAF) policy management for published web applications
- IDS/IPS signature management as a standalone service (included in NGFW where platform supports)
- Physical firewall hardware procurement or data-center installation
- Cloud-native security group management for IaaS workloads (covered under [[Microsegmentation]])

## Dependencies
- [[Microsegmentation]] — macrosegmentation defines the outer boundaries within which microsegmentation operates
- [[Interconnection]] — inter-zone routing is handled by the network routing layer managed under Interconnection
- [[Network_Access_Control]] — NAC admission decisions determine which zone a connecting device is placed into
- [[Monitoring]] — firewall policy violations and anomalous traffic alerts feed the central monitoring platform
