# Internet Voting System Using Blockchain 🗳️

A decentralized voting system based on Ethereum blockchain technology.Blockchain is a technology that is rapidly gaining momentum in era of industry 4.0. With high security and transparency provisions, it is being widely used in supply chain management systems, healthcare, payments, business, IoT, voting systems, etc.

## Why do we need it?
Current voting systems like ballot box voting or electronic voting suffer from various security threats such as DDoS attacks, polling booth capturing, vote alteration and manipulation, malware attacks, etc, and also require huge amounts of paperwork, human resources, and time. This creates a sense of distrust among existing systems.

Some of the disadvantages are:

1. Long Queues during elections
2. Security Breaches like data leaks, vote tampering.
3. Lot of paperwork involved, hence less eco-friendly and time-consuming.
4. Difficult for differently-abled voters to reach polling booth.
5. Cost of expenditure on elections is high.



So a gist of advantages are listed below:

You can vote anytime/anywhere (During Pandemics like COVID-19 where it’s impossible to hold elections physically

1. Secure
2. Immutable
3. Faster
4. Transparent


### Requirements

- [Node.js](https://nodejs.org)
- [Truffle](https://www.trufflesuite.com/truffle)
- [Ganache](https://github.com/trufflesuite/ganache-cli)
- [Metamask](https://metamask.io/)

## Setting up the development environment

### Getting the requirements

1. Download and install NodeJS

   > node.js `v14.15.4`

   Download NodeJS from [here](https://nodejs.org/en/download/ "Go to official NodeJS download page.").

1. Install truffle and ganache-cli

   > truffle `v5.2.4`  
   > ganache-cli `v6.12.2`

   ```shell
   npm install -g truffle
   npm install -g ganache-cli
   ```

1. Install metamask browser extension

   Download and install metamask from [here](https://metamask.io/download "Go to official metamask download page.").

### Configuring the project for development

1. Clone this repository

   ```shell
   git clone https://github.com/AbhinavSharma24/BlockVote.git
   cd BlockVote
   ```

1. Run local Ethereum blockchain

   ```shell
   ganache-cli
   ```

   > Note: Do not close `ganache-cli` (the blockchain network needs to be running all the time)

1. Configure metamask on the browser with following details

   New RPC URL: `http://localhost:8545`  
   Chain ID: `1337`

1. Import accounts using private keys from ganache-cli to the metamask extension on the browser
1. Deploy smart contract to the (local) blockchain

   ```shell
   # on the dVoting directory
   truffle migrate
   ```

   > Note: Use `truffle migrate --reset` for redeployments

1. Launch the development server (fronted)

   ```shell
   cd client
   npm install
   npm start
   ```

---
