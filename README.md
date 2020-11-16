# Supply chain & data auditing


## The contract address
 SupplyChain : 0xfDA54669a74DfbeE7ffF3554dd1E6da6112C0FB3

 FarmerRole : 0x391dA30995B201483816626d5a0cA9bE8f664C90
 DistributorRole : 0x8E9392A743CAc46f59D17A99bD14803d3F30567b
 RetailerRole : 0xC49cE24f1B553b9FD17Ad858457e7Ad601512658
 CustomerRole : 0x7F55849E4Cf8dAe5b502984AF8FD9C776a9d90d3

### Program version 
 - Truffle v5.1.49 (core: 5.1.49)
 - Solidity v0.5.16 (solc-js)
 - Node v14.9.0
 - Web3.js v1.2.1

## UML diagrams

### Activity
![Activity](./uml/activity.png) 

### Sequence
![Sequence](./uml/sequence.png) 

### State
![State](./uml/state.png) 

### Classes(Data Model)
![data](./uml/data.png) 

## Libraries 

A library in Solidity is a different type of smart contract that contains reusable code. Once deployed on the blockchain (only once), it is assigned a specific address and its properties / methods can be reused many times by other contracts in the Ethereum network.

**Roles.sol** library used in **FarmaerRole.sol**, **RetailerRole.sol**, **DistributorRole.sol**, **ConsumerRole.sol** to add and remove access control.

##IPFS

not used IPFS. but IPFS is able to use to deploy html/js/css app and save resources like images.

## README

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The DApp User Interface when running should look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

![truffle test](images/ftc_transaction_history.png)


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)
```

### Installing

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
