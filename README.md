
# ERC20 and Vault Contracts

## Overview

This repository contains two smart contracts: an ERC20 token contract and a Vault contract. The ERC20 token contract is a standard implementation of an ERC20 token, which includes functionalities such as minting, transferring, and burning tokens. The Vault contract allows users to deposit and withdraw ERC20 tokens securely.

## Contracts

### 1. ERC20 Token Contract

The ERC20 token contract follows the standard ERC20 interface with additional functionalities for minting and burning tokens.

#### Features

- **Minting**: Allows the contract owner to mint new tokens.
- **Burning**: Allows token holders to burn their own tokens.
- **Standard ERC20 Functions**: `transfer`, `approve`, `transferFrom`, `allowance`, `balanceOf`.

#### Contract Interface

- `mint(address to, uint256 amount)`: Mints new tokens to the specified address.
- `burn(uint256 amount)`: Burns the specified amount of tokens from the caller's account.
- `transfer(address to, uint256 amount)`: Transfers tokens to a specified address.
- `approve(address spender, uint256 amount)`: Approves the specified address to spend the specified amount of tokens on behalf of the caller.
- `transferFrom(address from, address to, uint256 amount)`: Transfers tokens from one address to another using the allowance mechanism.
- `allowance(address owner, address spender)`: Returns the amount of tokens that an owner has allowed a spender to use.
- `balanceOf(address account)`: Returns the token balance of the specified address.

### 2. Vault Contract

The Vault contract allows users to securely deposit and withdraw ERC20 tokens. 

#### Features

- **Deposit**: Users can deposit ERC20 tokens into the Vault.
- **Withdraw**: Users can withdraw their deposited tokens from the Vault.
- **Balance Tracking**: Keeps track of individual user balances within the Vault.

#### Contract Interface

- `deposit(uint256 amount)`: Allows users to deposit a specified amount of ERC20 tokens into the Vault.
- `withdraw(uint256 amount)`: Allows users to withdraw a specified amount of their deposited tokens from the Vault.
- `balanceOf(address account)`: Returns the balance of the specified address within the Vault.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
