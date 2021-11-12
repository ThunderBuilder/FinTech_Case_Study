# Unit 1 Homework Assignment: FinTech Case Study
# ELROND NETWORCK 

Elrond was co-founded in late 2017 by brothers Beniamin and Lucian Mincu alongside Lucian Todea as a solution to the problem of blockchain scalability, which they  thought to be the most pressing problem facing the industry.

Prior to Elrond, Beniamin and Lucian Mincu co-founded MetaChain Capital, a digital asset investment fund, with Beniamin Mincu serving as CEO and Lucian Mincu as chief technology officer. The two also co-founded ICO Market Data, an aggregator of information around  initial coin offerings.

Beniamin Mincu was also responsible for product, marketing and community for blockchain platform  NEM from 2014 to 2015, in addition to being an early investor in projects such as Zilliqa (ZIL), Tezos (XTZ), Brave and Binance. Lucian Mincu has additional experience as an information technology engineer and security specialist, having worked with Uhrenwerk 24, Cetto and Liebl Systems.

Todea is a serial tech entrepreneur who previously founded and served as CEO of Soft32, a software review and download site, and a partner of mobilPay, a mobile payments application. He is also an angel investor, having invested in biometrics tech company TypingDNA and accounting platform SmartBill.

Elrond is a complete rethinking of public blockchain infrastructure, specifically designed to be secure, efficient, scalable and interoperable. Elrond’s main contribution rests on two cornerstone building blocks: 1) A genuine Adaptive State Sharding approach: effectively partitioning the chain state into multiple shards, handled in parallel by different participating validators; 2) Secure Proof of Stake consensus mechanism: an improved variation of Proof of Stake (PoS) that ensures long term security and distributed fairness, while eliminating the need for energy intensive PoW algorithms.
The Elrond Virtual Machine is a dedicated smart contract execution engine built on WASM. It expands the family of languages available to smart contract developers to include Rust, C/C++, C#, Typescript. This means you can write smart contracts in whichever language you’re familiar with, compile it of WASM and easily debug its WAT human readable format.

MALTA / ACCESSWIRE / June 19, 2019 / Elrond, a leading sharding-based public
blockchain network, has announced the closure of its private round investment,
raising $1.9 million from Binance Labs, Electric Capital, NGC Partners, Maven
11, and Authorito Capital.

EGLD-USD currently hovers around $270 territory. It’s up over 950% YTD and 3,400% for the past 12 months. Moreover, the altcoin has gained about 19% over the past one month. With a market cap of over $5.3 billion, it currently ranks as the 37th largest cryptocurrency in the market according to CoinMarketCap.

Architecture Overview

Elrond is a high-throughput public blockchain aimed at providing security, efficiency, scalability and interoperability, beyond the current state-of-the-art. The two most important features that set Elrond apart are Adaptive State Sharding and the Secure Proof of Stake consensus mechanism.

Elrond is a complete redesign of blockchain architecture with the aim to achieve global scalability and near instant transaction speed. Elrond's architecture rests on the following key innovations:

Adaptive State Sharding on all levels: transaction, data and network. The dynamically adaptive sharding mechanism will perform shard merging and shard splitting while taking into consideration both the number of available validator nodes and also the network usage.
Secure Proof of Stake Consensus, completed in just two communication steps, using modified Boneh–Lynn–Shacham ("BLS") multi-signatures among the validators of the consensus group. Moreover, nodes inside the shard are randomly selected for the consensus group with no possibility of knowing the group's composition more than one round in advance.
High resiliency to malicious attacks due to periodical node reshuffling across shards. Every epoch, up to 1/3 of the nodes in every shard are reshuffled to other shards in order to prevent collusion.
Secure randomness source with BLS signing, which makes it non-biasable and unpredictable.
The Arwen WASM VM, an exceptionally fast virtual machine for executing smart contracts written in any programming language that can compile to WebAssembly.
Smart contracts on a sharded state architecture, with balanced load on shards. This is a requirement for a high-throughput blockchain platform. Balancing smart contracts across shards allows Elrond to run multiple SCs in parallel, while the cross-shard calls are handled by an asynchronous cross-shard execution process.
Fast finality for cross-shard transactions in mere seconds. Having a very high TPS is required for a high throughput blockchain solution, but TPS is only half the picture: fast finality for cross-shard transactions is of crucial importance. Most existing state-of-the-art blockchain architectures refuse to mention this aspect, but from a user standpoint it is extremely important. Fast cross-shard finality is naturally handled by Elrond at the protocol level, using a dispatching algorithm and a routing protocol.

