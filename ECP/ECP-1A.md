# ECP-1A: Formalizing the Evmos Community Proposal Framework

**Author:** LPX, Evmos DAO Governance Council

**Summary**: This proposal seeks to formalize the adoption of the Evmos Community Proposal (ECP) framework. All community proposals must go through the proposal lifecycle as outlined in the framework before going on-chain for voting. This document is a condensed version of the ECP Framework; for the full length version refer to the [Governance Documentation.](https://gov.evmos.community/governance/proposals)

**Abstract:** ECPs are standardized proposals subject to voting that (once enacted) regulate and define the behavior of the Evmos DAO's Governance system, and provides a funding mechanism for special projects and workstreams.

The Evmos Community Proposal (ECP) Framework sets the guideline for all subsequent ECPs to follow. This ECP is the foundational ECP that provides the necessary templates, processes, and guidelines for working within the framework and defines the key roles required for the operation and enforcement of the ECP process.

**Motivation:** The proposal lifecycle is designed to have technical, human, and procedural elements for a self-sustainable governance that holds the entire Evmos Community accountable for the continued growth of the ecosystem. The Governance Workstream and the Community has been self-regulating and informally enforcing the general guidelines posted in [“Best Practices”](https://commonwealth.im/evmos/discussion/6022-passing-a-community-proposal-best-practices) — however, as we prepare to expand the scope and responsibilities of Evmos DAO, we must prepare for another influx of proposals by providing clear guidelines and proposal standardization. 

We strongly believe that our governance participation is among the highest in the blockchain space because of our continued efforts in building a culture of open discussion, strong due diligence, helping one another, and our willingness to assist newcomers navigate the waters of governance. While I am confident that our Community will continue building great culture, a standardized proposal framework and clear lifecycle guideline will ensure that our governance continues on this path for the long-term.

---

# ECP Framework Components

## 1. Definitions of the ECP Framework

### Proposal Types

**On-Chain Governance**

On-chain governance refers to all protocol level execution of proposals using Cosmos SDK's `gov` module. Anyone who holds or stakes EVMOS can participate in these votes and takes precedence over the delegated validators of the voter. 


**Off-Chain Governance**

Off-chain governance refers to all community decisions that do not require an on-chain protocol-level change. These types of decisions include a wide variety of topics and concepts, from passing meta-governance proposals to the formation of special task forces or workstreams. 

### Proposal Types by Category

 - Protocol Proposals
 - Community Proposals
 - Meta-Governance Proposals
 - Workstreams & Special Initiatives
 - Community Grants & Funding
 - Protocol Incentives & Evmos Specific Proposals
 - Network Upgrades and Security

Refer to the [Governance Documentation](https://gov.evmos.community/governance/proposals/definitions) for more details.


## 2. The ECP Lifecycle

![](https://i.imgur.com/D8IcfJS.png)

**Phase 1: Discussion & Ideation | Min. 48 hours | Forum Tag: \[IDEATION\]**

The purpose of this phase is to vet ideas with the active Evmos community members. Each idea for a proposal should have its own Commonwealth thread, and discussions should be as narrowly focused as possible. 

Anyone can participate and is encouraged to provide feedback in this phase of governance. The goal of Phase 1 discussion is to gain a rough community consensus, and refine the idea so that it can be formalized. The thread author should make an effort to address all comments and take them into consideration.

**Phase 2: ECP Formalization | Min. 72 hours | Forum Tag: \[PRE-PROPOSAL\]**

Phase 2 is where the idea is formalized into an Evmos Community Proposal and includes all of the criteria specified in the ECP Framework. It must be a clear and complete description of the discussions and ideas held in the previous phase. 

**Phase 3: ECP Signaling (Temp. Check) | Min. 72 hours | Forum Tag: \[PROPOSAL\]**

The author may finalize the ECP by initiating a community temperature check. To do this, the author must add a poll within the thread to gauge the community sentiment.

Proposals should only move to Phase 3 once the author has considered all community comments, responded to all concerns and questions, and believes that the proposal is ready to go on-chain for a final network-wide vote. Proposals in Phase 3 should not be edited further with the exception of minor mistakes. 

**Phase 4: On-Chain Voting | Forum Tag: \[VOTING\]**

If the signaling polls in Phase 3 show an overall positive sentiment and no major issues are brought up, the proposal may be submitted on-chain for the formal voting. Submission guidelines [are listed here.](https://gov.evmos.community/governance/proposals/submission)

![](https://i.imgur.com/tI2JRp6.png)


### Exceptions to the Framework

**Governance Council**

The Evmos DAO Governance Council may "fast-track" a proposal onto on-chain voting for time-sensitive and urgent matters. The Council must be prepared to explain to the community regarding the decision. If the community deems that the decision was made in bad faith, the Community is encouraged to engage in discussions and hold the responsible parties accountable through disciplinary actions or in extreme cases the removal of a Council member through an on-chain vote.

**Core Developers**

Core developers are not bound to the ECP Framework for network and protocol related proposals. It is expected, however, that thorough testing and due diligence is performed by the developers for all network upgrades. It should be noted, however, that network upgrades must still go through the process of on-chain voting.


## 3. ECP Standards and Templates

### Standardized Proposal Templates

The Evmos Governance Framework allows for various different types of proposals, both on-chain and off-chain. All proposals must include the core components of the template. Depending on the proposal type, additional components may be required. 

Some proposal templates can be found in the [Governance Documentation.](https://gov.evmos.community/governance/proposals/templates) The Governance Council currently plans to improve the template system through a guided proposal creation dashboard.

## 4. ECP Submission Guidelines

Submission guidelines and tips can be found in the [Governance Documentation](https://gov.evmos.community/governance/proposals/submission) as well as the official [Developers Documentation](https://evmos.dev).

Proposals that have not followed the guidelines will most likely be rejected by the Community. If a proposal is made in bad faith, the Community is encouraged to vote `No with Veto`.

We strongly encourage all proposers to first submit it on testnet to check the formatting and deposit amount. Do not hesitate to reach out to a Governance Council member for review.