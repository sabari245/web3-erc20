## Fungible Token Implementation

In the provided workspace, there is a simple implementation of custom fungible tokens using ERC20 contracts and an ownable proxy contract. This implementation allows you to create and manage your own fungible tokens on the Ethereum blockchain. Let's break down the components and how they work:

### ERC20 Contracts

The ERC20 standard is a widely adopted Ethereum token standard that defines a set of rules and functions for creating and managing fungible tokens. In the provided workspace, there are two ERC20 contracts: `CustomToken` and `CustomTokenProxy`.

1. **CustomToken**: This contract implements the core functionality of an ERC20 token. It includes functions to mint new tokens, transfer tokens between addresses, check balances, and approve spending on behalf of an address.

2. **CustomTokenProxy**: This contract acts as an **ownable** proxy for the `CustomToken` contract. It means that the owner of the proxy contract has the ability to upgrade the functionality of the `CustomToken` contract. This allows for flexibility in case improvements or bug fixes are needed in the token contract while keeping the token address consistent.

### How to Use

To use this implementation, you would need to:

1. Deploy the `CustomTokenProxy` contract: This contract serves as the entry point for interacting with the ERC20 token functionality.

2. Interact with the `CustomToken` through the proxy: After deploying the proxy contract, you would use it to mint new tokens, transfer tokens between addresses, and perform other ERC20 token operations.

3. Ownership and Upgrades: The owner of the proxy contract has the ability to upgrade the `CustomToken` contract. This can be useful for making improvements or fixing issues in the token contract while maintaining the same token address.

### Getting Started

This entire workspace is downloaded from remix IDE. so kindly re-upload it to remix before using or this could also be deployed with the help of hardhat. refer hardhat documentation for further information

### DO NOT USE THIS IN PRODUCTION

This is only done as a part of Metacrafters Project. **PLEASE DO NOT USE THIS IN PRODUCTION OR DEVELOPMENT**. This code might
contain critical vulnerabilities, so do not use this for production or development under any circumstances
