---
name: "Backup & Disaster Recovery"
domain: Security
tags: [backup, disaster-recovery, rto, rpo, ransomware-resilience]
pricing:
  bronze: 25
  silver: 33
  gold: 40
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Backup & Disaster Recovery ensures that data and critical systems can be restored to a defined recovery point within an agreed recovery time, protecting mid-market organizations from data loss caused by ransomware, hardware failure, accidental deletion, or site-level disasters. The service implements the 3-2-1-1 backup principle — three copies, two media types, one offsite, one offline or immutable — giving organizations a recovery path that ransomware cannot encrypt or delete.

## What's Included
- Backup policy design aligned to customer-defined RTO and RPO requirements per system tier
- Agent-based and agentless backup of servers, VMs, and cloud workloads with incremental forever scheduling
- Immutable backup copy management with air-gap or object lock protection against ransomware
- Offsite and/or cloud backup replication to a geographically separate location
- Monthly automated restore testing with documented results and any identified gaps
- Disaster recovery runbook development and annual DR test exercise facilitation
- Backup job monitoring with proactive alerting on failures and retention violations

## What's Not Included
- High availability (HA) or clustering design for zero-downtime failover (separate from DR recovery)
- SaaS data backup (Microsoft 365, Salesforce, Google Workspace) — requires a separate SaaS backup engagement
- Database-specific transaction log backup for real-time RPO requirements below 15 minutes
- Physical tape library management or offsite tape courier services
- Application-layer recovery testing beyond file and VM restore verification

## Dependencies
- [[Business_Continuity]] — recovery time objectives and restoration sequences are defined in the BCP
- [[Virtualization]] — VM-aware backup integrates with the hypervisor platform for consistent snapshots
- [[Monitoring]] — backup job status and retention compliance are monitored through the central platform
- [[IT_Change_Management]] — DR test exercises are registered as planned changes to avoid monitoring false alarms
