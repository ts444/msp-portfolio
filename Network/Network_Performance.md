---
name: "Network Performance Management"
domain: Network
tags: [qos, traffic-shaping, performance, monitoring, bandwidth]
pricing:
  bronze: 15
  silver: 22
  gold: 30
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Network Performance Management ensures that business-critical applications consistently receive the bandwidth and latency they need by implementing and maintaining QoS policies and traffic-shaping rules across the network. For mid-market organizations running latency-sensitive workloads like VoIP, video conferencing, and cloud-hosted ERP, the service prevents best-effort traffic from crowding out revenue-impacting applications and provides the visibility needed to diagnose performance complaints before they escalate.

## What's Included
- QoS policy design and enforcement across WAN edge, core switches, and wireless infrastructure
- Traffic classification using DSCP marking, deep packet inspection, or application signatures
- Traffic shaping and policing rules with defined bandwidth guarantees per application class
- Real-time and historical network performance dashboards (latency, jitter, packet loss, utilization)
- Proactive alerting on threshold breaches with root-cause identification
- Monthly performance reports with trend analysis and capacity recommendations
- Policy tuning in response to new applications or changing traffic patterns

## What's Not Included
- Application-level performance optimization (e.g., database query tuning or CDN configuration)
- WAN circuit upgrades or ISP negotiations (covered under [[WAN]])
- SD-WAN application-aware routing policy management (covered under [[Interconnection]])
- Network hardware procurement or replacement
- Performance testing or load simulation engagements

## Dependencies
- [[WAN]] — WAN link quality data is essential input for performance baselining and alerting
- [[Interconnection]] — QoS markings are applied and honored within the switching and routing layer
- [[Wireless]] — wireless client performance metrics are included in the performance management scope
- [[Monitoring]] — performance threshold alerts integrate with the central monitoring and ticketing platform
