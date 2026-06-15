---
name: "Infrastructure Monitoring"
domain: Infrastructure
tags: [monitoring, alerting, observability, uptime, performance]
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
Infrastructure Monitoring provides continuous visibility into the health, performance, and availability of servers, network devices, cloud resources, and critical services across the customer's environment. Rather than reacting to outages after users report them, the service uses threshold-based and anomaly-based alerting to surface issues early, giving the operations team time to investigate and resolve before business impact occurs.

## What's Included
- Agent-based and agentless monitoring of servers, endpoints, and network devices (CPU, memory, disk, interface metrics)
- Availability monitoring for critical services and applications with configurable check intervals
- Synthetic transaction monitoring for web-based applications and authentication flows
- Alert routing to appropriate on-call teams with severity classification and escalation policies
- Centralized monitoring dashboard accessible to customer IT stakeholders
- Monthly availability and incident trend reports
- Monitoring scope review and tuning on a quarterly basis to reduce alert noise

## What's Not Included
- Application performance monitoring (APM) for custom-developed software (requires a separate engagement)
- Log management and security event correlation (covered under [[SIEM]])
- End-user experience monitoring or digital experience management tools
- Monitoring of infrastructure not managed under an active MSP service agreement
- 24/7 staffed network operations center (NOC) response — alerting is routed per defined escalation paths

## Dependencies
- [[Configuration_Management]] — monitored device inventory is sourced from the CMDB
- [[SIEM]] — infrastructure events and alerts are forwarded to SIEM for security correlation
- [[IT_Change_Management]] — scheduled maintenance windows suppress alerting during approved changes
- [[Deployment]] — monitoring agents are deployed and configured as part of every new system provisioning
