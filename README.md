# TRACE — Trusted Registry for Autonomous and Connected Entities

**A proposed open infrastructure standard for verifiable AI agent identity, authorization, and accountability across organizational and jurisdictional boundaries.**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**Version 0.3** — June 2026 (Expanded Integrations)  
**Author**: Rui Soares  
ISMS Manager, Crossjoin Solutions | Invited Lecturer, NOVA IMS, Lisbon | CISSP

---

## 📋 Table of Contents

- [Executive Summary](#executive-summary)
- [The Problem](#the-problem)
- [What is TRACE?](#what-is-trace)
- [Integrations and Interoperability](#integrations-and-interoperability)
- [Standards Alignment](#standards-alignment)
- [Status & Roadmap](#status--roadmap)
- [Call to Action](#call-to-action)
- [License](#license)

---

## Executive Summary

AI agents are increasingly acting autonomously across borders — booking meetings, executing transactions, controlling systems, and spawning sub-agents. Without shared infrastructure for identity and accountability, this creates serious risks.

**TRACE** (Trusted Registry for Autonomous and Connected Entities) provides a practical, layered, open standard to answer the fundamental questions:

> **Who are you? Who sent you? What are you authorised to do?**

**v0.3** significantly strengthens the proposal with explicit mappings to **C2PA**, **OpenTelemetry**, **Estonia’s AI ID initiative**, and **China’s CAC rules**, positioning TRACE as the unifying identity backbone for agentic AI.

---

## The Problem

Enterprise IAM tools (OAuth 2.0, SPIFFE, OpenID Connect) work well *inside* organizational boundaries but were never designed for agents operating across them. This gap enables spoofing, unaccountable delegation chains, and difficulty in incident response.

This is no longer theoretical — it is an active challenge in 2026.

---

## What is TRACE?

TRACE is a **four-layer open infrastructure**:

| Layer              | Purpose                                                                 | Key Mechanisms |
|--------------------|-------------------------------------------------------------------------|----------------|
| **1. Identity**    | Persistent, verifiable agent identity tied to legal entities            | W3C DIDs on permissioned ledger + Recursive Sub-Tokens |
| **2. Access**      | Real-time authorization at resource boundaries                          | Registry queries + Scoped permissions |
| **3. Governance**  | Oversight, rapid response, and long-term stewardship                    | ICANN-style Foundation + Automated Circuit Breakers |
| **4. Economic Alignment** | Skin-in-the-game and positive incentives                              | Conditional collateral/escrow + reputation tiers |

TRACE is **complementary** — it augments existing standards rather than replacing them.

---

## Integrations and Interoperability

TRACE is designed to work seamlessly with leading tools and regulations. See the full details in:

→ **[TRACE_Position_Paper_v0.3.pdf](https://github.com/rumagoso/TRACE/blob/main/TRACE_Position_Paper_v0.3.pdf)**

**Key Integrations**:

- **C2PA / Content Credentials**: TRACE DIDs serve as authoritative signers for manifests, adding persistent identity and revocation.
- **OpenTelemetry**: Enrich agent traces with TRACE identity for end-to-end observability and governance.
- **Estonia AI IDs** (June 2026): Direct mapping for national-to-global scaling.
- **China CAC Rules**: Enables compliant labeling and cross-border enforcement.

These mappings close critical gaps in provenance, observability, and regulatory compliance.

---

## Standards Alignment

TRACE aligns with and supports:
- W3C DID Core, OAuth 2.0
- NIST AI RMF & SP 800-63
- ISO/IEC 42001, EU AI Act, NIS2
- **C2PA**, **OpenTelemetry GenAI**
- Estonia AI ID initiative, China CAC labeling rules
- EBSI and other digital identity frameworks

---

## Status & Roadmap

| Milestone                        | Status                  | Date          |
|----------------------------------|-------------------------|---------------|
| Position Paper v0.3 (Integrations) | Draft                  | June 2026    |
| Position Paper v0.2              | Published              | March 2026   |
| NIST NCCoE Submission            | Submitted              | March 2026   |
| CSA Blog Submission              | Pending                | —            |
| Working Group Formation          | Open                   | Now          |
| Reference Implementation / PoCs  | Planned                | Q3–Q4 2026   |

---

## Call to Action

We invite collaboration from:

- Standards bodies (C2PA, OpenTelemetry, ISO, NIST)
- Governments & regulators (Estonia, EU, China, etc.)
- AI framework developers (LangGraph, AutoGen, CrewAI, etc.)
- Security & identity experts

**How to contribute**:
1. ⭐ Star the repo
2. Review and comment on the [Position Paper](https://github.com/rumagoso/TRACE/blob/main/TRACE_Position_Paper_v0.3.pdf)
3. Join the working group (open expression of interest)
4. Propose or build PoCs with C2PA, OTel, or national ID integrations

---

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

---

**Repository**: [https://github.com/rumagoso/TRACE](https://github.com/rumagoso/TRACE)

*Last updated: June 2026*
