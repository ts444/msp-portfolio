---
name: "Configuration Management"
domain: Infrastructure
tags: [configuration, cmdb, automation, compliance, drift-detection]
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
Configuration Management provides mid-market organizations with a structured, automated approach to defining, enforcing, and auditing the desired state of servers, endpoints, and network devices. By maintaining a continuously updated Configuration Management Database (CMDB) and applying policy-as-code techniques, the service eliminates configuration drift and reduces the attack surface introduced by unmanaged or inconsistently configured systems.

## What's Included
- Maintained CMDB covering all managed servers, endpoints, and network devices
- Policy-as-code enforcement using industry-standard tooling (e.g., Ansible, DSC, or equivalent)
- Continuous configuration drift detection with automated alerting on deviations
- Golden-image baseline definition and version control for all device classes
- Scheduled and on-demand compliance reporting against CIS Benchmarks or customer-defined standards
- Change correlation — linking configuration changes to approved change records
- Rollback procedures and tested runbooks for rapid remediation of unauthorized changes

## What's Not Included
- Software license management or procurement (covered under [[IT_Asset_Management]])
- Application-level configuration management for custom-developed software
- Cloud-native infrastructure-as-code pipeline development (e.g., Terraform module authoring)
- Configuration of OT/SCADA or industrial control systems
- Physical hardware provisioning or rack-and-stack activities

## Dependencies
- [[Deployment]] — baseline configurations are applied as part of the deployment workflow
- [[Patch_Management]] — patch state is tracked as a configuration attribute in the CMDB
- [[Monitoring]] — configuration drift alerts feed into the infrastructure monitoring dashboard
- [[IT_Change_Management]] — configuration changes must reference approved change records
