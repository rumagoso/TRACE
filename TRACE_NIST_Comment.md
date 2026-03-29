# Public Comment: NCCoE Concept Paper
## Accelerating the Adoption of Software and AI Agent Identity and Authorization
### Submitted to: AI-Identity@nist.gov
### Submitted by: Rui Soares — rui.soares@crossjoin.pt
### Date: March 2026

---

## Submitter Background

Rui Soares is an Information Security and IT Governance professional with over 30 years of experience. He serves as ISMS Manager at Crossjoin Solutions (Almada, Portugal) and as an Invited Lecturer at NOVA IMS in Lisbon, where he teaches IT Governance, ITIL 4, and cybersecurity. He holds the CISSP certification and is an active contributor to the Cloud Security Alliance, including AI Controls Matrix review processes. He is the author of the TRACE proposal referenced in this submission and the developer of the WBSC (Worldview Belief System Card) framework for AI transparency, published through CSA.

---

## Summary

This comment responds to the NCCoE's request for input on the concept paper "Accelerating the Adoption of Software and AI Agent Identity and Authorization." It identifies a critical scope gap in the current framing and proposes a concrete reference architecture — TRACE — to address it.

The core observation: the concept paper applies existing enterprise IAM standards (OAuth 2.0, SPIFFE/SPIRE, OpenID Connect) to agents operating within known organisational boundaries. This is necessary and valuable. It does not address the problem that will define the next phase of agentic AI deployment: **agents crossing organisational boundaries with no shared registry, no cross-jurisdictional accountability chain, and no economic consequence for failure.**

The NCCoE concept paper explicitly defers this scope. This comment argues it should be the primary focus of the next iteration — and proposes TRACE as a reference architecture for that work.

---

## 1. The Scope Gap

The concept paper's stated scope covers agents operating within enterprise environments, applying existing identity standards to internal agentic architectures. This is the right starting point.

However, the accountability failure modes that are already materialising — agent impersonation across organisational boundaries, rogue delegation chains crossing jurisdictions, incident investigations with no recoverable chain of custody — are precisely the scenarios that enterprise IAM cannot address, because they involve agents operating outside the deploying organisation's identity perimeter.

Current standards under consideration by NCCoE — OAuth 2.0, SPIFFE/SPIRE, OpenID Connect — were designed for authenticated principals operating within known trust boundaries. An AI agent that spawns a sub-agent that delegates to a third agent in a different jurisdiction has exited those boundaries entirely. No existing standard provides a cross-organisational, cross-jurisdictional answer to the question: "Who are you, who sent you, and what are you authorised to do?"

This gap is not theoretical. Amazon's November 2025 lawsuit against Perplexity — alleging covert agent activity across organisational boundaries — is an early example of the litigation that will proliferate as agents operate at scale without verifiable identity infrastructure.

---

## 2. TRACE: A Reference Architecture Proposal

The submitter has developed TRACE — Trusted Registry for Autonomous and Connected Entities — as a proposed open infrastructure standard specifically designed to address the cross-boundary identity and accountability gap.

TRACE operates across four layers:

**Layer 1 — Identity.** Every AI agent must register before operating in a TRACE-compliant environment. A cryptographic identity — bound to hardware (TPM, vTPM, HSM) where possible, to a verified legal entity where not — is recorded on a permissioned distributed ledger using W3C-compliant Decentralised Identifiers (DIDs). Recursive Sub-Tokens enable high-velocity delegation without requiring a ledger write for every micro-task, while maintaining the chain of custody. A sub-agent's scope is always a strict subset of its parent's registered authorisation.

**Layer 2 — Access.** Resources query TRACE before granting access to any agent. Registered and in good standing: access at the appropriate trust tier. Unregistered: no access, without exception. This gate operates across organisational and jurisdictional boundaries — not only within enterprise perimeters.

**Layer 3 — Governance.** The TRACE Foundation — a multi-stakeholder non-profit modelled on ICANN's governance architecture — governs the registry at two speeds: automated Circuit Breakers for real-time threat containment (24-hour technical suspension triggered by anomaly detection) and human supermajority for permanent revocation. Regulatory observers hold read access and incident notification rights.

**Layer 4 — Economic Alignment.** Agents operating at high-risk tiers must post conditional collateral — financial stakes held in escrow against verified failures. On confirmed failure, collateral is released to a victim recourse pool. High-tier agents with clean records receive tiered infrastructure incentives. This layer creates economic skin in the game — making accountability financially consequential, not just technically specified.

---

## 3. Specific Responses to NCCoE Questions

**On identification:** Agent identities should be fixed at registration, not ephemeral. Ephemeral task-specific identities are appropriate for sub-agent tokens (TRACE's Recursive Sub-Tokens), but the root identity must be persistent, cryptographically bound to a legal entity, and publicly auditable. The distinction matters: fixed root identity enables accountability; ephemeral sub-tokens enable performance.

**On authentication:** Strong authentication for AI agents requires hardware binding (TPM/HSM) where agents operate on known infrastructure, and legal entity verification where they do not. vTPM support is essential for cloud-native deployments where agents migrate across environments.

**On cross-boundary scenarios:** The concept paper explicitly defers agents from untrusted external sources. TRACE proposes this should be the primary focus of the next project phase. The enterprise-internal problem is solvable with existing IAM. The cross-boundary problem is not — and it is the more consequential one.

**On the economic layer:** Existing identity frameworks have no mechanism for financial accountability. TRACE's Layer 4 proposes conditional collateral as a pre-condition for high-risk agent operation. This aligns with insurance and bonding frameworks used in other high-risk professional contexts and provides regulators with an enforcement lever that does not require new legislation.

**On standards coordination:** TRACE is designed to be complementary to, not competitive with, the standards under NCCoE consideration. It adopts W3C DID as its identifier format, is compatible with OAuth 2.0 delegation flows for enterprise-internal sub-agent tokens, and maps to NIST SP 800-63-4 for identity assurance levels. The proposed EBSI (European Blockchain Services Infrastructure) ledger for the EU context is architecture-equivalent to permissioned alternatives suitable for US deployment.

---

## 4. Recommendation

The NCCoE demonstration project scoped in the concept paper — applying existing IAM standards to enterprise-internal agents — is a necessary and valuable first step. This comment recommends that the subsequent project phase explicitly address:

1. Cross-organisational agent identity — a shared registry architecture for agents operating across enterprise boundaries.
2. Cross-jurisdictional accountability — how identity and accountability chains are maintained when agents cross regulatory jurisdictions.
3. Economic accountability mechanisms — how financial consequences are attached to agent failures at scale.

TRACE is offered as a reference architecture for that second phase. The full position paper is available at: https://www.linkedin.com/pulse/registry-ai-agents-problem-rui-soares-bcyye/ or upon request at rui.soares@crossjoin.pt.

---

## 5. Conclusion

The NCCoE concept paper correctly identifies agent identity and authorisation as a foundational challenge. The standards under consideration address the enterprise-internal dimension well. The cross-boundary dimension — where the most consequential failure modes live — remains unaddressed by any current initiative.

NIST is in a position to define the infrastructure standard that closes this gap before the failures make it unavoidable. TRACE is a concrete, technically grounded proposal for what that infrastructure could look like.

The submitter welcomes direct engagement and is available to present the TRACE proposal in greater detail at CAISI listening sessions or working group convenings.

---

*Rui Soares*
*ISMS Manager, Crossjoin Solutions*
*Invited Lecturer, NOVA IMS, Lisbon*
*CISSP | ISO 27001 | NIS2 Practitioner*
*rui.soares@crossjoin.pt*
