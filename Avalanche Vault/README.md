Vault Contract README
This README provides an overview of the two Solidity contracts included in this repository: Vault.sol and ERC20.sol. These contracts facilitate the creation of a simple vault for managing ERC20 tokens.

Vault.sol
Vault.sol implements a basic vault contract that allows users to deposit and withdraw ERC20 tokens. It also maintains a record of the token balance and the total supply of shares representing ownership in the vault.

Functions
constructor(address \_token): Initializes the vault with the address of the ERC20 token to be managed.

deposit(uint \_amount): Allows users to deposit ERC20 tokens into the vault, minting shares equivalent to the deposited amount.

withdraw(uint \_shares): Allows users to withdraw ERC20 tokens from the vault, burning shares equivalent to the withdrawn amount.

Variables
token: Immutable variable storing the address of the ERC20 token managed by the vault.

totalSupply: Total supply of shares representing ownership in the vault.

balanceOf: Mapping storing the balance of shares for each account.

ERC20.sol
ERC20.sol is a basic implementation of the ERC20 token standard. It includes functionalities such as transfer, approve, and transferFrom, along with minting and burning tokens.

Functions
transfer(address recipient, uint amount): Allows the sender to transfer tokens to another address.

approve(address spender, uint amount): Approves the spender to spend a certain amount of tokens on behalf of the owner.

transferFrom(address sender, address recipient, uint amount): Allows a spender to transfer tokens on behalf of the owner, given approval.

mint(uint amount): Mints a certain amount of tokens and adds them to the total supply.

burn(uint amount): Burns a certain amount of tokens, reducing the total supply.

Variables
totalSupply: Total supply of the token.

balanceOf: Mapping storing the balance of tokens for each address.

allowance: Mapping storing the allowance granted by token owners to spenders.

name: Name of the token.

symbol: Symbol of the token.

decimals: Number of decimals for the token.

License
Both contracts are released under the MIT License. See the SPDX-License-Identifier tags in the source code for more details.

For further details and usage instructions, refer to the comments in the respective contract files.

Disclaimer
These contracts are provided as educational material and may not be suitable for use in production environments without further auditing and testing. Use them at your own risk.
