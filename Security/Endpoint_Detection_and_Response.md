---
name: "Endpoint Detection & Response (EDR)"
domain: Security
tags: [edr, endpoint, threat-detection, response, peripheral-control]
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
Endpoint Detection & Response deploys a lightweight agent on servers, workstations, and laptops that provides continuous behavioral monitoring, threat detection, and remote response capabilities far beyond what traditional antivirus can deliver. For mid-market organizations, the service includes peripheral control policies that govern USB and removable media usage — a frequently overlooked data exfiltration and malware introduction vector — alongside the telemetry integration that feeds the SIEM with endpoint-level visibility.

## What's Included
- EDR agent deployment and management on all in-scope Windows, macOS, and Linux endpoints
- Behavioral threat detection using MITRE ATT&CK-aligned detection logic with continuous updates
- Peripheral control policy management: USB storage block/allow lists, removable media restrictions, and printer controls
- Automated threat containment actions (process termination, network isolation) with defined escalation thresholds
- Threat alert triage, investigation, and escalation to defined security contacts
- Endpoint telemetry forwarding to SIEM for cross-source correlation
- Monthly EDR coverage and detection efficacy reporting

## What's Not Included
- Mobile device management (MDM) for iOS and Android devices
- Data loss prevention (DLP) for cloud applications and email channels
- Application whitelisting and execution control beyond EDR-native capabilities (covered under [[Device_Hardening]])
- Full incident response and forensic investigation engagements
- Network-layer threat detection (covered under [[Network_Detection_and_Response]])

## Dependencies
- [[SIEM]] — EDR telemetry and alerts are a primary data source for security event correlation
- [[Device_Hardening]] — hardening baselines reduce the attack surface that EDR must defend
- [[Patch_Management]] — current OS and application patches reduce the exploitable vulnerabilities EDR must detect
- [[Identity_Access_Management]] — user context from the identity platform enriches EDR alert triage
