---
name: "Virtualization & IaaS"
domain: Infrastructure
tags: [virtualization, iaas, hypervisor, cloud, vm-management]
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
Virtualization & IaaS manages the hypervisor layer and cloud infrastructure-as-a-service environments that underpin a customer's compute workloads, whether hosted on-premises (VMware, Hyper-V) or in public cloud platforms (Azure, AWS). Mid-market organizations benefit from expert capacity management, live migration orchestration, and cloud cost governance that prevents the sprawl and overspend that typically accompany self-managed cloud estates.

## What's Included
- Hypervisor platform management (VMware vSphere, Microsoft Hyper-V) including host and cluster configuration
- Virtual machine lifecycle management: provisioning, resizing, snapshot policy, and decommissioning
- IaaS resource management on public cloud platforms: compute, storage, virtual networking, and scaling groups
- Capacity planning and right-sizing analysis with actionable cost optimization recommendations
- Hypervisor and cloud platform patch and upgrade management
- High-availability and live-migration configuration for supported platforms
- Cloud cost reporting with resource tagging governance and anomaly alerting

## What's Not Included
- Platform-as-a-Service (PaaS) or Software-as-a-Service (SaaS) management
- Container orchestration and Kubernetes cluster management
- Application migration planning or replatforming projects
- Data-center physical infrastructure (power, cooling, physical servers) management
- Multi-cloud brokering or cloud-native architecture consulting

## Dependencies
- [[Deployment]] — VM provisioning follows the standard deployment pipeline managed by this service
- [[Monitoring]] — hypervisor host and VM health metrics are consumed by the central monitoring platform
- [[Backup_and_DR]] — VM-aware backup and snapshot policies are coordinated with the DR strategy
- [[IT_Asset_Management]] — virtual and cloud assets are tracked in the asset management inventory
