---
name: "Patch Management"
domain: Infrastructure
tags: [patching, vulnerability, os, third-party, compliance]
pricing:
  bronze: 15
  silver: 22
  gold: 32
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---

## Overview
Patch Management provides a structured, risk-prioritized approach to keeping operating systems and third-party applications current across servers, endpoints, and network devices. For mid-market organizations, unpatched systems are consistently the most exploited entry point; this service eliminates the manual effort and inconsistency of ad-hoc patching by delivering automated deployment, rollback capabilities, and compliance evidence that satisfies auditors and cyber insurers.

## What's Included
- OS patch management for Windows and Linux servers and endpoints on a defined patching cadence
- Third-party application patching for common software (browsers, Office suites, Java, PDF readers, and others in the approved catalog)
- Patch testing in a staging ring before production rollout, with defined rollback procedures
- Emergency/out-of-band patch deployment for critical CVEs within defined SLA windows
- Patch compliance dashboards showing coverage, exceptions, and aging metrics
- Patch exception management with compensating control documentation and review cycles
- Monthly patch status reports with trending and risk-prioritization commentary

## What's Not Included
- Custom or internally developed application patching
- Firmware updates for network devices (covered under [[Interconnection]] and [[Configuration_Management]])
- Patching of OT/SCADA or industrial control systems
- Vulnerability scanning and severity prioritization (covered under [[Vulnerability_Management]])
- Software procurement or license management for patched applications

## Dependencies
- [[Vulnerability_Management]] — vulnerability scan results inform patch prioritization and exception risk scoring
- [[Configuration_Management]] — patch state is tracked as a configuration attribute in the CMDB
- [[Monitoring]] — failed patch jobs and compliance drift trigger alerts in the monitoring platform
- [[IT_Change_Management]] — patch deployment windows are registered as standard or emergency changes
