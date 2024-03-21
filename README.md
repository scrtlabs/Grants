# Secret Grants
This is the main repository for Secret Grant proposal submissions. This README provides a high level overview of Secret Grants. Please submit all Secret Grant requests by creating a new [issue](https://github.com/SecretFoundation/Grants/issues). Welcome!

**The updated Secret Grants program was announced on Dec 1 2023 - Please read the [announcement](https://scrt.network/blog/scrt-labs-grants-program) carefully.**

**The latest cohort - Q2 2024 - was announced [here[(https://scrt.network/blog/q224-grants-open/).** 

## Proposal Categories
Grant proposals fall primarily into fourthree categories:  **Privacy-as-a-Service**, for projects using Secret Privacy-as-a-Service features; **Secret Apps**, for everything that is directly built on top of Secret Network; **Ecosystem**, for tools that expand Secret Network and improve general usability; and **Network improvements**, for major upgrades to the network itself. Please consult the below list of ideas we’ve recognized to date as being of special interest to the community and essential to ongoing ecosystem growth. That said, we welcome any and all proposals and recognize that the most interesting proposals may be things the Secret Network community has yet to consider. Innovation knows no bounds!


## Privacy-as-a-Service
This category includes dApps that run on other blockchains and use Secret for confidential computation, storing of confidential data and the like.
Possible use cases for such application include the following:
* **Confidential Order Books**
* **Confidential Voting** Use of additive HME to allow for user generated voting pools
* **Sealed-bid Auctions**
* **Confidential Payroll and Transfers**
* **NFTs with locked content**
* **Digital Identity** Specifically on-chain credentials based on reputation of your private on-chain interactions
* **Private Key Backup** Inheritance and Key storage using Private secret contracts
* **Gaming**
* **Usage of SecretVRF**
* **MPC wallets or MPC usecases** Use a Secret contract as a signer within your distributed computation protocol - Wallets, MEV protection, privacy etc.

Additional ideas for more use cases are also encouraged.


## Secret Apps

### Secret DeFi
Secret DeFi is a privacy-first, front-running resistant DeFi ecosystem. Its growth has seen the development of Secret Tokens (a fungible privacy token standard), crosschain mainnet bridges (including to ETHereum and Ethereum Layer2s (Axelar), Polkadot (Composable), Binance Smart chain (Axelar), Solana (wormhole), Cosmos - IBc (ATOM, TIA, dYdX, OSMO etc.). With live applications like Shade Protocol and their native stablecoin SILK there are multiple layers to build on top off.

We welcome the community to submit grant proposals to build any of the applications below:

* **Staking derivatives** to create capital efficiency in the Secret Network. Staking derivatives allow staked SCRT to be used for further yield opportunities in Secret DeFi. Here’s one attempt on a product roadmap.
* **Liquidation engine integrations for Secret liqudity**
* **Variable interest lending products:** Either Secret-based implementations of ETH DeFi projects such as Compound or Aave, or brand new lending products leveraging Secret’s unique properties.
* **Algorithmic stable coin projects** (such as Maker-type implementations). We believe it’s critical for the Web3 ecosystem to have a decentralized stable coin with privacy.
* **Managed/automated DeFi strategies**
* **Dark pools (private orderbook exchange) for privacy preserving trading.** A Dark Pools secret contract manages the encrypted order book in its state and can run multiple order matching methods such as Market / Limit / Stop-Loss orders.
* **Fixed income products:** Fixed interest lending / borrowing products with insurance / liquidity pool to guarantee fixed payments.
* **Credit scoring and under collateralized lending** using liquidity / insurance pools and Secret Oracles that tap into Web2 data sources like Plaid or centralized exchange balances. Undercollateralized loans can be built on top of Secret Network using on-chain privacy-preserving reputation credit scoring contracts.
* **Advanced AMM / CFMM DEXs** optimized for low slippage trading (like Curve) or multiple pools (like Balancer) to create decentralized index funds.
* **Derivatives and Contract for Difference products** with SCRT and SNIP20 collaterals
* **Options contracts:** Put / call options based on an orderbook or AMM model with SCRT and SNIP20 collaterals
* **Synthetic Asset creation** with SCRT and SNIP20 collaterals
* **Decentralized Perpetual Swap products** (with vAMM similar to Perpetual Protocol with front-running resistance for more efficient capital deployment)
* **Insurance products** for Secret DeFi

### Secret Vaults
* **Decentralized Substack:** Build a decentralized content (audio, blog) monetization tool for content stored on IPFS or another decentralized storage platforms. You can refer to this article for more information. Padlock and SecretVault contracts can also be an inspiration for access control related cases.
* **Dead Man Switch:** An event on the Secret Network (such as block numbers / elapsed time or a payment) triggers a secret contract to release a "secret" either to a selected recipient (private output) or the entire network (public state).

### Data Marketplaces
* Crowd-sourced signal generation with staking incentives for SNIP20 and synthetic asset trading
* Decentralized and privacy preserving machine learning use-cases (image recognition, collaborative private model training etc.)

### Secret NFTs / Metaverse
* Secret Lootbox for SCRT / ETH / SOL / etc games: Lootbox NFTs used in games on Secret or other networks would be represented with SecretNFTs, revealing rewards only after NFT is claimed
* p2p NFT lending

### Decentralized Governance and DAOs
* **SecretFund:** Build a DAO funded by block rewards of delegators participating in the DAO. Delegators receive governance tokens proportional to their contribution. Governance tokens determine how the funds in SecretFund are managed.

## Ecosystem

### Interoperability
* Secret Network - Bridge to Monero, Bitcoin or other L1 using the Secret Private contracts to store private keys of the other chain.
* SecretTunnel - Interoperable Secrets: Create a contract to verify state changes and allow asset transfers between Secret Network and L2 Secret Network forks for big data and high throughput use-cases.

### Oracles
* Secret Oracles: Build TLS connection from validator enclaves to certain APIs to create private data feed for secret contracts (i.e. Binance and other exchange balances for decentralized credit scoring / leverage)
* Public API oracles: Allow Secret Network validators (or nodes) to query public APIs for on-chain secret contract based oracle. Validators would reach on-chain consensus on inputs
* Oracle support for Secret Network using Chainlink, Pyth, SupraOracles etc.

### Developer tools and improvements
* Tooling for one-click-run-and-deploy of contracts (like Remix for Secret Contracts)
* Network forks suitable for Big Data and high throughput (< 1 second block time for orderbook based DEXs)
* Create a library for running Secret Contract integration tests (like how Truffle uses Mocha/JS for Solidity)

## Network improvements

While we intend to share more details on these potential protocol-level improvements in future posts, here is a brief list of possibilities:

* ML Library that can run on-chain (requires deterministic floats or fixed-point support)
* MPC keys distributed across the validator set so to generate decryption keys (HME voting, External MEV protection etc.)
* Differential privacy library for getter methods
* Fully Homomorphic Encryption backend
* Gas/Fee abstraction methods
* Modules to improve the usage of community funds and allows them to flow through Cosmos

## Grant Details

Please review the following details before applying:

### Funding amount
Funding amounts are variable, depending on the complexity and value to the network, although the average grant would likely be in the order of thousands or tens of thousands of dollars. Grants may be split into several smaller milestones and receive funding accordingly on a per-milestone basis, as mentioned below. Since this is a non-dilutive funding opportunity, we encourage commercial projects to also look for alternative sources of funding as well. We are especially interested in seeing new start-up companies and projects emerge that build exclusively on Secret Network. For these in particular, non-dilutive funding such as a grant would be significant.

Grant awards will be distributed in 3 or more installments, with initial payment to take place right after approval of the grant. Teams are expected to define key milestones for the project and propose installment amount upon completion of different milestones. It is important that the milestones relate to reaching PMF and/or significant adoption. Higer grants are awarded to projects reaching 

### Requirements
All software projects developed using grant funds program must be released under a permissive open-source license, such as MIT, Apache 2.0, 2-Clause BSD or similar.

### Who are we looking for
We are looking for individual developers, new and existing companies and projects, community members or established teams with a proven track record to contribute to the Secret Network ecosystem. Prior work on Secret Network or experience in deploying Ethereum or other blockchain applications is a big plus.

Secret Apps are encouraged to have a path for commercial sustainability (token or fee model).

### Recommended Process
First, **ideation:** Use Secret Network developer forum and Secret Network Discord (#use-cases and #find-a-team channels) to brainstorm, discuss ideas and form teams. We encourage you to get feedback from the community (including the Enigma development and product team) before submitting any application.

Then, **application:** When ready, submit an application via the [Issue tab of this repository](https://github.com/Scrtlabs/Grants/issues). Do this by opening a new issue in the format of [this sample application](https://github.com/SecretFoundation/Grants/blob/main/Sample%20grant%20application).

The application should cover the following details:

* High level description of the project
* Problem / solution (max. 200 words)
* Detailed product / network improvement description (max. 500 words)
* Go-to-market and commercialization plan (if applicable)
* Team: Please share all past experiences, github links and repos
* Milestones and budget: Please provide a budget, development timelines for milestones and distribution of budget based on milestones.

If you’d instead like to apply privately, please email info@scrtlabs.com with the above information.

### Evaluation process
We will review your application and get back to you with next steps (request for more information, schedule a video interview etc.) in two weeks.

# THANK YOU!
Thank you for your interest in Secret Grants! We cannot wait to work alongside you in building Secret Network into a data privacy hub for all blockchains, helping secure the decentralized internet.
