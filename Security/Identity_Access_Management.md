---
name: "Identity & Access Management (IAM)"
domain: Security
tags: [iam, identity, pim, pam, sso, mfa, directory]
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
Identity & Access Management governs who can access which systems and data, under what conditions, and with what level of privilege — covering the full identity lifecycle from onboarding to offboarding. The service includes Privileged Identity Management (PIM) for just-in-time elevation of admin rights and Privileged Access Management (PAM) for session recording and credential vaulting of administrative accounts, giving mid-market organizations the identity controls required by modern cyber insurance policies and compliance frameworks.

## What's Included
- Identity directory management (Active Directory, Entra ID / Azure AD, or equivalent) including user, group, and OU administration
- Single Sign-On (SSO) configuration and management for SaaS and internal applications
- Multi-factor authentication (MFA) policy enforcement across all managed identity providers
- Privileged Identity Management (PIM): just-in-time privilege elevation with approval workflows and time-limited access
- Privileged Access Management (PAM): privileged session recording, credential vaulting, and privileged account lifecycle management
- Joiner-mover-leaver (JML) process automation tied to HR system integration
- Quarterly access certification campaigns with manager-driven review and attestation

## What's Not Included
- Physical access control system integration (badge readers, door controllers)
- Customer identity and access management (CIAM) for consumer-facing applications
- Role-based access control design for custom-developed applications
- Identity governance and administration (IGA) platform implementation beyond the included JML automation
- Biometric authentication system management

## Dependencies
- [[Remote_Access_Management]] — remote access entitlements are governed by IAM group memberships and policies
- [[Secret_Management]] — privileged account credentials are vaulted through the secrets management platform
- [[SIEM]] — authentication logs and privileged access events are forwarded to SIEM for anomaly detection
- [[Network_Access_Control]] — NAC admission decisions consume identity attributes from the directory
