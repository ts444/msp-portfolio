---
name: "Microsegmentation"
domain: Security
tags: [microsegmentation, zero-trust, east-west, firewall, workload-isolation]
pricing:
  bronze: 22
  silver: 30
  gold: 40
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Microsegmentation applies fine-grained, identity- and workload-aware access controls to east-west traffic within the data center and cloud environments, preventing an attacker who has compromised one workload from moving laterally to high-value targets. For mid-market organizations migrating to hybrid cloud or holding sensitive data under regulatory compliance requirements, microsegmentation provides the blast-radius containment that traditional perimeter firewalls cannot deliver inside a flat network.

## What's Included
- Workload communication mapping to establish a baseline of legitimate east-west traffic flows
- Policy design and enforcement using host-based firewalls, hypervisor-level controls, or dedicated microsegmentation platforms
- Application-tier isolation: separate policies for web, application, and database tiers
- Cloud security group and network policy management for IaaS workloads
- Policy change workflow with impact simulation before enforcement
- Ongoing policy tuning as applications evolve and new workloads are deployed
- Quarterly segmentation posture review with coverage metrics and gap analysis

## What's Not Included
- Network perimeter segmentation between sites or security zones (covered under [[Macrosegmentation]])
- Application firewall (WAF) policy management for web-facing services
- Container network policy management for Kubernetes environments
- Zero Trust Network Access for remote users (covered under [[Remote_Access_Management]])
- Penetration testing to validate segmentation effectiveness

## Dependencies
- [[Macrosegmentation]] — microsegmentation policies sit inside the broader security zone boundaries defined at the macro level
- [[Virtualization]] — hypervisor-level enforcement depends on the virtualization platform managed by this service
- [[Configuration_Management]] — workload attributes used in policy tagging are sourced from the CMDB
- [[Monitoring]] — policy violation alerts feed into the central monitoring and SIEM platforms
