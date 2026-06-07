# Decentralized Trust Graph Working Group (DTGWG)

> A joint working group under [Trust Over IP (ToIP)](https://trustoverip.org) and the
> [Decentralized Identity Foundation (DIF)](https://identity.foundation), hosted within
> [LF Decentralized Trust](https://www.lfdecentralizedtrust.org).

---

## Table of Content
- [Latest Updates](#latest-updates)
- [About This Repository](#about-this-repository)
- [DTGWG Overview](#dtgwg-overview)
- [DTGWG Scope](#dtgwg-scope)
- [Task Force Repositories](#task-force-repositories)
- [LF Decentralized Trust Labs](#lf-decentralized-trust-lab-repositories)
- [How to Participate](#how-to-participate)
- [Licensing](#licensing)

---
## Latest Updates

| Date | Update | Document | Status | Notes |
|---|---|---|---|---|
| 2026-05-20 | Added draft baseline for the DTG hybrid interaction architecture, including architecture layers, core components, key interaction patterns, and status caveats for formal terms, implementation-specific elements, and emerging concepts. | [DTG Hybrid Interaction Architecture Baseline](architecture/dtg-hybrid-interaction-architecture-baseline.md) | Draft baseline v0.1 | Informative contributor-facing architecture document; not a DTG specification. |

## About This Repository

This is the umbrella repository for the Decentralized Trust Graph Working Group (DTGWG).
It is designed to serve as an entry point to our work and a guide to all our resources.

It links to the individual repositories maintained by each DTGWG Task Force, where corresponding 
topic-specific specifications, deliverables, and discussions live, as well as to the 
LF Decentralized Trust Labs that provide early-stage implementations of the DTGWG specifications.

Beyond navigation, the [discussions](https://github.com/trustoverip/dtgwg-general/discussions) in this umbrella repository acts as the "glue between the pieces" serving as the home for overarching conversations and developments that span task forces, such as architectural concepts, onboarding flows, or sociotechnical interactions and ceremonies that draw on and integrate deliverables from across the group.

[↑ Back to top](#decentralized-trust-graph-working-group-dtgwg)

---

## DTGWG Overview

The DTGWG develops the specifications, components, tooling, and governance components needed to build a decentralized trust graph (DTG) —
enabling proof of personhood, proof of agenthood, and the creation of verifiable trust relationships between people, devices, groups/communities/organizations of any type, and AI agents — all without requiring a centralized database.

Every party controls their own portable subgraph of the DTG through their own digital agents and wallets.

[↑ Back to top](#decentralized-trust-graph-working-group-dtgwg)

---

## DTGWG Scope

The DTGWG covers the full stack of specifications required for a functioning decentralized
trust graph, including:

- Key management and recovery
- Verifiable identifiers (e.g., decentralized identifiers) and verifiable credentials
- Verifiable relationship credentials and social vouching
- Verifiable membership credentials and verifiable trust communities
- Relationship cards (r-cards)
- Privacy-preserving zero-knowledge proofs
- Verifiable trust agents (VTAs) and rust task protocols
- Trust registries
- Out-of-band introductions
- UI/UX affordances for DTG wallets

The work is based open standards for decentralized identity and trust — principally
[W3C Decentralized Identifiers (DIDs) 1.0](https://www.w3.org/TR/did-core/) and
[W3C Verifiable Credentials Data Model 2.0](https://www.w3.org/TR/vc-data-model-2.0/).

It builds on
[*Design Principles for the ToIP Stack*](https://trustoverip.org/permalink/Design-Principles-for-the-ToIP-Stack-V1.0-2022-11-17.pdf),
the [*ToIP Technology Architecture Specification*](https://trustoverip.github.io/TechArch/),
other ToIP technical specifications, and complementary open standards for
decentralized digital trust infrastructure.

[↑ Back to top](#decentralized-trust-graph-working-group-dtgwg)

---

## Task Force Repositories

Each DTGWG Task Force operates its own repository. The following table shows the different
task forces with a short description and a link to the corresponding repository.

| Task Force | Focus Area | Repository |
|---|---|---|
| **Risk Assessment & Harms Prevention** | Analyses the overall requirements and potential harms for a successful decentralized trust graph, produces a risk assessment analysis and a recommendation on policies and best practices to prevent harms. | [dtgwg-rahp-tf](https://github.com/trustoverip/dtgwg-rahp-tf) |
| **Credentials** | Define the technical requirements for personhood credentials (PHCs) and verifiable relationship credential (VRCs), including credential formats, signature algorithms, zero-knowledge proofs, and revocation mechanisms. | [dtgwg-cred-tf](https://github.com/trustoverip/dtgwg-cred-tf) |
| **R-Cards** | Define the technical requirements for relationship card (r-card) interoperability and extensibility. | [dtgwg-rcards-tf](https://github.com/trustoverip/dtgwg-rcards-tf) |
| **Trust Task Protocols** | Define trust task protocols for standard DTG trust tasks, including QR codes, pairwise private DID exchange, PHC/VRC issuance and verification, r-card exchange, and personal private channels. | [dtgwg-trust-tasks-tf](https://github.com/trustoverip/dtgwg-trust-tasks-tf) |
| **Agent Names** | Define a syntax, resolution protocol, and service endpoints for URL strings that resolve to DIDs and DID documents for communicating with DTG verifiable trust agents (VTAs). | [dtgwg-agent-names-tf](https://github.com/trustoverip/dtgwg-agent-names-tf) |
| **DTG ZKP** | Define the ZKP requirements and designs necessary to make privacy-preserving proofs about DTG credentials | [dtg-zkp-tf](https://github.com/trustoverip/dtgwg-zkp-tf) |
| **DTG UX** | Define UX requirements and guidelines for sovereign wallets and standard user ceremonies for each of the primary trust tasks above. | [dtg-ux-tf](https://github.com/trustoverip/dtgwg-ux-tf) |


[↑ Back to top](#decentralized-trust-graph-working-group-dtgwg)

---

## LF Decentralized Trust Lab Repositories

LF Decentralized Trust Labs hosts open source reference implementations of DTGWG components in the following repos (which are also accessible via the GitHub [OpenVTC](https://github.com/OpenVTC) page).

| Lab Name | Description | Repository |
|---|---|---|
| **DTG Credentials** | Early implementation to the [DTG Credential specification v0.3](https://github.com/trustoverip/dtgwg-cred-tf). | [dtg-credentials](https://github.com/OpenVTC/dtg-credentials) |
| **OpenVTC** | Implements open standards and protocols to enable "Know Your Developer" capabilities, following the [*First Person Project white paper*](https://www.firstperson.network/white-paper) for establishing and verifying first-person trust relationships using Personhood Credentials (PHCs) and Verifiable Relationship Credentials (VRCs). | [openvtc](https://github.com/OpenVTC/openvtc) |
| **Verifiable Trust Infrastructure — Verifiable Trust Agent** | A Verifiable Trust Agent (VTA) is an always-on service that manages cryptographic keys, DIDs, and access-control policies for a Verifiable Trust Community. This repository contains the VTA service, a shared SDK, and the Community Network Manager (CNM) CLI. | [verifiable-trust-infrastructure](https://github.com/OpenVTC/verifiable-trust-infrastructure) |

[↑ Back to top](#decentralized-trust-graph-working-group-dtgwg)

---

## How to Participate

Since the DTGWG is a joint working group, participation in it or any of the DTGWG Task Forces is open through either ToIP or
DIF members:

1. Join either:
  1. [Trust Over IP](https://trustoverip.org/get-involved) as a member or observer.
  2. [Decentralized Identity Foundation](https://identity.foundation/join/) as a member.
4. Then, sign up for the [DTGWG mailing list](https://lists.lfdecentralizedtrust.org/g/toip-decen-trust-graph-wg)
   and accept the WG charter.
5. Attend a weekly working group call — details on the [DTGWG Confluence page](https://lf-toip.atlassian.net/wiki/spaces/HOME/pages/257785857/Decentralized+Trust+Graph+Working+Group).

[↑ Back to top](#decentralized-trust-graph-working-group-dtgwg)

---

## Licensing

- **Documentation/Copyright:** [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)
- **Patent mode:** W3C Mode (based on the W3C Patent Policy)
- **Source code:** Apache 2.0

Further information is available on the [DTGWG Confluence page](https://lf-toip.atlassian.net/wiki/spaces/HOME/pages/257785857/Decentralized+Trust+Graph+Working+Group).

[↑ Back to top](#decentralized-trust-graph-working-group-dtgwg)

---

*This repository is the umbrella index for DTGWG. Specifications and deliverables
live in the Task Force repositories and implementations in the LF Decentralized Trust Lab repositories 
both linked in the tables above.*

