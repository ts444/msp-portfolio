---
name: "Device Hardening"
domain: Security
tags: [hardening, cis-benchmarks, baseline, attack-surface-reduction, compliance]
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
Device Hardening systematically reduces the exploitable attack surface of servers, workstations, and network devices by applying security configuration baselines derived from industry standards such as CIS Benchmarks and DISA STIGs. For mid-market organizations, a hardened device baseline is the most cost-effective preventive control available — neutralizing entire categories of initial access and privilege escalation techniques before they can be exploited.

## What's Included
- CIS Benchmark or equivalent security baseline development for all major OS types in the environment
- Automated baseline application using Group Policy, configuration management tooling, or MDM
- Attack surface reduction configuration: disabling unnecessary services, ports, protocols, and legacy authentication methods
- Application allowlisting policy design and enforcement for high-risk device classes
- Local administrator account management: renaming, credential rotation, and LAPS deployment
- Hardening compliance scanning with deviation reporting and remediation tracking
- Baseline review and update following major OS releases or significant new threat developments

## What's Not Included
- Network device firmware hardening (covered under [[Configuration_Management]])
- Mobile device hardening for BYOD personal devices
- Cloud workload security posture management (CSPM) for cloud-native services
- Custom application security configuration review
- Physical device security controls (BIOS/UEFI passwords, drive encryption keys) — encryption managed separately

## Dependencies
- [[Configuration_Management]] — hardening baselines are enforced through the configuration management tooling and tracked in the CMDB
- [[Patch_Management]] — current patch state is a prerequisite for achieving full hardening benchmark scores
- [[Endpoint_Detection_and_Response]] — EDR complements hardening by detecting exploitation attempts against residual attack surface
- [[Vulnerability_Management]] — hardening gaps identified in vulnerability scans feed back into baseline updates
