---
name: "Secret Management"
domain: Security
tags: [secrets, certificates, pki, credentials, vault]
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
Secret Management provides centralized, audited storage and lifecycle management for the credentials, API keys, certificates, and cryptographic secrets that modern infrastructure depends on. For mid-market organizations, secrets sprawled across configuration files, spreadsheets, and shared inboxes represent one of the most common breach vectors; this service replaces ad-hoc practices with a vault-based platform, automated rotation policies, and a complete audit trail of every secret access.

## What's Included
- Secrets vault deployment and management (e.g., HashiCorp Vault, Azure Key Vault, or equivalent)
- Onboarding of credentials, API keys, database passwords, and service account secrets into the vault
- Automated secret rotation for supported systems with zero-downtime rotation workflows
- TLS/SSL certificate lifecycle management: issuance, renewal, revocation, and expiry alerting
- Internal PKI management for machine and service identities
- Secret access audit logging with alerting on unauthorized or anomalous access attempts
- Secret sprawl discovery scanning to identify hardcoded credentials in repositories and configurations

## What's Not Included
- Hardware security module (HSM) procurement or physical key ceremony management
- Code signing certificate management for software distribution pipelines
- End-user password management (covered under [[Identity_Access_Management]])
- SSH key management for end-user workstations
- Secrets management for custom application code (requires development team integration)

## Dependencies
- [[Identity_Access_Management]] — vault access policies are tied to identity and role assignments managed in IAM
- [[Configuration_Management]] — configuration baselines reference vault paths rather than plaintext secrets
- [[DNS]] — certificate validation workflows depend on DNS management
- [[Monitoring]] — certificate expiry alerts and vault availability are monitored through the central platform
