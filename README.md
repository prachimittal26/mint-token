# mint-token
# ERC20 Token Project README

## Overview
This project demonstrates the creation and deployment of a custom ERC20 token on the Ethereum blockchain. The token contract includes functionalities for minting, transferring, and burning tokens.

## Contract Details
The ERC20 token contract (`MyToken.sol`) is deployed with the following details:

- **Name**: MyToken
- **Symbol**: MTK
- **Initial Supply**: 1000 MTK tokens
- **Owner**: The deployer of the contract is the initial owner of all tokens.

## Functionalities
### 1. Minting Tokens
The contract owner (deployer) can mint new tokens and allocate them to a specified address.

## Transfer Function

The `transfer` function allows any user to transfer their tokens to another address.

### Function Definition

```solidity
function transfer(address recipient, uint256 amount) public override returns (bool)
Function Signature:

solidity
Copy code
function transfer(address to, uint256 amount) public returns (bool);
3. Burning Tokens
Any token holder can burn (destroy) a specific amount of their own tokens.

Function Signature:


function burn(uint256 amount) public;
Deployment
The contract is deployed using Hardhat, ensuring proper testing and deployment practices. Deployment scripts and configuration are included in the project directory (scripts/deploy.js).

To deploy the contract locally or on a test network, follow these steps:

Install dependencies: npm install
Compile contracts: npx hardhat compile
Deploy contract: npx hardhat run scripts/deploy.js --network <network-name>
Replace <network-name> with your desired network configuration (e.g., localhost for local testing, rinkeby for Ethereum testnet).

Testing
The project includes unit tests to ensure the functionality and security of the ERC20 token contract. Tests cover scenarios such as minting, transferring, burning, and ownership checks.

To run tests:

bash
Copy code
npx hardhat test
Contributors
Your Name
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
OpenZeppelin for providing the ERC20 implementation used in this project.
Ethereum and the developer community for valuable resources and support.
less
Copy code

### Notes:
- Replace placeholders (`<network-name>`, `Your Name`, `your-username`) with actual details relevant to your project.
- Ensure to update the `LICENSE` file if you choose a different license than MIT.


