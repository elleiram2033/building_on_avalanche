# Module4 Building On Avalanche
This Solidity smart contract, named Module4, is an ERC20 token with additional functionalities for managing a collection of swords and allowing users to redeem these swords by burning the token.

## Overview

The contract inherits from ERC20 and includes the following features:

- **ERC20 Token**: Standard ERC20 functionality for token management.
- **Swords Collection**: A collection of swords with details such as name, stock, and price.
- **Redeem Functionality**: Users can redeem swords by burning the token corresponding to the sword's price.
- **Minting**: Only the contract owner can mint new tokens to designated addresses.
- **Burning**: Users can burn their tokens.
- **Transfers**: Allows token transfers between addresses.

## Functionality

### Constructor

Upon deployment (`constructor`), the contract initializes with a predefined token name ("Degen") and symbol ("DGN"), and sets up an initial collection of swords.

### Sword Struct

The `Sword` struct defines attributes for each sword including `name`, `stock`, and `price`.

### Redeem Function

The `Redeem` function allows users to redeem a specific type of sword by burning the corresponding amount of tokens. It checks if the requested sword type exists, if the user has sufficient tokens, and if there is enough stock available.

### Additional Functions

- **ESwordsShop**: Returns an array of all available swords.
- **Mint**: Allows the contract owner to mint new tokens to a specified address.
- **Burn**: Allows any user to burn their own tokens.
- **Transfers**: Allows token transfers between addresses.

### Modifiers

- **onlySender**: Restricts access to functions based on the caller's address, ensuring only the contract owner can execute certain operations.

## Usage

1. **Deploying the Contract**: Deploy the contract on a supported Ethereum environment using Remix or another IDE.
2. **Interacting with the Contract**: Use the provided functions (`Redeem`, `Mint`, `Burn`, `Transfers`) to manage tokens and swords.

## Development Environment

This contract was developed and tested using Remix IDE (remix.ethereum.org).

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.

