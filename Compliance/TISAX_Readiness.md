---
name: "TISAX Readiness Assessment"
domain: Compliance
tags: [tisax, vda-isa, automotive, readiness-assessment, information-security, supplier]
pricing:
  bronze: 3000
  silver: 6000
  gold: 12000
unit: per-engagement
sla:
  bronze: { availability: "business-hours", response: "1bd", resolution_p1: "5bd", resolution_p2: "10bd" }
  silver: { availability: "business-hours", response: "4h", resolution_p1: "3bd", resolution_p2: "5bd" }
  gold:   { availability: "extended-hours", response: "2h", resolution_p1: "1bd", resolution_p2: "3bd" }
---

## Overview
TISAX Readiness Assessment prepares automotive suppliers and OEM partners for Trusted Information Security Assessment Exchange (TISAX) audits by scoping the applicable TISAX label, performing a gap assessment against the VDA ISA (Information Security Assessment) catalogue, and delivering a prioritised remediation roadmap. The service enables customers to enter a TISAX assessment with a defined control baseline and no critical non-conformities, avoiding the delay and cost of a failed audit cycle.

## What's Included
- TISAX label scoping: determination of required labels (Info High, Proto, Prototype Parts) based on data handled and OEM contractual obligations
- Baseline gap assessment against the current VDA ISA version covering all applicable control objectives
- Remediation roadmap: prioritised action plan with effort estimates, owners, and target completion dates aligned to the assessment window
- Evidence preparation guidance: documentation templates and artefact checklists for auditor submission
- Pre-assessment internal review: simulation of the TISAX assessment to validate readiness before ENX portal registration
- ENX portal registration support and assessment body coordination

## What's Not Included
- The TISAX assessment itself (conducted by an accredited TISAX assessment provider through ENX)
- ISO 27001 certification — although controls overlap, TISAX and ISO 27001 are separate schemes (see [[ISMS_Programme]])
- Remediation project delivery beyond recommendations (available as a separate engagement)
- Third-party supplier TISAX audits on behalf of the customer

## Dependencies
- [[ISMS_Programme]] — existing ISMS controls form the foundation for TISAX compliance; overlapping controls are mapped to reduce remediation scope
- [[IT_Asset_Management]] — asset inventory and data classification are required inputs to the VDA ISA control assessment
- [[IT_Risk_Management]] — IT risk register provides input to TISAX risk treatment objective evidence
