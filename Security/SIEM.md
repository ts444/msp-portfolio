---
name: "Security Information & Event Management (SIEM)"
domain: Security
tags: [siem, log-management, correlation, detection, alerting]
pricing:
  bronze: 28
  silver: 36
  gold: 40
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
SIEM provides centralized collection, normalization, and correlation of security events from across the customer's infrastructure, enabling detection of threats that no single point solution can identify in isolation. For mid-market organizations, the service delivers enterprise-grade detection coverage without the cost of building an in-house security operations team, supported by curated detection rules, threat-intelligence-enriched alerts, and documented triage and escalation procedures.

## What's Included
- Log ingestion and normalization from servers, endpoints, firewalls, identity providers, and cloud platforms
- Out-of-the-box and custom detection rule management aligned to MITRE ATT&CK
- Threat intelligence integration to enrich alerts with IOC context
- Alert triage and escalation to the customer's IT team or defined security contacts
- Incident timeline reconstruction and forensic evidence preservation for investigated alerts
- Compliance-mapped reporting for common frameworks (ISO 27001, SOC 2, NIS2)
- Quarterly detection rule tuning to reduce false positives and address emerging threat patterns

## What's Not Included
- 24/7 staffed Security Operations Center (SOC) with active threat hunting (available as a separate MDR engagement)
- Digital forensics and incident response (DFIR) beyond initial evidence preservation
- Endpoint telemetry collection (requires [[Endpoint_Detection_and_Response]] integration)
- Deception technology alert ingestion (requires [[Deception]] integration)
- Custom SIEM platform development or self-hosted infrastructure management

## Dependencies
- [[Endpoint_Detection_and_Response]] — EDR telemetry is a primary log source for endpoint-level detection
- [[Network_Detection_and_Response]] — NDR flow and alert data are ingested for network-layer correlation
- [[Identity_Access_Management]] — authentication and directory logs are critical SIEM data sources
- [[Monitoring]] — infrastructure events from the monitoring platform are forwarded to the SIEM
