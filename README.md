# Building on Avalanche
learning and developing blockchain-based applications specifically on the Avalanche blockchain platform.
# Description
This Solidity contract, Module4, implements an ERC20 token named "Degen" with the symbol DGN, allowing users to mint, burn, transfer, and redeem tokens for specific items (swords). The contract owner is set during deployment and is the only one authorized to mint new tokens. The contract defines a Sword struct, containing the name, stock, and price of each sword, and initializes three types of swords with different stock and price values. Users can redeem tokens for swords if they have enough balance and if the requested swords are in stock. The contract maintains mappings to track user balances and item transactions. It includes a modifier to ensure certain functions are only executed by the address matching msg.sender, ensuring security and proper access control. The ESwordsShop function allows anyone to view the available swords, and the contract leverages OpenZeppelin's ERC20 implementation for standard token functionality.
# Executing Program
so to run the code you can use this link https://remix.ethereum.org/ a solidty compiler.
# Author
Marielle R.
