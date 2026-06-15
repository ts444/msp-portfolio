---
name: "DDoS Protection"
domain: Security
tags: [ddos, availability, scrubbing, mitigation, internet-resilience]
pricing:
  bronze: 20
  silver: 28
  gold: 38
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "15m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
DDoS Protection provides always-on volumetric and application-layer attack detection and mitigation, ensuring that internet-facing services remain reachable during distributed denial-of-service campaigns. For mid-market organizations that rely on web portals, customer-facing APIs, or VPN gateways for daily operations, even a one-hour DDoS-induced outage can translate directly to revenue loss and reputational damage — making proactive scrubbing and rapid mitigation a business-critical investment.

## What's Included
- Always-on traffic baselining and volumetric attack detection at the network edge
- Cloud-based scrubbing center integration for traffic diversion during large-scale volumetric attacks
- On-premises mitigation policy management for application-layer (layer-7) and protocol-layer attacks
- Attack detection alerting with automated mitigation triggering and human escalation
- Real-time attack dashboards and post-attack reports with traffic analysis and attack vector classification
- Anycast or BGP-based traffic diversion configuration and testing
- Annual DDoS simulation exercise to validate mitigation effectiveness and response procedures

## What's Not Included
- Web application firewall (WAF) management for application-layer exploit prevention (separate from DDoS L7 rate limiting)
- Content delivery network (CDN) provisioning or optimization
- ISP-level upstream filtering negotiation with the customer's internet provider (covered under [[WAN]])
- DDoS protection for internal network segments not accessible from the internet
- SaaS platform availability (e.g., Microsoft 365, Salesforce) — dependent on vendor SLA

## Dependencies
- [[WAN]] — internet circuit health and ISP relationships are prerequisites for effective traffic diversion
- [[Macrosegmentation]] — DDoS mitigation policies are coordinated with perimeter firewall zone controls
- [[Monitoring]] — attack detection events feed into the central monitoring platform for incident tracking
- [[Business_Continuity]] — DDoS response procedures are incorporated into the BCP escalation playbooks
