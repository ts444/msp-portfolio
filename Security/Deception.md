---
name: "Deception Technology"
domain: Security
tags: [deception, honeypot, canary, threat-detection, early-warning]
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
Deception Technology deploys decoy assets — fake servers, credentials, files, and network services — throughout the customer's environment to detect attackers who have already bypassed perimeter controls and are conducting internal reconnaissance. For mid-market organizations, deception provides a high-fidelity, near-zero-false-positive early warning system that dramatically reduces dwell time by alerting the moment an adversary interacts with a resource no legitimate user should ever touch.

## What's Included
- Design and deployment of deception decoys appropriate to the environment (honey servers, honey credentials, honey files, honey DNS records)
- Decoy asset placement strategy aligned to the network topology and attacker lateral movement paths
- Real-time alerting with high-fidelity context (source IP, accessed decoy, timing, and technique) on any decoy interaction
- Integration of deception alerts into SIEM for correlation with other detection signals
- Decoy lifecycle management: rotation, updating, and replacement to maintain plausibility
- Quarterly deception coverage review to ensure decoys remain relevant as the environment evolves
- Incident handoff with interaction logs to support forensic investigation

## What's Not Included
- Active deception or adversary engagement (hack-back) activities
- Internet-facing honeypot deployment for external threat intelligence gathering
- Physical deception assets (fake documents, hardware implants)
- Penetration testing to validate decoy detectability
- Managed threat hunting or active threat investigation (covered under [[SIEM]])

## Dependencies
- [[SIEM]] — deception alerts are forwarded to SIEM for correlation with complementary detection signals
- [[Topologies]] — accurate network topology is required to place decoys on plausible lateral movement paths
- [[Network_Detection_and_Response]] — NDR flow visibility helps validate that decoy traffic is isolated from production flows
- [[Identity_Access_Management]] — honey credentials are created as low-privilege accounts in the identity directory
