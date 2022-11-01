# ECP-3: Empowering the Community and Building a Sustainable Treasury

## ⚠ Work in Progress - Live & Changing Document

**Author:** LPX, Evmos DAO Governance Council 

**Summary**: The funding of this proposal (Phase 2) will mark the beginning of a new era for the Evmos network. 

The Governance Council is requesting Xmil EVMOS (\~N% of the Community Pool) to initiate the DAO’s Treasury with the goals of being a self-sustainable, self-funded DAO within the next year.

**Abstract:** The funding of the DAO’s treasury will allow the DAO and its contributors to take calculated and aggressive moves to bootstrap the Evmos ecosystem while paving the path for a brighter future. 

 - Quick and effective deployment of incentive programs and project/partner onboarding initiatives
 - Alignment of incentives and off-chain governance 
 - Community-governed incentives program
 - Utilization of both novel and tried-and-true strategies in an ongoing effort to make Evmos DAO a self-sustainable entity


## Motivation 

As over 108mil tokens sit idly in the Community Pool, the DAO wishes to utilize a relatively small portion in its continued efforts to advance the Evmos ecosystem. As the main driving force in community-led growth of Evmos, we hope that the Community is able to see our vision in what is possible with a workable treasury.  

Our long term vision for Evmos DAO is to be fully decentralized and governed autonomously by the community. But getting to that ideal vision of a “true” DAO while maintaining effective governance is not a simple task nor is there a cookie-cut method to follow. DAOs are still in the very early days of trying to figure out which mechanisms and processes work best — even the most seemingly established and respected DAOs are constantly iterating their governance process.

For example, Uniswap (est. 2018) is known for singlehandedly propelling the world of DeFi with their concept of liquidity pools. They boast the world’s largest treasury worth nearly $3bil, and yet growth and innovation was not meeting their expectations. Just a few months ago Uniswap governance passed a landmark proposal to create the “Uniswap Foundation” with a funding of $75mil. The foundation wanted  “to reduce governance friction at Uniswap for high-impact and high-value projects and improve navigation in the ecosystem.” 

The realization that a strict, rigid governance can be a huge impediment for effective off-chain decision making and the execution of projects and initiatives is spreading through the Ethereum ecosystem like wildfire. In just the past three months, the following notable DAOs have formed their own versions of their foundation for the purpose of reducing friction in their ability to be effective: Rarible DAO, Pool Together DAO, TrueFi DAO, Synapse DAO, Developer DAO, Bancor DAO, Balancer DAO, and a handful more (it should be noted that the term “Foundation” in these aforementioned DAOs have a different connotation from the Evmos “Foundation”).

This is a phenomenon that Evmos DAO will closely be monitoring, as we strive to continuously improve and are always on the lookout for developments in more effective governance. However, this new trend gives us a boost of confidence that forming a DAO Treasury separate from the Community Pool is not only the right move, but a smart move. 


---


## DAO Treasury Specifications

**Prerequisites**: Accountability within a DAO is all about setting and holding contributors and governance participants to a common expectation aligned to the DAO’s mission, values and goals. The same principles should apply to treasury management and spending processes. 

The specifications of the Evmos DAO Treasury is designed with the following accountability measures in place:

 1. Safe, upgradeable contracts managed by trusted multi-signatories
 2. Transparency and clarity on all spending via off-chain proposals with timelock
 3. The delegation of responsibilities to workstream leaders within the DAO
 4. Secondary contracts for risk management (vested token releases, payment streaming, payment splitting)


**Main Multisig Specifications:** The main treasury will be a Gnosis Safe deployment, the most battle-tested multisig contract on Ethereum. Its n-of-m configuration will start as 4-of-7 on Evmos mainnet. Both parameters n and m may evolve and are ultimately defined by DAO members and the Evmos Community with security in mind.

