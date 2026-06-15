---
name: "DNS Management"
domain: Network
tags: [dns, name-resolution, dnssec, filtering, availability]
pricing:
  bronze: 15
  silver: 20
  gold: 28
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
DNS Management provides authoritative and recursive DNS services with high availability, DNSSEC validation, and protective DNS filtering that blocks malicious domains before connections are established. For mid-market organizations, reliable DNS is a foundational dependency for every cloud service, SaaS application, and internal resource — making proactive DNS management a high-leverage, low-visibility control that prevents outages and reduces malware dwell time.

## What's Included
- Internal recursive DNS server management with redundant resolvers and automatic failover
- Authoritative DNS zone management for all internal and externally registered domains
- DNSSEC signing and validation for managed zones
- Protective DNS filtering with category-based blocking (malware, phishing, command-and-control)
- DNS record lifecycle management: creation, modification, TTL optimization, and cleanup
- DNS query logging and anomaly detection for DNS-based exfiltration attempts
- Quarterly DNS health review and record audit

## What's Not Included
- Domain name registration, renewal, or registrar account management
- Application-layer load balancing using DNS (e.g., GeoDNS or global server load balancing)
- Public CDN DNS configuration management
- Certificate issuance or management tied to DNS-01 ACME challenges (covered under [[Secret_Management]])
- Split-horizon DNS architectures requiring custom application-layer logic

## Dependencies
- [[Interconnection]] — DNS resolvers are reachable through the routed network managed by this service
- [[Wireless]] — wireless clients depend on DNS resolution for all application connectivity
- [[Secret_Management]] — DNS-based certificate validation workflows interact with certificate lifecycle management
- [[Monitoring]] — DNS resolver availability and query latency are monitored through the central platform