Glossary

Metachain: the blockchain that runs in a special shard, where the main responsibilities are not processing transactions, but notarizing and finalizing the processed shard block headers.

Address: the public key of a wallet. The Elrond Address format is bech32, specified by the BIP 0173. The public key always starts with an erd1. e.g.: erd1sea63y47u569ns3x5mqjf4vnygn9whkk7p6ry4rfpqyd6rd5addqyd9lf2.

Node: a computer or server, running the Elrond client and relaying messages received from its peers.

Validator: a node on the Elrond network that staked at least 2500 EGLD, that processes transactions and secures the network by participating in the consensus mechanism, while earning rewards from the protocol and transaction fees.

Observer: a passive member of the network that can act as a read & relay interface.

Validate: the act of running a validator node and contributing to the network by relaying and validating information.

Stake: contribute to the network security by delegating 1 EGLD or more towards a staking provider that operates validator nodes.

Delegate: contribute to the network security by delegating 10 EGLD or more towards the Elrond Community Delegation contract.

Stake rewards: locked funds for running validator nodes to secure the network and generate income in form of rewards. Rewards can be claimed or restaked.

Delegate rewards: locked funds from delegation contracts also generate income in form of rewards. These rewards can be claimed or redelegated

Unstake: the intention to unlock staked/delegated funds, that will become available after the 10 epoch unbonding period.

Unbond: withdraw the funds in the original account after the 10 epoch unbonding period.

Staking provider: node operator that created a staking pool and accepts funds for staking.

Staking pool: a system smart contract that accepts funds for staking.

Delegation cap: the maximum amount of funds accepted by a staking pool.

APR: annual percentage rate.

Service fee: fee that the service providers are taking from the rewards their staking pools have received.
Entities

There are two primary entities in Elrond: users and nodes.

A user is anyone holding one or more pairs of keys (one secret, one public). Using a pair of keys, the user can submit signed transactions to the network. The Elrond network treats each pair of keys as an account, and each account implicitly has an associated amount of EGLD tokens, called the balance of the account. Moreover, an account also has an associated mapping storage, which holds arbitrary values.

An account is uniquely identified by its address. The Elrond network defines the address of an account to be equal to the public key of its corresponding pair of keys (the secret key remains known only by the user that owns the key pair). The public key is 32 bytes in length, which means that the address of an account is 32 bytes as well. As a standard, the Elrond network uses the Bech32 human-readable representation for account addresses.

Users normally manage the keys of their accounts using wallets, which are applications dedicated to securely contain these keys. While it's completely possible to manage one's keys and accounts without a wallet application, it is an uncommon practice and employed mostly by advanced users or by automated processes. The nodes are the devices connected to the Elrond network, which perform the operations requested by its users. Nodes can be either passive or actively engaged in processing tasks. Eligible validators are active participants in the network. Specifically, they are responsible for performing consensus, adding blocks, maintaining the state, and they are also rewarded for their contribution. Each eligible validator can be uniquely identified by its 96-byte-long BLS public key (not to be confused with account keys, which are generated with the Schnorr algorithm).

A user that manages one or multiple nodes is called a node operator. These users must stake a substantial amount of EGLD tokens for each of their node as a collateral, effectively vouching for the correctness and performance of the nodes. The network locks the staked amount, which cannot be accessed by the node operator unless they withdraw both the stake and the nodes. Nodes that have been staked for by a user are promoted to validator status, and they may participate in consensus and earn rewards for their contribution. Without staking, nodes remain observers of the network. While passive, observers are still important in the network.

Web Wallet :
https://maiar.com

Use the wallet to send, receive and store EGLD in a secure manner. Includes automations for interacting with staking products and ecosystem pools.

The Maiar DeFi Wallet

