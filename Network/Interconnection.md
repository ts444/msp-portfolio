---
name: "Network Interconnection"
domain: Network
tags: [switching, routing, dhcp, ip-addressing, sd-wan]
pricing:
  bronze: 20
  silver: 28
  gold: 38
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Network Interconnection is the foundational layer-2 and layer-3 management service that ties together all sites, VLANs, and cloud connections within a customer's environment. It encompasses IP address management, DHCP, switching, routing, and SD-WAN overlay policies, giving mid-market organizations a coherent, scalable internal network architecture without requiring dedicated in-house network engineers.

## What's Included
- IP addressing schema design, documentation, and ongoing management (IPAM)
- DHCP server configuration, scope management, lease monitoring, and failover
- Layer-2 switching configuration: VLANs, spanning tree, port security, and trunk policies
- Layer-3 routing configuration: static routes, OSPF/BGP peering, and inter-VLAN routing
- SD-WAN policy management: application-aware routing, link bonding, and failover rules
- Network topology documentation kept current after every change
- Scheduled firmware updates for switches and routers with tested rollback procedures

## What's Not Included
- Physical cabling, rack installation, or hardware procurement
- Wireless access point management (covered under [[Wireless]])
- WAN circuit provisioning and ISP relationship management (covered under [[WAN]])
- Firewall rule management beyond basic inter-VLAN ACLs (covered under [[Macrosegmentation]] or [[Microsegmentation]])
- Data-center fabric or spine-leaf architecture design

## Dependencies
- [[WAN]] — WAN circuits terminate into the routing layer managed by this service
- [[DNS]] — DNS servers are reachable through the routed network managed here
- [[Topologies]] — topology documentation is maintained in alignment with this service's change records
- [[Network_Performance]] — routing and switching metrics are consumed by performance management workflows
