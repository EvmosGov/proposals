# Build A Community Owned DEX (UniV3)
## Authors
-  [Orbital Apes](https://twitter.com/OrbitalApes)
-  [Evmos DAO](https://twitter.com/EvmosDAO)

## Summary
The Evmos DAO and Orbital Apes team aim to deliver a fully community owned DEX within two months. We believe that Evmos can become market competitive in terms of liquidity and user experience. 

- No investment token 
- No initial swap fees 
- Not profit oriented
- UniV3 functionalities (concentrated liquidity)
- Integrated IBC asset and continous development guaranteed

If this proposal passes, we will ship a V3 DEX deployment in the shortest amount of time. The OA team will handle the engineering side, while the responsibilities of socials management, proposals for incentives and incentives management would be handled by the EvmosDAO.

The requested funds is for the Orbital Apes team only since the Evmos DAO is already fully funded. Funding is requested as this DEX will be built as public good for Evmos and will not have any funding coming from token sales or protocol fees.

*Notes: This can be seen as an alternative to the ICHI proposal. We believe that we can ship a more feature rich DEX at **much lower costs**. To our knowledge, UniV3 is not adding new chains any time soon due to legal reasons.*


## Goal
Create a capital efficient AMM to grow native liquidity on Evmos. This will be achieved with the help of EvmosDAO by creating cross-chain proposals for co-incentives (Evmos and Partnering chain) to LP providers and cross-chain token swaps to create protocol-owned liquidity managed by EvmosDAO.

## Deployment Path of UniV3 Fork

- Engineer custom V3 DEX frontend with IBC<>ERC20 conversion
- Fork UniV3 and deploy modified contracts (no protocol fees, no investement token) in April
- Bridge integration  
- Keplr integration (third party dependency)

### Benefits  
**1 - Liquidity**
The Evmos DAO team will be making proposals on other IBC chains to incentivize this DEX along with supplemented Evmos incentives.Protocol owned liquidty would work along side this as well. This will allow Evmos to build more native liquidity and force wider users to IBC tokens into Evmos. After this more DeFi protocols can be built once on chain liquidity is established.

**2 - Time to market**
We are market ready within two months. Targetting testnet before April and mainnet once the UniV3 license expires. 
*Side note: The whole cosmos ecosystem is moving towards LSD's. V3 positions are much more tuned for these pools then traditional Dex's. V3 is may more profitable for LP's and provides a much stronger peg between something like stAtom/Atom. If we wait 5 months instead of 2 months we could potentially lose a large chunk of this liquidity to other protocols.*

**3 - Keplr integration**
In the near future Keplr is going to have full EVM compatibiltiy. The users will be able to interact with Keplr and Metamask on the DEX.

- [ERC20 Support](https://github.com/chainapsis/keplr-wallet/pull/531)
- [Tx Signing Support](https://github.com/chainapsis/keplr-wallet/pull/483)
- Contracts signing: Once contracts signing is integrated by Keplr the OA will merge it into the DEX.

**4 - IBC conversion page**
Similar to https://app.evmos.org/assets, this will provide a user friendly interface and reduce complexity of onboarding cosmos based users. A bridge section will be added to deposit/withdraw from multiple EVM chains such as Ethereum, Avalanche, BNB and many more through Satellite (Axelar). 

**5 - No Protocol Fees** 
Traditional decentralized exchanges charge a fee on every swap that flows directly to the protocol or token holders. Initially this will be set to zero, any changes of the fee structure must be approved by the Evmos governance in form of a text proposal. LP fees will still be charged and distributed on swaps to LP providers.

**6 - No Investment Token**
The community owned DEX will not have a corresponding governance token. As a community owned project built by OA/EvmosDAO future major developments will be funded through seperate funding requests or grants programs/boutnies. Incentives for liquidity will come in the form of Evmos incentives proposals and Cross-Chain incentives proposals.


**7 - Future Development: All the upcoming Evmos/Cross-Chain innovation**
- New innovation like ICA and ICQ will be actively explored and integrated the best possible way to stay competitive. Such integration would require a seperate funding request.
- Explore and integrate cross-chain bridge swaps through services such as LiFi.


## Milestones

- Deploy the AMM V3 (Contracts/Frontend/Backend) to the Evmos Testnet | Funds realesed: 40% two weeks after testnet 
- Deploy the AMM V3 (Contracts/Frontend/Backend) to the Evmos Mainnet | Funds realesed: 40% two weeks after mainnet 
- IBC conversion page integration | Funds realesed: 10% after functional integration 
- Keplr integration | Funds realesed: 10% after functional integration 


## Funding Amount
This funding proposal will kick off the development for V3. The requested amount of 200,000 Evmos goes fully to the OA team since the Evmos DAO is already funded by the Evmos community.

Signatories (3/4 Threshold):
- GV | DAO 
- CtrlAltApe | OA
- Luisqa | Zenith Station
- Silk Nodes 

Safe Deployment Address: [0x7B4Ca78E62e06De7A921DF03A319ff09A09A84D0](https://safe.evmos.org/evmos:0x7B4Ca78E62e06De7A921DF03A319ff09A09A84D0/home?showCreationModal=true)

**Risk / Risk Mitigation**
Risk: The OA team fails to deliver an AMM for the community.
Mitigation: Funds are held in a multisig and are paid out on completion of milestones.