All the components for a global financial system that operates at internet scale are in place.
The Elrond protocol is capable of the throughput required by the next billion people.
The Maiar App is on its way to onboarding them.
The Maiar Exchange economic engine is ready to be battle-tested.
To light the fuse for internet-scale DeFi, we are thrilled to introduce the Maiar DeFi Wallet - a web extension for Chrome, Brave and other Chromium browsers - that acts as a companion for Elrond dApps!
The Maiar DeFi Wallet can host multiple Elrond wallets and quickly swap between them, to send and receive EGLD and ESDT tokens, as well as sign transactions for DeFi products, such as the Maiar Exchange.
Product Positioning
The Maiar App is intended to seamlessly onboard new crypto users and offer them core features, such as fiat on-ramps, sending & receiving, staking, logging in with a QR code and signing messages. It is also the perfect companion for experiencing DeFi products on the go.
The Elrond Web Wallet is intended as a full-featured rich desktop client. It does everything the Maiar App can do, and has a lot more features on top, such as richer dashboards, more information, access to special events and more login options, all displayed in a beautiful interface tailored for large screens.
The Maiar DeFi Wallet is a lightweight version of the Elrond Web Wallet that reduces the number of steps and time required for users to interact with Elrond dApps.
By simply clicking the appropriate button on a web extension pop-up, instead of picking up their phone or loging in repeatedly, a power DeFi user can significantly accelerate their interaction with decentralized products. They thus gain an edge when trading, farming, or even interacting with games and other Elrond dApps that will all be able to integrate the Maiar DeFi Wallet.
In addition, the Maiar DeFi Wallet allows importing multiple different wallets and connecting to different networks, such as mainnet, testnet or devnet. For convenience, you only need to input the password once, as a login. You can securely swap between multiple wallets and sign messages or transfer funds, without having to login again.
Maiar DeFi Wallet security
The web extension only stores the cryptographic hashes relevant to the imported wallets, which can exclusively work with a secure password that only you know.
The Maiar DeFi Wallet has been audited by security professionals, passed the Chrome Store verifications and was intensely tested by the internal team and a private round of DeFi experts.
As an extra precaution, we are releasing the extension with the restriction of connecting to the testnet and devnet, to conduct heavy public testing before finally going live with the mainnet version.

The Maiar Exchange and MEX token:
https://maiar.exchange
The Maiar Exchange will launch in November.

It's a DEX AMM running on the Elrond Network. It is built by the same team that has built the Elrond blockchain. You could call it the "official" DEX. There can be any number of DEX-es built on Elrond, but the team wanted to build the first one, because it is special.
SFTs LP Tokens: trade, collateralize - Providing liquidity on the Maiar Exchange gives you LP tokens, like most AMM DEXes. Uniquely in the space, the Maiar Exchage LP tokens are tradeable. This means you can provide liquidity, then sell your position, or take a loan against it (use LP tokens as collateral). Awesome and a DeFi first, because of Elrond’s unique ESDT (Elrond Standard Digital Token) architecture.

Maiar App: onboarding, 2FA - You can use Elrond’s Maiar app to login and sign transactions on the Maiar Exchange. As secure as a Ledger hardware wallet, as convenient as Face ID + tapping on the screen.

Additionally, Maiar is super easy to use - it automatically and securely creates a wallet in seconds, using just a phone number (not shared, only a hash of it is used one time for wallet creation). ~500k users use Maiar, and it was just launched in February ~ 6 months ago.
The Elrond ecosystem has 200+ partners. With the launch of the Maiar Exchange, the ESDT version of their tokens can be deployed in liquidity pools and expand access for their community. This will generate adoption for the Maiar Exchange, volume, and generate more transactions on the Elrond blockchain, increasing demand for EGLD in the process.
MEX is the token powering the Maiar Exchange. It is required for the governance of the decentralized exchange platform, as fuel for the perpetual decision-making process that will maintain the Maiar DEX ahead of the curve in terms of innovation, operational model, listing policies, and other actions aimed at creating a sustainable value cycle for its stakeholders. Furthermore, the MEX token is designed as a value capture mechanism and incentive vehicle that will allow the compelling attributes of the economical advancements it enables to scale with its adoption. 

https://elrond.com/blog/maiar-exchange-mex-tokenomics/
