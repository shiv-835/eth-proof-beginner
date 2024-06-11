# Squish Token (SQH)

This project implements a simple ERC-20-like token named Squish (SQH) using Solidity. It serves as a foundational project for beginners learning about Ethereum and Solidity development offered by Metacrafters.

## Overview

This project originates from the Ethereum Proof Beginner course offered by Metacrafters. The goal is to construct a basic token that mimics the functionality of the ERC-20 standard.

## Features

* **Token Name:** Squish (SQH)
* **Total Supply:** Tracks the overall amount of tokens in circulation.
* **Balances:** Maintains a record of each address's SQH token balance.

## Functionality

**Public Variables:**

* `tokenname`: Stores the official name of the token (Squish).
* `tokenabbreviation`: Represents the abbreviation for the token (SQH).
* `totalsupply`: Tracks the total number of SQH tokens currently in circulation.

**Mapping:**

* `balances`: Utilizes a mapping to efficiently store the balance of each address that holds SQH tokens.

**Functions:**

* **mint(address _address, uint _value):**
    * Adds a specified number of SQH tokens to a given address.
    * Parameters:
        * `_address`: The address to which tokens will be minted.
        * `_value`: The quantity of tokens to be minted.
    * Increases both the total supply and the balance of the specified address.
* **burn(address _address, uint _value):**
    * Removes a specified number of SQH tokens from a given address.
    * Parameters:
        * `_address`: The address from which tokens will be burned.
        * `_value`: The quantity of tokens to be burned.
    * Decreases both the total supply and the balance of the specified address.
    * Implements a check to ensure the address has sufficient tokens for burning.
