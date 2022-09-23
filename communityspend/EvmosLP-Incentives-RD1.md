---
title: Launching the Evmos Liquidity Incentives Program
authors: Tricky, Benny Lava, LPX
proposal: ECP-PS-1
type: CommunityPoolSpend
discussion: https://commonwealth.im/evmos/discussion/6977-prevote-kickstart-defi-on-evmos
polls: https://bafybeieyr4vsc3gubivurtvvuunhmkl3uqvsuv3zuag34gnh3xzgdyzcpe.ipfs.w3s.link/polls.json
govreviewed: true

---

# Launching the Evmos Liquidity Incentives Program

## **Summary** 

This proposal will kickstart the Evmos Liquidity Incentives Program with the bootstrapping of liquidity pools on the Diffusion DEX. More initiatives are in the works with other DeFi projects, and will be proposed when ready. 

## **Motivation** 

The Evmos blockchain is a superior environment for DeFi, but it has had its fair share of roadblocks that have slowed down and limited growth in the Evmos ecosystem. We have also had very attractive staking APR that gave a higher return than most liquidity pools, and a bridge exploit that destroyed the TVL of Evmos DeFi in a matter of hours.

Despite the hurdles, we are confident in saying that we had great success with our incentivization initiative for the EVMOS/OSMO pool through Prop 39 which provided 600,000 EVMOS tokens for external incentives over 90 days on the Osmosis DEX. Since then, EVMOS has become one of the most popular pools on Osmosis in nearly all areas including TVL, volume, and daily APRs. At the time of writing, the pool has grown from just $2M, now to the 5th largest pool on osmosis with a TVL of $9.8M and one of the highest volume pools of over $3M. The incentives that helped drive this success will be expiring soon, and while we do plan on extending the Osmosis program, we must also begin looking inward: our native TVL.

## **Strategy** 

As more EVMOS tokens are staked, the APR rates have been decreasing at an accellerated rate. Millions of tokens are being unbonded at this moment, and without alternative pools with very appealing rates, they will most likely be going to Osmosis to be sold. Our first priority is to 1) build the much needed liquidity to wean off our reliance on Osmosis pools for liquid markets; 2) attract fellow IBC friends to participate in our high rewards programs and attract the unbonding Evmos tokens to find its way into these incentivized pools.  

The Community Treasury is currently sitting around 33mil EVMOS tokens with 75mil+ EVMOS tokens returning from the unclaimed airdrops, and with an usage incentives escrow wallet which is now nearing 35mil tokens. 

In total, roughly 143mil EVMOS (~$357mil @ $2.5), is left sitting with no benefits, when they can be put to strategic use that not only encourages more network participants, but also brings the community rewards for helping with the bootstrap initiative. 

In summary, this is an aggressive but needed first step in further growing the Evmos network. Liam from Evmos explains eloquently in [this comment](https://commonwealth.im/evmos/discussion/6977-prevote-kickstart-defi-on-evmos?comment=30063) why this proposal is so important. We highly suggest reading it if you are unsure or on the fence.

## **Plan of Action**

Diffusion will be the first DEX to receive incentives, as they have been the leading DEX prior to the Nomad exploit. More protocols and DeFi projects will follow, with programs of their own. 

Diffusion will continue with their DIFF rewards for existing pools, resulting in *double rewards* for the pools that will be incentivized further with Evmos tokens.

2mil EVMOS tokens will be released into a Gnosis Safe (3/5 signatures). Over the course of 180 days, the allocated EVMOS rewards will be released into Diffusion's staking contract (MiniChefv2 & Audited). We are initially aiming to minimize risk by releasing the funds every two weeks allowing time for assessments, and if needed, the re-balancing of rewards for underperforming pools. 

The multisig will be managed by: 

- 3 Evmos DAO Governance members (Benny Lava, Tricky, LPX)
- 1 Diffusion team member (mercenaryApe)
- 1 Evmos Foundation member (<WHO WILL IT BE>

## **Incentives Allocations**

The EVMOS incentives will go towards attracting liquidity for EVMOS pairs with ATOM, WETH, WBTC, OSMO, JUNO, DIFF, and USDC pools. The EVMOS token incentive breakdown for those pools would be as follows:

- (POOL PAIRS) - EVMOS INCENTIVES (Amount per Bridge)
- EVMOS / ATOM - 400k
- EVMOS / wETH - 300k (150k each Axelar, Celer)
- EVMOS / wBTC - 300k (100k each Axelar, Gravity Bridge, Celer)
- EVMOS / Stablecoins - 800k (USDC split evenly between Axelar and Celer -- USDT and DAI for Gravity Bridge) 
- EVMOS / OSMO - 50k
- EVMOS / JUNO - 50k
- EVMOS / DIFF - 100k
  
For the kickoff program, we propose the equal distribution of incentives between the bridged assets **with the exception of gUSDC and gWETH pools**, as they are already being incentivized and are locked into smart contracts for the time being. 

![image](https://user-images.githubusercontent.com/16395727/192063915-ba6c8ae0-6e67-4eaf-9e87-3704002cfa8a.png)

  
## **Future Plans**
  
Future proposals can use this data to gauge their own bridge incentives. This will help the most desired liquidity continue to come onto Evmos and maintain attractive APRs while doing so. We are currently aiming to hit a TVL of $20mil on Evmos by the end of the year (across the entire network).

2mil EVMOS is less than 1.5% of our available funds, and covers an entire DEX including interchain assets on Evmos. When compared to the 0.5% spent for a single EVMOS/OSMO pool, we firmly believe that this kickoff initiative is reasonable. We are currently working on a standardized framework in which these processes can be streamlined and more transparent; we thank the community for your patience and thank you to all those that have participated in the discussion stage of the proposal.

**About Diffusion:**

Diffusion is the a Uniswap v2 fork with Sushi's MinichefV2 implemented for rewards distribution. Diffusion was the first DEX and by far the largest in TVL and volume before the Nomad hack. With stablecoins back on Evmos and incentives to give them a boost, the revitalized team will soon be releasing a new roadmap and their plans to continually improve the DEX.

---
- Authors: Tricky, Benny Lava, & LPX of Evmos DAO Governance Workstream
- Reviewed by Diffusion team
- Funding amount signaled by [the Evmos Community on Commonwealth](https://commonwealth.im/evmos/discussion/6977-kickstart-defi-on-evmos) and during Governance Call.
---
  
Payload:
  
  `./evmosd tx gov submit-proposal community-pool-spend ./liqme.json --from lpx --gas 1000000 --fees 100000000000000000atevmos --chain-id "evmos_9000-4" --node https://evmos-testnet-rpc.polkachu.com:443`

  ```
  

 {
    "title": "",
    "description: "",
    "recipient": "holdup",
    "amount": "0aevmos",
    "deposit":"10000000000000000aevmos"
 }
  ```

