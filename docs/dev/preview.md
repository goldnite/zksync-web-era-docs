# Alpha preview

zkSync is first and foremost a mission-driven project. Our goal is to make web3 accessible to everyone. zkSync 1.x provided access to transfers/swaps/nft minting secured by Ethereum for a fraction of the cost.

zkSync 2.0 opens the whole ecosystem of Ethereum to mass adoption. To make web3 accessible to every person no matter its income, it will let the users choose between high security & 20x fee reduction compared to Ethereum or security much higher than a typical sidechain & near-constant tx costs. Unlike before, these users will be able to participate on the same chain. To provide more customization for users' wallets, zkSync 2.0 will also support account abstractions. More features are to come!

Implementing all the features required for the next generation of L2s is a big task. We're actively working on making the next generation of zero-knowledge rollups as easy (or even more!) to use as Ethereum itself.

So, the current state of implementation is the **alpha preview**. It means that while there are a lot of things that are not there yet, the core of the system is ready, it works, and serves its purpose.

## What is available now

- **Native support of ECDSA signatures.** It means that unlike the first version of zkSync and most of the ZK Rollups no special operation is required to register the user's private key. Any account can be managed in L2 with the same private key that is used for L1.
- **Solidity 0.8.x support.** No need for change and re-audit of the codebase.
- **Web3 API**. With small exceptions, our API is fully compatible with Ethereum. This allows seamless integration with existing indexers, explorers, etc.
- **Support for Ethereum cryptographic primitives**. zkSync natively supports `keccak256`, `sha256`, and `ecrecover` via precompiles.
- **Hardhat plugin**. Which allows easy testing and development of smart contracts on zkSync.

## What will be released soon

- **More developer tooling!** Composability between various hardhat plugins with the zkSync plugin, easy local setup with Docker, etc will be essential for the growth of the ecosystem.
- **L1 <> L2 interoperability.** L1 <> L2 calls are very important for bridges, cross-layer governance protocols, etc.
- **Support for Vyper and older versions of Solidity.** We are actively working on supporting different versions of Solidity to allow seamless integration for the existing projects.
- **Priority mode implementation.** Even if the zkSync operators go down, the users must be able to withdraw their funds from the protocol. The priority mode is the mode that is triggered when the operator becomes malicious or unavailable. It allows anyone to become an operator and process transactions.
- **zkPorter extension.** One of the biggest and most important features. It will let the users choose between high security & 20x fee reduction compared to Ethereum for zkRollup accounts or security much higher than a typical sidechain & near-constant tx costs for zkPorter accounts.
- **Account abstractions.** Imagine being able to implement custom logic for signature checking for your account. Or maybe social recovery? Before users had to create separate accounts for such purposes. All of this would be easily supported with account abstractions.