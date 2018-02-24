# qtumbounties

## Qtum needs your help!

This repository serves as an active index of open bounties and issues in the Qtum ecosystem. We've got issues of all difficulties so everyone can participate.

Qtum needs help all over. If you're interested in C++, [Qtum Core](https://github.com/qtumproject) is the place for you. If you're more comfortable with JavaScript, [QtumJS](https://github.com/qtumproject/qtumjs) has plenty of open issues.

## Contributing

Before you get started, please read through the Qtum [style guide](https://docs.google.com/document/d/1ynIlt-lTPVvbxvjCKsAlQ0ctLMK1feEef0DN7JkCZSU/edit?usp=sharing). 

If you're looking for a place to contribute, we're also available on [Gitter](https://gitter.im/qtum-project/Lobby).

# Projects

The following is a list of projects and prototypes with open bounties and issues. 

# Prototypes:

## APIs

The APIs for Qtum allow for smart contract and decentralized application developers to create a front end and otherwise interact and analyze the data and objects stored on the Qtum blockchain. Similar projects to these include web3.js (for Ethereum) and BitcoinJS (for Bitcoin). These APIs commonly provide other utilities and dependencies needed for interacting with the blockchain, such as applicable hashing algorithms, encryption, etc. 

We would like to see more API support in the Qtum ecosystem. We know not everyone designs their applications to work in Javascript, and so having a variety of languages to choose from would be beneficial to many developers. 

The current languages we are most interested in include: Java, Rust, Go, Python, and C#. 

Other Tasks:

* Database prototype for the x86 design backed by leveldb and capable of working in a consensus critical environment while allowing contracts to use infinite length key and value data.

# Qtum Core
https://github.com/qtumproject/qtum

Qtum Core is the heart of the Qtum project and implements the core blockchain protocol. It consists of many different components and is intended to be a heavy, but complete solution for most people in the ecosystem. Qtum Core is considered the reference implementation of Qtum, and thus is effectively the law for how the Qtum blockchain protocol should behave. The code for Qtum Core is based heavily on Bitcoin Core's code, and is written almost entirely in C++ with the exception of a Python based test suite. 

The components included in Qtum Core include:

* Wallet - A mechanism for storing and using tokens with both GUI and RPC based interfaces for usage
* Consensus - The consensus rules which maintain the security of the Qtum blockchain. They can not be changed without incredible coordinated effort to ensure everyone else on the network updates. 
* P2P Network - The network by which nodes communicate to transfer transaction data, block data, etc
* Staking - A component whereby you can use the tokens stored within this node in order to create new blocks and validate transactions. 

# QtumJS
https://github.com/qtumproject/qtumjs

This is our primary official API at the moment interacting with blockchain applications built on Qtum. 

# Qtum-Electrum
https://github.com/qtumproject/qtum-electrum

This is a lightweight wallet-only version of Qtum. This version can be used for storing and using tokens, but can not be used for staking and relies on external Qtum Core nodes to validate the network and transactions within it. 

# Qmix
https://github.com/kfichter/qmix

Qmix is Qtum's in-browser Solidity IDE (an homage to [remix](https://remix.ethereum.org)). Qmix is currently very much in beta, and we're looking for feedback! We've got a bunch of things that currently don't work and a lot of room for feedback.

## Open Issues
- We currently only allow importing files from within Qtum. We want to allow imports from github gists as well.

# x86 VM
https://github.com/qtumproject/x86lib

This is a specialized x86 based virtual machine implementing the Intel i686 instruction set. This is Qtum's future direction and will allow developers to write smart contracts in mainstream programming languages such as C++, Rust, and Go. There is also a prototype GCC based toolchain targeting the "operating system" implemented by this VM.

## Database
Currently Qtum is using Ethereum's database for all contract storage needs. This has several shortcomings though that we wish to remedy. We want to be capable of storing unlimited (or almost unlimited) length key and value data, and for this data to be represented in an efficient and easy to query manner for modern solidstate drive and hard drive based servers.

# Web Wallet
https://github.com/qtumproject/qtum-web-wallet

This is a web based version of the Qtum Electrum wallet. It can not be used for securing the network, staking, and relies on external nodes for transaction and network validation. 

# Dapp Developer Documentation
https://github.com/qtumproject/qtum/wiki

This is our documentation for decentralized application developers. This documentation is used by developers building their own applications on Qtum.