Safe Audits: [(External Link)](https://github.com/safe-global/safe-contracts/tree/v1.3.0/docs)

The multisig will initially be composed of Governance Council Directors and trusted ecosystem members or validators (in the case that we are not able to fill all 7 slots). A shortlist of backup signers will be maintained in the case that a signatory must be removed or is no longer capable of fulfilling his or her duty.  

Safe Deployment Address (Evmos Mainnet): `0x3E5c63644E683549055b9Be8653de26E0B4CD36E`
Evmos DAO Treasury Deployment:  `TBD` 

---

**Flow of Funds (Simplified)**

The main treasury's main role is to enact and execute on-chain transfer of funds as decided by DAO participants via off-chain voting. It should be noted that the Governance Council will initially request funds for planned projects and will likely propose many more in the long term. 

![Example Diagram](https://i.imgur.com/SaUGC2q.png)

The eventual goal of the DAO treasury is to be fully community owned. This process of handing off the keys to the treasury can not happen, however, until the DAO's off-chain governance is well-matured and protected against potential bad actors. Progressive decentralization is a guiding value that we have pledged to in our Constitution, and we encourage the Community to keep us accountable. 

**Off-Chain Proposals**

For funding requests that are under the domain of the DAO's treasury, a GovernorAlpha contract — or a suitable alternative — will be deployed. 

The proposal lifecycle of Governor contracts are relatively simple and offer the security of a mandatory timelock in which a malicious attempt can be veto'd.

![](https://i.imgur.com/Z1ul6WS.png)

Fund distribution methods may differ from workstreams and special projects. For example, recipients may opt to utilize friendlier tools like Colony or Coordinape if they wish to do so. 

For large funding requests or funding that is out of the scope of the DAO's programs, a formal on-chain proposal must be made to receive funding from the *Community Pool*.


## Road to Self-Sustainability & Decentralization Initiatives

For the past half-year, Evmos DAO contributors have been proudly serving the Community. We hope that our previous efforts are recognized by the Community and is a testament to our genuine dedication to the advancement of the Evmos ecosystem and network. 

The target operational, development, and incentives runway with this funding request is **one year**; however, we hope to extend that runway as much as possible through various programs. On the other hand, the absolute best case scenario for the DAO would be to achieve self-sustainability by late next year. 

| # | Initiative | Description | Allocation  | 
| - | ---------- | ---------- | -------- |
| 1 | Workstream (SubDAO) Funding | Compensation of current and future workstream members and the funding of workstream initiatives. | 20%     |
| 2 | GOV Tokenomics & Community Gauges | The $GOV token and the gauge system is designed to decentralize Liquidity Incentives allocation, promote long-term alignments, and facilitate off-chain governance voting. | 12.5%     |
| 3 | Boosted Liquidity Vaults & veGOV | The funding of the new proposed liquidity incentives programs that is community-led, more transparent, DEX-agnostic, and shared benefits. | 22.5%     |
| 4 | Perpetual Bounty Fund & deGOV | The funding of the new proposed liquidity incentives programs that is community-led, more transparent, and is DEX-agnostic. | 10%     | 
| 5 | Treasury Growth & yGOV | Initial funding for DeFi revenue generation strategies and yield-bearing GOV tokens | 7.5%     |
| 6 | Treasury Bonds | Building community-owned liquidity through the sales of treasury issued bonds. | 5%     |
| 7 | Strategic Reserves | The reserves will be used only when strategic opportunities are presented to the DAO or rebalancing of the treasury is necessary. In particular, DAO2DAO token-stable swaps will be sought after to diversify our assets into stablecoins without creating market sell pressure.   | 20%     |

- All remaining funds that are not immediately needed will be considered as strategic reserves and remain in the main treasury until ready for deployment (i.e. while we wait for new workstreams to be established, deployment of contracts, etc.).

---

## GOVMOS ($GOV) Utility & Tokenomics

The GOV token will be the main driver of our off-chain governance, incentive alignments, long-term sustainability, and decentralization efforts. A combination of tried and true strategies as well as novel implementations in DeFi and smart contracting will be utilized. Heavy inspiration is drawn from well-established and successful DAOs that have pioneered the way in governance philosophies and decentralized finance and economics: MakerDAO, Compound, Curve, Yearn, Gnosis, 1Hive, Uniswap, Sushi, Aave, ShapeShift, Balancer, MolochDAO, and many more.

### GOV: Evmos DAO Governance Base Token Layer

Alignment between the Evmos DAO governance token (GOVMOS, or GOV for short) holders and protocol stakeholders (EVMOS) is crucial for an *efficient* decentralized governance -- GOV tokens are the vehicle to drive this alignment. GOV tokens are not a financial investment, although there will be economic benefits. GOV token holders are typically DAO contributors and Evmos Community members who are committed to seeing the continued growth of the Evmos ecosystem, and want a seat at the governance table.

Optimizing for the right people to participate in governance processes is an ever-evolving discussion in governance circles. It may not be pragmatic to assume that all voters should participate in every governance decision. Participating in governance is a lot of work — reading and digesting a proposal, providing feedback for discussion and voting on every matter can be mentally fatiguing. In addition, many do not have the subject matter expertise or desire to participate in proposals outside of their domain.

This approach is not to be a gatekeeper of decisions - anyone who wishes will be able to participate. The key difference between on-chain proposals and off-chain DAO proposals is that DAO governance is *voluntary*. 

$GOV will be launched as an ERC20 with a 1:1 EVMOS backing. In simpler terms, depositing one EVMOS token will mint you one GOV token; reciprocally, returning one GOV token will release one EVMOS token. GOV tokens are transferrable, fungible, and tradeable. GOV serves as the base layer token for the many functions of its derivatives. **Holding GOV tokens do not grant any voting power.**

**Important concept to remember:** `$GOVMOS` is essentially `$WEVMOS` but with expanded feature sets that allow the DAO and community participants to create and govern the following derivatives and programs. 

### GOV Derivatives Overview

![](https://i.imgur.com/WN7f8LC.png)


### veGOV: Aligned & Incentivized Decentralized Decision Making

Participating in Evmos DAO governance requires that a wallet have a balance of vote-escrowed GOV (veGOV). veGOV is a non-standard ERC20 implementation, popularized and battle tested by DAOs on Ethereum, that determines each wallet's voting power.

veGOV is obtained by depositing and locking GOV into the DAO's escrow contract. The maximum lock time is two years, and the minimum one month. 

The amount of veGOV received is proportional to the lock-time selected - locking 100 GOV for the maximum two year period will return 100 veGOV. A one year lock of 100 GOV would return 50 veGOV, and so forth. 

Once veGOV is issued to a wallet the tokens will automatically begin decaying at a 1/2 slope linear rate until the time-lock period is reached. For example, if 500 veGOV tokens were rewarded at the time of deposit, 250 veGOV would remain at the time when the vesting period is complete and the original GOV tokens are available for withdrawal. 

Users may decide to keep the original GOV tokens vested even after the completion date in order to retain the remaining veGOV. However, as soon as the original GOV tokens are claimed back into the originating wallet, the remaining veGOV will burn itself.

The vote-escrowed approach plays several crucial roles in the DAO's governance and our long term goals:

1) Significantly reduces sybil and other attack vectors in off-chain governance proposals
2) Ensures that participants are aligned with the long-term goals of the DAO and our vision
3) Incentivizes governance participation with boosted yields
4) Will be the main driver of the Liquidity Incentives Program 2.0 with community governed incentives allocation and DEX-agnostic TVL growth
5) Generates recurring revenue and treasury diversification through DAO-owned liquidity

