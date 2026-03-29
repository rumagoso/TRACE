# TRACE — Trusted Registry for Autonomous and Connected Entities

**A proposed open infrastructure standard for AI agent identity and accountability.**

---

## The Problem

AI agents book meetings, execute financial transactions, control industrial systems, and spawn sub-agents — across organisational and jurisdictional boundaries — with no shared infrastructure to answer a basic question:

> *Who are you, who sent you, and what are you authorised to do?*

Enterprise IAM standards (OAuth 2.0, SPIFFE/SPIRE, OpenID Connect) address agents operating inside a single organisation's trust perimeter. They were not designed for agents crossing that perimeter. No current standard was.

This is not a future risk. It is a present condition.

---

## What TRACE Is

TRACE is a proposed four-layer open standard to close this gap.

| Layer | Name | Function |
|---|---|---|
| 1 | Identity | Cryptographic identity bound to a verified legal entity, recorded on a permissioned ledger using W3C DIDs. Recursive Sub-Tokens enable high-velocity delegation without losing chain of custody. |
| 2 | Access | Resources query TRACE before granting access. Registered and in good standing: access at the appropriate trust tier. Unregistered: no access, without exception. |
| 3 | Governance | The TRACE Foundation — a multi-stakeholder non-profit modelled on ICANN — governs the registry at two speeds: automated Circuit Breakers for real-time containment, human supermajority for permanent revocation. |
| 4 | Economic Alignment | High-risk agents post conditional collateral held in escrow. On verified failure, collateral is released to a victim recourse pool. Clean records earn tiered infrastructure incentives. |

TRACE complements, not competes with, existing frameworks. It provides the identity substrate the EU AI Act assumes but does not specify; the accountability chain ISO 42001 requires but does not provision; the revocation mechanism NIS2 implies but does not mandate for AI.

---

## Status

| Milestone | Status |
|---|---|
| Position Paper v0.2 | Published — March 2026 |
| NIST NCCoE Public Comment | Submitted — March 2026 |
| CSA Blog Submission | Pending |
| Working Group Formation | Open for interest |

---

## Documents

- **Position Paper v0.2** — [LinkedIn](https://www.linkedin.com/pulse/registry-ai-agents-problem-rui-soares-bcyye/) — full architecture, threat model, standards alignment, and call to action
- **NIST NCCoE Public Comment** — submitted to AI-Identity@nist.gov ahead of the April 2, 2026 deadline — available in this repository

---

## Standards Alignment

TRACE is designed for compatibility with: W3C DID Core 1.0, OAuth 2.0, NIST SP 800-63-4, NIST AI RMF, ISO/IEC 42001, EU AI Act (Articles 9, 13, 22), NIS2 Directive, EBSI (EU deployments), CSA AICM.

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Author

**Rui Soares**
ISMS Manager, Crossjoin Solutions | Invited Lecturer, NOVA IMS, Lisbon | CISSP
rui.msoares@gmail.com

---

## Licence

[Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE)

You are free to share and adapt this material for any purpose, including commercial, provided you give appropriate credit.
