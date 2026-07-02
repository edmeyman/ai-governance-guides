# AI Governance Executive Guide Series

Practical frameworks for governing AI systems across regulated industries, built on the principle that governance must produce evidence, not just assertions.

> *"Governance is enforced at the authorization boundary: the point where an output becomes an effect-bearing action, and where evidence, not explanations, must exist."*

## Overview

AI is being deployed in high-stakes environments where outputs can affect people, operations, safety, access, compliance, and public trust. Most organizations can describe policies, oversight roles, and monitoring procedures. Fewer can answer the harder question:

**Was this specific AI action permitted before it executed, and can that determination be independently reconstructed?**

The AI Governance Executive Guide Series provides practical, sector-specific frameworks for answering that question. The guides are designed around classification, evidence, oversight, authorization-boundary controls, fail-closed operation, and audit readiness.

The guides are foundational governance frameworks, not exhaustive policy trackers or current-law references. They cite statutes, regulations, memoranda, standards, and guidance only where those sources materially affect the general governance model, compliance or acquisition posture, evidence requirements, oversight structure, or audit-readiness framework. Use-case-specific, agency-specific, jurisdiction-specific, or rapidly changing requirements should be verified separately before reliance or implementation.

## The Guides

The PDF filenames retain the original stable link names. Each PDF identifies its current version in its cover and front matter.

| Volume | Title | Audience | Description |
|--------|-------|----------|-------------|
| **1** | [Financial Services](guides/FS_AI_Governance_Guide_v1.0.pdf) | CROs, Model Risk Officers, Compliance, Internal Audit | Model-risk governance, evidence requirements, third-party oversight, authorization artifacts, and examiner-ready AI governance |
| **2** | [Healthcare](guides/Healthcare_AI_Governance_Guide_v1.0.pdf) | CMOs, Clinical Informatics, Quality Officers, Compliance | Clinical AI governance, patient-safety evidence, human oversight, authorization-boundary controls, and audit-ready documentation |
| **3** | [Federal Programs](guides/FedPrograms_AI_Governance_Guide_v1.0.pdf) | Agency CAIOs, Program Managers, COs/CORs, IG Staff | Acquisition, contractor oversight, evidence packages, mission assurance, and Inspector General audit readiness |
| **4** | [Government Contractors](guides/GovContractors_AI_Governance_Guide_v1.0.pdf) | Contractor CTOs, Capture Managers, Proposal Teams, Compliance Officers | Contractor evidence packages, subcontractor governance, proposal readiness, audit response, and authorization-ready delivery |

## Key Concepts

### Evidence Over Assertion

Move from "we have policies" to "here is the evidence." Each guide is structured to help organizations produce governance records, evidence packages, and oversight documentation that can be reviewed, challenged, and maintained over time.

### Authorization Boundary

The authorization boundary is the point where an AI output becomes an effect-bearing action. For governed actions, the relevant question is not only what the AI produced, but whether that action was permitted before release under the applicable policy, authority chain, provenance condition, and oversight requirement.

### Authorization Artifact

An authorization artifact is a tamper-evident, replayable record showing whether a governed AI action was permitted before execution. Logs and monitoring data may support oversight, but they do not substitute for a pre-execution authorization artifact.

### Fail-Closed Design

If governance conditions are not met, the action does not proceed. A governed action releases only when it receives an ALLOW verdict. If the required authorization artifact cannot be produced, the action fails closed.

### Verdict Space

The verdict space is:

- **ALLOW**: the action is permitted under current policy and may execute.
- **DENY**: the action is prohibited under current policy and is blocked.
- **ABSTAIN**: policy cannot resolve the action to ALLOW or DENY. Execution is blocked pending authorized human override, and the override is itself a recorded authorization event.

There is no ESCALATE verdict and no HALT verdict. Escalation is the consequence of ABSTAIN, not a fourth verdict.

### Four-Tier Risk Classification

Not all AI requires the same oversight. Classification ensures governance intensity matches actual risk.

| Tier | Risk Level | Examples |
|------|------------|----------|
| **Tier 1** | Critical / high-impact | Rights-affecting, safety-affecting, mission-critical, clinical, financial, or citizen-facing AI |
| **Tier 2** | Elevated | Operational impact, employee-facing systems, significant data or workflow dependence |
| **Tier 3** | Standard | Internal operations with limited external effect |
| **Tier 4** | Minimal | Personal productivity or low-risk internal use |

### Two Governance Tracks

- **Decisioning AI**: outputs that drive or materially affect decisions, actions, eligibility, safety, operations, or resource allocation.
- **Communications AI**: content generation, correspondence, drafting, summarization, or records-related use with disclosure, attribution, or records-management implications.

### Governed Unit

The unit of governance is not "the model." It is an AI system performing a defined use case within a business process, including its inputs, outputs, integrations, and decision authority. The same model used in different contexts may produce different Governed Units, each independently classified and governed.

## Technical Foundation

These guides are built on the [Five Tests Standard (5TS)](https://doi.org/10.5281/zenodo.21040295), an open, vendor-neutral specification for proof-carrying authorization records in runtime AI authorization.

5TS defines five normative tests:

| Test | Requirement |
|------|-------------|
| **Stop** | The system can be halted before side effects occur. |
| **Ownership** | Each consequential decision maps to a named accountable authority. |
| **Replay** | The decision can be reproduced at the boundary. |
| **Escalation** | Control transfers at defined policy boundaries. |
| **Provenance** | The inputs grounding a verdict have an established origin. Origin, not truth. |

The 5TS explanatory foundation is published as:

**Verifiable AI Governance: The Five Tests Standard (5TS) and Proof-Carrying Decisions**  
DOI: [10.5281/zenodo.21048661](https://doi.org/10.5281/zenodo.21048661)

The open standard repository is maintained at:

[github.com/edmeyman/4ts-standard](https://github.com/edmeyman/4ts-standard)

The repository name remains `4ts-standard` for continuity.

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to:

- **Share**: copy and redistribute the material in any medium or format.
- **Adapt**: remix, transform, and build upon the material for any purpose, including commercial purposes.

Under the following terms:

- **Attribution**: you must give appropriate credit, provide a link to the license, and indicate if changes were made.

## Attribution

When citing or reusing this work, use:

```text
FERZ, Inc., "AI Governance Executive Guide Series," 2026.
Available at https://github.com/edmeyman/ai-governance-guides
Licensed under CC BY 4.0.
