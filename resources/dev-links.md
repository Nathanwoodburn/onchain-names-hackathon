# Dev Links


## Onchain Wallet

[https://www.rainbowkit.com](https://www.rainbowkit.com/)

[https://docs.walletconnect.com](https://docs.walletconnect.com/)

[https://www.dynamic.xyz](https://www.dynamic.xyz/)

https://metamask.io/sdk/

## Handshake

Handshake is a decentralized, permissionless naming protocol where every peer is validating and in charge of managing the root DNS naming zone with the goal of creating an alternative to existing Certificate Authorities and naming systems.

Regular domain names ending with `.com` , `.vn` are all domains on these Top Level Domains (TLDs). Handshake is an alternate root zone where anyone can create and own their own TLD like `.theshake` and domains under it like `website.theshake`.

For more info, check out the links below:

An intro to Handshake: https://learn.namebase.io/about-handshake/about-handshake

Official website: https://handshake.org/

Protocol summary: https://hsd-dev.org/protocol/summary.html

## Core software

### hsd (complete node with wallets)

The core node software that powers the handshake network is called `hsd` and is written in Javascript. This node connects to other peers and syncs the blockchain. It can also manage wallets to store funds/domains and participate in auctions.

hsd code: https://github.com/handshake-org/hsd

Install guide: https://github.com/handshake-org/hsd/blob/master/docs/install.md

### hnsd (light client / resolver only)

If you don’t need all the feature of hsd and only want to resolve Handshake DNS, then `hnsd` is a light client written in C. Just like hsd, it is also decentralized and directly talks to other peers. As a light client, it syncs only block headers so is much faster than hsd, but all it can do is resolve handshake domains by asking proofs from other peers. This is typically enough for end-users / first time devs to get started with Handshake.

hnsd code / Install guide: https://github.com/handshake-org/hnsd

## Other Projects

The Handshake ecosystem has a lot of projects, most open source, and would love some contributions!

> **Also: Read https://theshake.xyz/resources/build as it covers many other Handshake projects.**
> 
- <expand>
    
    ### Fingertip
    
    Fingertip is a resolver that makes it easy for everyone to use hnsd (and also adds DANE support).
    
    Code: https://github.com/imperviousinc/fingertip
    
    ### Bob Wallet
    
    Bob Wallet is a desktop wallet built on hsd. It can be used to store funds, domains, participate in auctions, trade names and more.
    
    Code: https://github.com/kyokan/bob-wallet
    
    ### Fire Wallet
    
    A new wallet being developed, also uses hsd under the hood.
    
    Code: https://github.com/Nathanwoodburn/FireWalletBrowser
    
    ### And more!
    
    There are too many to list here, check out https://theshake.xyz/resources/build for a better organized and longer list.
    

## ENS

ENS (Ethereum Name Service) is a distributed, open, and extensible naming system based on the Ethereum blockchain. It allows users to associate human-readable names (e.g., "myname.eth") with Ethereum addresses, content hashes, and other cryptocurrency resources. This makes it easier to remember and share addresses instead of dealing with long, complex strings of characters.

Official website: https://ens.domains/

Docs: https://docs.ens.domains/

## Base

Base is built as an Ethereum L2, with the security, stability, and scalability you need to power your onchain apps. Confidently deploy any EVM codebase and onramp your users and assets from Ethereum L1, Coinbase, and other interoperable chains.

https://base.org

[https://docs.base.org](https://docs.base.org/)

## zkSync

zkSync is a trustless Layer 2 protocol for scalable low-cost payments on Ethereum, powered by **[zkRollup technology](https://zksync.io/faq/tech.html#zk-rollup-architecture)**. It is a user-centric zk rollup platform from **[Matter Labs](https://matter-labs.io/)**, with security, user experience, and developer experience as the core focus.

[https://zksync.io](https://docs.zksync.io/)

[https://docs.zksync.io](https://docs.zksync.io/)

Stellar is a layer-1 open-source, decentralized, peer-to-peer blockchain network that provides a framework for developers to create applications, issue assets, and connect to existing financial rails. Stellar is designed to enable creators, innovators, and developers to build projects on the network that can interoperate with each other.

[https://stellar.org](https://stellar.org/)

https://developers.stellar.org/docs

## Internet Computer (ICP)

The Internet Computer (ICP) is a blockchain network that aims to be a decentralized cloud computing platform. It allows developers to build and run applications, websites, and services directly on the internet without relying on centralized cloud providers. ICP introduces the concept of "Internet Identity" for users to access various services built on the platform. It uses a different model than Ethereum where developers, not users, pay for computation resources their applications consume. ICP provides decentralized data storage and aims to offer an open, decentralized alternative to traditional web services.

https://internetcomputer.org

https://internetcomputer.org/internet-identity

Base is built as an Ethereum L2, with the security, stability, and scalability you need to power your onchain apps. Confidently deploy any EVM codebase and onramp your users and assets from Ethereum L1, Coinbase, and other interoperable chains.

## Akash

Akash Network allows anyone to buy or sell cloud computing resources, such as CPU, RAM, storage, and bandwidth, in a decentralized manner. Providers can earn AKT tokens by offering their unused computing capacity on the network. Developers and businesses can then rent these resources on-demand to deploy and run applications, websites, or services at a lower cost compared to centralized cloud providers.

https://akash.network/

https://akash.network/docs/

## Unstoppable Domains

Unstoppable Domains is a blockchain-based domain name system similar to ENS that allows users to purchase domains with extensions like ".crypto", ".blockchain", ".nft", etc. It enables users to create decentralized websites and blockchain-based identities that cannot be censored or taken down by any central authority. These domains point to decentralized websites hosted on IPFS or decentralized storage solutions.

https://unstoppabledomains.com/

https://docs.unstoppabledomains.com/

## Flare network

Flare is the blockchain for data. It is a [layer 1](https://docs.flare.network/tech/glossary/#layer1), EVM smart contract platform designed to expand the utility of blockchain.

Flare's aim is to provide data as a public good, meaning that data is not controlled by a centralized entity and is available to all. The infrastructure providers, which perform doubly as [validators](https://docs.flare.network/tech/validators/) and [data providers](https://docs.flare.network/infra/data/operating/), enable two native oracles, the [FTSO](https://docs.flare.network/tech/ftso/) and the [State Connector](https://docs.flare.network/tech/state-connector/). This native processing provides developers on Flare with efficient access to large amounts of data and data proofs at minimal cost.

https://flare.network

[https://docs.flare.network/](https://docs.flare.network/tech/flare/)

## Cardano

Cardano is a collection of [open-source](https://en.wikipedia.org/wiki/Open_source), patent-free protocols. It's a platform that enables you to store, transform, and manage value, identity, and governance. Cardano follows research not opinions or bias.

https://cardado.org

[https://developers.cardano.org/docs/](https://developers.cardano.org/docs/get-started/)

## Connext network

Connext is a modular protocol for securely passing funds and data between chains. Developers can use Connext to build crosschain apps (**xApps**) - applications that interact with multiple domains (blockchains and/or rollups) simultaneously.

[https://connext.network](https://connext.network/)

[https://docs.connext.network](https://docs.connext.network/)

## LayerZero

LayerZero is a messaging protocol, not a blockchain. Using smart contracts deployed on each chain, in combination with [Decentralized Verifier Networks (DVNs)](https://docs.layerzero.network/explore/decentralized-verifier-networks) and [Executors](https://docs.layerzero.network/explore/executors), LayerZero enables different blockchains to seamlessly interact with one another.

[https://layerzero.network](https://layerzero.network/)

https://docs.layerzero.network/

## Avalanche

Avalanche is an open-source platform for building decentralized applications in one interoperable, decentralized, and highly scalable ecosystem. Powered by [a uniquely powerful consensus mechanism](https://docs.avax.network/learn/avalanche/avalanche-consensus), Avalanche is the first ecosystem designed to accommodate the scale of global finance, with near-instant transaction finality.

[https://avax.network](https://avax.network/)

[https://docs.avax.network](https://docs.avax.network/)

## Cosmos

The [Cosmos SDK](https://github.com/cosmos/cosmos-sdk) is an open-source framework for building multi-asset public Proof-of-Stake (PoS) blockchains, like the Cosmos Hub, as well as permissioned Proof-of-Authority (PoA) blockchains. Blockchains built with the Cosmos SDK are generally referred to as application-specific blockchains.

[https://cosmos.network](https://cosmos.network/)

[https://docs.cosmos.network](https://docs.cosmos.network/)

## Binance Smart Chain

BNB Smart Chain (BSC) is the blockchain component of the BNB Chain ecosystem that is equipped with the smart contract functionality and compatibility with the Ethereum Virtual Machine (EVM) and is used for developing various kinds of decentralized applications. The design goal of BSC was to leave the high throughput of BNB Beacon Chain intact while introducing smart contracts into the BNB Chain ecosystem. Being EVM-compatible, other than easy portability, BSC enjoys support of the rich universe of [Ethereum](https://academy.binance.com/en/articles/what-is-ethereum) tools and dApps

[https://bnbchain.org](https://www.bnbchain.org/en)

https://docs.bnbchain.org/docs/getting-started/

## Aptos

Aptos blockchain, designed with scalability, safety, reliability, and upgradeability as key principles, to address these challenges. The Aptos blockchain has been developed over the past three years by over 350+ developers across the globe. It offers new and novel innovations in consensus, smart contract design, system security, performance, and decentralization.

[https://aptosfoundation.org](https://aptosfoundation.org/)

https://aptos.dev/

## SUI

Sui is a layer-1 blockchain optimizing for low-latency blockchain transfers. Its focus on instant transaction finality and high-speed transaction throughput make Sui a suitable platform for on-chain use cases like games, finance, and other real-time applications.

[https:/sui.io/](http://sui.io/)

https://docs.sui.io/

## SEI

Unleashing the Power of Speed and Innovation. A cutting-edge blockchain where unprecedented speed meets innovation. Sei is redefining what developers can achieve, offering unparalleled transaction speeds, robust security, and groundbreaking scalability.

https://www.sei.io/

[https://docs.sei.io](https://docs.sei.io/)

## Kadena

Kadena was founded on the idea that blockchain could revolutionize how the world interacts and transacts. But to get to mass adoption, chain technology and the ecosystem connecting it to the business world needed to be reimagined from the ground up. Our founders built a proprietary chain architecture and created the tools to make blockchain work for business – at speed, scale, and energy efficiency previously thought unachievable.

https://kadena.io

https://docs.kadena.io/

## Axelar

Axelar enables secure token transfers and communication across different blockchains, regardless of consensus mechanisms or message payloads. It’s based on the same [proof-of-stake security model](https://docs.axelar.dev/learn/security#proof-of-stake-consensus) as many of the chains it connects. Interchain apps built on Axlear are truly permissionless: their transactions cannot be censored by any oracle, relayer, or validator.

[https://axelar.network](https://axelar.network/)

https://docs.axelar.dev/

## Filecoin

Filecoin is a peer-to-peer network that allows anyone to store and retrieve data on the internet. Built-in economic incentives ensure that files are stored and retrieved reliably and continuously.

[https://filecoin.io](https://filecoin.io/)

[https://docs.filecoin.io](https://docs.filecoin.io/)

## Arweave

The Arweave network is like Bitcoin, but for data: A permanent and decentralized web inside an open ledger.

Permanent storage has many applications: from the preservation of humanity's most important data, to the hosting of truly decentralized and provably neutral web apps.

The Arweave protocol is stable, mature and widely adopted. As such, its ecosystem is fully decentralized. This site is just the tip of the iceberg. It acts as a map that points you to places you can learn about, use and build on Arweave.

Dive in! The rabbit hole is deep, and the possibilities are endless.

[https://www.arweave.org](https://www.arweave.org/)

https://github.com/ArweaveTeam/arweave-js

## Flow

The Flow blockchain is a decentralized, developer-friendly blockchain designed for building decentralized applications (dApps), games, and digital assets. It was created by Dapper Labs, the company behind the popular blockchain game CryptoKitties.

The Flow blockchain aims to provide a scalable, secure, and user-friendly platform for building decentralized applications and managing digital assets. It utilizes a unique architecture called "multi-node proof-of-stake consensus" to achieve high throughput and low latency, making it suitable for applications that require high performance, such as games and digital collectibles.

Official website: https://flow.com/

Dev Quick Start: https://developers.flow.com/build/getting-started/quickstarts/hello-world

## Chia

Chia Network is a blockchain-focused company and platform that supports the creation and execution of smart contracts written in a custom-designed programming language called Chialisp. It seeks to build upon Nakamoto's consensus principles established in Bitcoin, relying on a consensus mechanism known as Proof of Space and Time. Chia specializes in decentralized data management, enhancing security, regulatory compliance, and eco-friendly practices across several sectors.

[https://www.chia.net](https://www.chia.net/)

[https://docs.chia.net](https://docs.chia.net/)