# AI Governance Executive Guide Series

Practical frameworks for governing AI systems across regulated industries—built on the principle that governance must produce evidence, not just assertions.

> *"Governance is the authorization boundary: the point where outputs become decisions, and where evidence—not explanations—must exist."*

## Overview

AI is being deployed in high-stakes environments—financial services, healthcare, federal programs—where decisions affect people's lives, livelihoods, and rights. Yet most organizations lack the governance infrastructure to answer a basic question: **"How do you know your AI is doing what it's supposed to do?"**

The existing frameworks (SR 11-7, NIST AI RMF, OMB M-24-10) tell you *what* to care about. They don't tell you *how to know* you're actually governing. That's the gap these guides fill.

Each guide provides industry-specific, operationally practical governance frameworks—tiered by risk, aligned to regulatory expectations, and designed to produce the evidence that auditors and regulators actually require.

## The Guides

| Volume | Title | Audience | Description |
|--------|-------|----------|-------------|
| **1** | [Financial Services](guides/FS_AI_Governance_Guide_v1.0.pdf) | CROs, Model Risk Officers, Compliance | SR 11-7 alignment, third-party risk, enterprise AI risk management |
| **2** | [Healthcare](guides/Healthcare_AI_Governance_Guide_v1.0.pdf) | CMOs, Clinical Informatics, Quality Officers | Clinical AI safety, FDA compliance, patient protection |
| **3** | [Federal Programs](guides/FedPrograms_AI_Governance_Guide_v1.0.pdf) | Agency CAIOs, Program Managers, COs/CORs | Acquisition, oversight, and mission assurance for government buyers |
| **4** | [Government Contractors](guides/GovContractors_AI_Governance_Guide_v1.0.pdf) | Contractor CTOs, Capture Managers, Proposal Teams | Winning work, protecting relationships, surviving audits |

## Key Concepts

### Evidence Over Assertion
Move from "we have policies" to "here's proof." Every framework is designed to produce audit-grade artifacts, not just documentation.

### Four-Tier Risk Classification
Not all AI requires the same oversight. Classification ensures governance intensity matches actual risk:

| Tier | Risk Level | Examples |
|------|------------|----------|
| **Tier 1** | Critical | Rights-impacting, safety-impacting, mission-critical AI |
| **Tier 2** | Elevated | Operational impact, employee-facing, significant data |
| **Tier 3** | Standard | Internal operations, no direct citizen/patient/customer impact |
| **Tier 4** | Minimal | Personal productivity, no sensitive data |

### Two Governance Tracks
- **Decisioning AI** — Outputs that drive decisions affecting people or operations
- **Communications AI** — Content generation with records management and disclosure implications

### The Governed Unit
The unit of governance is not "the model" — it's an AI system performing a defined use case within a business process, including its inputs, outputs, integrations, and decision authority. The same AI in different contexts = different Governed Units, each independently classified.

## Technical Foundation

These guides are built on the [Four Tests Standard (4TS)](https://github.com/edmeyman/4ts-standard), an open specification for verifiable AI governance. 4TS defines what it means for an AI decision to be governed: authorized, validated, monitored, and auditable.

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to:
- **Share** — copy and redistribute the material in any medium or format
- **Adapt** — remix, transform, and build upon the material for any purpose, including commercial

Under the following terms:
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.

### Attribution

When citing or reusing this work, use:

```
FERZ LLC, "AI Governance Executive Guide Series," 2025. 
Available at https://github.com/edmeyman/ai-governance-guides
Licensed under CC BY 4.0.
```

## Canonical Source

The official download location is [ferzconsulting.com/services-overview/strategic-advisory-services/ai-governance-executive-guides](https://ferzconsulting.com/services-overview/strategic-advisory-services/ai-governance-executive-guides).

This repository mirrors the official releases for version control and citability.

## Version History

See [CHANGELOG.md](CHANGELOG.md) for release history.

## Contact

For inquiries regarding the guides or licensing discussions: [ferz.ai](https://ferz.ai)

---

© 2026 FERZ, Inc. All rights reserved.
