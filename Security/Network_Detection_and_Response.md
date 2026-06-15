---
name: "Network Detection & Response (NDR)"
domain: Security
tags: [ndr, network-detection, traffic-analysis, lateral-movement, east-west]
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
Network Detection & Response analyses raw network traffic and flow data across north-south and east-west network segments to detect threats that bypass endpoint and perimeter controls — including lateral movement, command-and-control beaconing, and data staging for exfiltration. For mid-market organizations, NDR provides the network-layer visibility that makes the difference between detecting a breach in hours and discovering it months later during a forensic investigation.

## What's Included
- Network traffic analysis using behavioral baselines and ML-based anomaly detection across monitored segments
- East-west traffic inspection for lateral movement indicators (credential reuse, unusual protocol usage, port scanning)
- Encrypted traffic analysis (ETA) to detect threats in TLS flows without decryption
- Command-and-control (C2) and DNS tunneling detection using protocol and behavioral analytics
- Alert triage and investigation with full packet capture retrieval for confirmed detections
- NDR telemetry and alert forwarding to SIEM for cross-source threat correlation
- Monthly detection coverage review and sensor placement assessment

## What's Not Included
- Host-based behavioral detection on endpoints (covered under [[Endpoint_Detection_and_Response]])
- Inline blocking or active network response (detection-only; response actions are escalated to operations)
- Network performance monitoring (covered under [[Network_Performance]])
- Full packet capture archiving beyond the defined retention window
- OT/SCADA protocol-aware network monitoring

## Dependencies
- [[SIEM]] — NDR alerts and flow data are ingested by SIEM for correlation with endpoint and identity event data
- [[Interconnection]] — network sensors are deployed at strategic points within the switching and routing infrastructure
- [[Macrosegmentation]] — monitoring coverage is mapped to the defined security zone topology
- [[Endpoint_Detection_and_Response]] — NDR and EDR detections are correlated in SIEM to build complete attack timelines
