# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The DApp User Interface when running should look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

![truffle test](images/ftc_transaction_history.png)
### Versions used
Truffle v4.1.14 (core: 4.1.14)
Solidity v0.4.24 (solc-js)
web3 0.20.6 -> To implement the front end as given in the boiler plate code.
### Libraries used
IPFS is not used for this course work
### Deployment in Rinkeby 
Using network 'rinkeby'.

Running migration: 1_initial_migration.js
  Deploying Migrations...
  ... 0x7b0d000faef2b12520e6b2ae500c249792f269783610caf218d4ff47862dc8e9
  Migrations: 0x4a6a821d21fce1beff521d4140a708a91bcf4db4
Saving successful migration to network...
  ... 0x20c95df0d6fb2ee1281c26b30ffda01295be3156ee98ad95ed7f9d8c353e4674
Saving artifacts...
Running migration: 2_deploy_contracts.js
  Deploying FarmerRole...
  ... 0x29cccc35d71b98198ba794e93f327d5cdce37827768d67ca88ea5e94e310ab9c
  FarmerRole: 0x7bcfaed6d13ca8401a46811670a3cbf097d354cd
  Deploying DistributorRole...
  ... 0x9f43432e91209d9cbf2882f3cb79f4bb6ccdce1e84aef895a1758073e3a3f641
  DistributorRole: 0x1f3cbd4286cae5d70abc8c67062b14e6e96f3e38
  Deploying RetailerRole...
  ... 0x37eb84fdbafd883174c1b25b51dc3c436f66127555afa1e0c17e9dbaab94d9e2
  RetailerRole: 0xb5291e27b24139d97ba4fcb7d26c4edf3a000051
  Deploying ConsumerRole...
  ... 0x45d2835ae35ff6e1fb221d7d43de8fa303bff3871d7cd14b55098aa9e28a22ae
  ConsumerRole: 0xeacef214b08468376a0b6d68f9a86638efd62d14
  Deploying SupplyChain...
  ... 0x5d1d822c88981ac836cd34e97b17a52a3c47e29860b31ee16c69e70ef3cedd4a
  SupplyChain: 0x059aa1001e0bebba5eae8fcf0c1ce202a62baa86
Saving successful migration to network...
  ... 0xa4fd3ac8884403eb1ab5471328848379f5fe6f5b9cae02a32b307cbea05079d0
Saving artifacts...
### Contract address on Rinkeby test network:
Transaction hash: 0xa4fd3ac8884403eb1ab5471328848379f5fe6f5b9cae02a32b307cbea05079d0
Contract ID: 0x4a6a821d21fce1beff521d4140a708a91bcf4db4
Rinkeby test Network Link: https://rinkeby.etherscan.io/address/0x4a6a821d21fce1beff521d4140a708a91bcf4db4

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)
```

### Installing

> The starter code is written for **Solidity v0.4.24**. At the time of writing, the current Truffle v5 comes with Solidity v0.5 that requires function *mutability* and *visibility* to be specified (please refer to Solidity [documentation](https://docs.soliditylang.org/en/v0.5.0/050-breaking-changes.html) for more details). To use this starter code, please run `npm i -g truffle@4.1.14` to install Truffle v4 with Solidity v0.4.24. 

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/udacity/nd1309/tree/master/course-5/project-6
```

Change directory to ```project-6``` folder and install all requisite npm packages (as listed in ```package.json```):

```
cd project-6
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```

## Built With

* [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
* [IPFS](https://ipfs.io/) - IPFS is the Distributed Web | A peer-to-peer hypermedia protocol
to make the web faster, safer, and more open.
* [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.


## Authors

See also the list of [contributors](https://github.com/your/project/contributors.md) who participated in this project.

## Acknowledgments

* Solidity
* Ganache-cli
* Truffle
* IPFS