**Liquidity Gauges**: A pre-determined amount of EVMOS tokens will be allocated towards Liquidity Incentives each month. veGOV weight from community participants will ultimately dictate the allocation of incentives for each liquidity pool. 

Through the gauge system we are able to run our liquidity incentives program perpetually and in a much more decentralized, fair, and community-centric method. 

**Multi-Token Liquidity Mining**: Each pool's Gauge contract can distribute up to 5 different kinds of tokens. This allows for multiple partners/protocols/DAOs to incentivize a given pool by adding their own tokens. 

The goal of the Liquidity Guages is to be as permissionless and community-governed as possible. However, the Governance Council may blacklist tokens from being able to be deposited as an incentivization token to combat spam.

**Liquidity Vaults (Lockers)**: DAO-owned liquidity vaults (farms) will be deployed to maintain our stance of neutrality and allow the natural growth and healthy competition between DEXs and DeFi protocols. 

In an effort to facilitate the steady growth of Evmos' TVL and liquidity, incentives will be boosted for those who commit to a bonding period when depositing their LP tokens. Auto-compounding contracts will also be deployed and utilized to maximize the yield for depositors.

![](https://i.imgur.com/KcoDXpG.png)

**Current Problem**: While Prop 64 provided the Evmos network the much needed native liquidity, the proposal was not designed to be a long-term solution. The TVL that has been built is held hostage by the high farming APRs provided at the expense of the Community Pool. The lack of any lockup mechanism also encourages "pool hopping" leading to potentially volatile liquidity and subsequently volatile price movements.

![](https://i.imgur.com/4ScBYt4.png)

 
### deGOV: Governance Rewards for Network Decentralization Assistance

Delegated GOV tokens, or deGOV are similar to veGOV in that they hold voting weight. However, while veGOV is deflationary once received, deGOV gains voting weight the longer they are staked with the DAO. deGOV tokens are minted at a 1:2 ratio, meaning a 10 GOV deposit will return 5 deGOV.

deGOV does not have a maximum time-lock period, but will stop accruing voting power at 24 months, with a voting weight boost of 2x of the original deposit. The minimum bonding time is one month,

**The Perpetual Bounty Fund**

deGOV will play a key role in the maintaining the sustainability of the Community Perpetual Bounty Fund. The concept of the Perpetual Bounty Fund straightforward - the DAO participates in network staking for the purpose of creating a self-replenishing fund for bounties, contributor payments, and special initiatives. 

- The authz module is utilized to re-stake “maintenance” token amounts to offset the daily changing APR.
- A portion of the daily rewards (TBD) are sent to a claiming contract in which deGOV holders may wish to claim their share of the staking rewards.
- The remainder of the rewards are claimed and sent back into a DAO treasury wallet used for bounties and funding initiatives. 
- If the bounty fund's growth is far exceeding the pace of outbound funds, the DAO may choose to re-route the funds to another program or into the Strategic Reserve fund.

Bounties can range from internal growth initiatives to external outreach campaigns. An internal growth example would be to bounty out a SourceCred deployment on Evmos to incentivize participation in governance, encourage constructive discussions, nurture a culture of helping others, etc. The potential bounties and programs can also act as an assistance tool for the core devs by contributing in areas like the improvement and expansion of the Evmos documentation. 

As we eagerly wait for our community to grow and have leaders step up in the creation of new workstreams, bounties are an excellent tool to not only lighten the already heavy workload, but to attract talent, long-term contributors, and future leaders.

**Delegation Gauges**: Similar to Liquidity Gauges, the community will have the power to decide the allocation amounts for 75% of the delegateable tokens from the Perpetual Bounty Fund. The Governance Council, although unlikely to happen often, reserves the right to decide the monthly delegation amounts of the remaining 25%.

The Perpetual Bounty Fund is restricted from delegating to any validator in the top 25 by VP, calculated at the last day of each month. Any votes towards the top 25 validators will be disregarded and allocations distributed proportionately to the eligible validators.  

### yGOV: Yield Bearing Single-Sided Staking Rebase Tokens

Yield bearing GOV (or yGOV) are obtained by depositing GOV into an escrow contract controlled by the DAO. **yGOV does not have any voting weight.**

yGOV is a rebasing token that is redeemable 1:1 with GOV. EVMOS tokens that are represented by the deposited GOV will be deployed into the network's DeFi ecosystem to generate optimized yields. The rebasing occurs shortly after every Evmos epoch and the yields are transferred directly to the users. This allows the constant accural of yields without the need for any action from the end user. 

The redemption (unbonding) time for yGOV is 15 days. Instant withdrawals may be possible depending on the reserve liquidity available at that the time, but will incur a harsh 25% penalty fee. 

![](https://i.imgur.com/R48AOko.png)


**Liquidity Reserve**: A small reserve liquidity for the yGOV<>GOV swap contract will be maintained for those who are in an emergency and willing to incur the penalty fee.

**yvGOV (Yield-Bearing Vested GOV)** is another GOV deriviative that is being researched. yvGOV will be a vested version of yGOV, with similar characteristics of veGOV. 

## Treasury Bonds Market

Protocol owned liquidity (POL) is an important topic that is constantly brought up as one of the most important aspects of growing a healthy treasury. While POL is mostly used in the context of DeFi protocols' and product/service DAOs' treasuries, Evmos DAO is unique in that we are serving a community of an entire Layer-1 Blockchain. Thus, we feel justified in using the term "Community Owned Liquidity." Just as we defend the integrity of the Evmos Constitution and our Governance System, we must fight to defend the value of our network. 



**Benefits of Community Owned Liquidity**

- Diversification of Assets
- Revenue Generation from Swap Fees
- Long-term Aligned Ecosystem Growth
- Stable Network-Wide Liquidity