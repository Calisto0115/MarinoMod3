# MyToken

MyToken is a custom ERC20 token implemented in Solidity.

## Contract Details

The MyToken contract has a private variable owner that stores the address of the contract’s owner. 
The constructor function is called when the contract is deployed. It takes three parameters: the name and symbol of the token,
and the initial supply of tokens. The constructor calls the ERC20 constructor to set the name and symbol, 
and then mints the initial supply of tokens to the address deploying the contract (msg.sender), which is also set as the owner of the contract.


The contract inherits from the OpenZeppelin ERC20 contract and includes additional functionality:

- `mint`: This function allows the contract owner to mint new tokens and assign them to a specific account.
- `burn`: This function allows any account to burn their own tokens, reducing their balance.
- `transfer`: This function allows any account to transfer their tokens to another account. It includes a check to prevent transfers to the zero address.

## Prerequisites

You need to have the following installed:

- Node.js
- npm
- Truffle
- Ganache

## Installation

1. Clone the repository
2. Install the dependencies with `npm install`
3. Compile the contract with `truffle compile`
4. Deploy the contract with `truffle migrate`

## The Contract 

The contract includes a modifier onlyOwner that restricts certain functions to be called only by the owner of the contract. 
If the msg.sender is not the owner, it will revert the transaction. The mint function allows the owner to create new tokens and assign them to a specific account. 
The burn function allows any account to destroy their own tokens, reducing their balance. The transfer function allows any account to send tokens to another account. 
It overrides the transfer function from the ERC20 contract to include a check that prevents tokens from being sent to the zero address (an address with all zeros, which is an invalid address in Ethereum).

## Usage

You can interact with the contract using Truffle console or programmatically with Web3.js or Ethers.js.

## Author

https://academy.metacrafters.io/profile

## License

This project is licensed under the MIT License.
