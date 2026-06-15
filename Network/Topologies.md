---
name: "Network Topology Management"
domain: Network
tags: [topology, documentation, network-diagram, change-management, inventory]
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
Network Topology Management maintains an accurate, always-current map of the customer's network infrastructure — from physical cabling and device interconnections to logical VLAN assignments and cloud peering points. For mid-market organizations that have grown organically, undocumented topology is a major risk multiplier during incidents and audits; this service turns network documentation from a periodic project into a continuously maintained operational asset.

## What's Included
- Automated network discovery to identify all managed devices, interfaces, and connections
- Logical and physical topology diagrams maintained and version-controlled after every change
- VLAN, subnet, and routing table documentation kept synchronized with the live network
- Network device inventory with hardware model, firmware version, and end-of-support dates
- Topology-based impact analysis to support change requests and incident response
- Annual topology review workshop with the customer's IT team
- Integration of topology data into ITSM and CMDB platforms where applicable

## What's Not Included
- Application dependency mapping or service-level topology visualization
- Physical data-center floor plans or rack elevation diagrams (requires a separate professional services engagement)
- Cloud infrastructure topology management for IaaS resources (covered under [[Virtualization]])
- Network design consulting or greenfield architecture engagements
- Automated topology enforcement or configuration remediation (covered under [[Configuration_Management]])

## Dependencies
- [[Interconnection]] — switching and routing changes are reflected immediately in topology documentation
- [[WAN]] — WAN circuit endpoints and CPE devices are included in the topology inventory
- [[Wireless]] — access point placement and controller topology are part of the managed documentation set
- [[IT_Change_Management]] — topology updates are triggered by approved change records
