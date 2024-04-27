# CustomToken Contract

This Solidity smart contract implements a custom ERC20 token with additional functionality such as minting, burning, and transferring tokens.

## Overview

The `CustomToken` contract is based on the ERC20 standard and extends functionality from the OpenZeppelin `ERC20` and `Ownable` contracts. It allows for the creation of a custom token with a specified name, symbol, initial supply, and owner.

### Features

- Customizable token name and symbol
- Initial token supply specified during deployment
- Ownership functionality provided by the `Ownable` contract
- Minting of new tokens by the contract owner
- Burning of tokens by any token holder
- Transfer of tokens between addresses

## Deployment

The contract can be deployed to any Ethereum-compatible blockchain network. During deployment, the following parameters must be provided:

- `_name`: The name of the token.
- `_symbol`: The symbol of the token.
- `_initialSupply`: The initial supply of tokens to be minted.
- `_initialOwner`: The address that will initially own all tokens and have administrative privileges.

## Usage

Once deployed, the contract provides the following functions for interacting with the token:

- `mintTokens`: Mint new tokens and assign them to a specified address. Only the contract owner can call this function.
- `burnTokens`: Burn a specified amount of tokens from the caller's balance.
- `transferTokens`: Transfer tokens from the caller's address to a specified recipient.
