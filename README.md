# MSP Portfolio

A service catalogue for a Managed Service Provider (MSP) targeting mid-market
organisations. Each note describes one managed service — what it includes,
how it is delivered, its pricing tiers, and the associated service levels.

This is an [Obsidian](https://obsidian.md) vault; the notes are plain Markdown
and can be read directly on GitHub or in any text editor.

## Structure

Services are organised into six domains:

| Domain | Services | Scope |
| --- | --- | --- |
| [Compliance](Compliance/) | 5 | GDPR, NIS2, TISAX, ISMS, and regulatory deadline tracking |
| [Governance](Governance/) | 5 | IT asset, change, risk, project, and knowledge management |
| [Infrastructure](Infrastructure/) | 6 | Deployment, patching, monitoring, virtualization, configuration & remote access |
| [Network](Network/) | 7 | WAN, VPN, wireless, DNS, topologies, performance & interconnection |
| [Security](Security/) | 19 | SIEM, EDR/NDR, IAM, vulnerability & incident response, segmentation, backup/DR, and more |
| [Workplace](Workplace/) | 4 | Collaboration, productivity, awareness training & remote work |

## Note format

Every service note carries YAML frontmatter with a consistent schema, followed
by descriptive sections (Overview, What's Included, and so on):

```yaml
---
name: "Service name"
domain: Security
tags: [tag1, tag2]
pricing:
  bronze: 28
  silver: 36
  gold: 40
unit: per-user/month
sla:
  bronze: { availability: "99.0%", response: "4h", resolution_p1: "8h", resolution_p2: "24h" }
  silver: { availability: "99.5%", response: "2h", resolution_p1: "4h", resolution_p2: "12h" }
  gold:   { availability: "99.9%", response: "30m", resolution_p1: "2h", resolution_p2: "6h" }
---
```

- **pricing** — tiered (bronze / silver / gold) in the stated `unit`.
- **sla** — per-tier availability, response time, and P1/P2 resolution targets.

## Usage

Open the folder as an Obsidian vault, or browse the Markdown files directly on
GitHub. The structured frontmatter makes the catalogue straightforward to parse
for downstream tooling (quoting, comparison, reporting).
