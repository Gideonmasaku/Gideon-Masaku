# BIT_KCA Smart Contract

## Description
`BIT_KCA` is a simple Ethereum smart contract written in Solidity. This contract allows users to store a numeric value and a message. The number can be increased or decreased, and the message can be updated. The contract is designed to help demonstrate basic Solidity concepts such as state variables, functions, and constructors.

## Prerequisites
- **Solidity 0.8.26**: This contract is designed for Solidity version 0.8.26.
- **Ethereum Development Environment**: You can use tools like [Remix](https://remix.ethereum.org/), [Truffle](https://www.trufflesuite.com/), or [Hardhat](https://hardhat.org/) to deploy and interact with this contract.

## Installation and Deployment
1. **Clone the repository** or copy the code into a Solidity-compatible IDE like Remix.
2. **Compile the contract** using Solidity compiler version 0.8.26 or higher.
3. **Deploy the contract**:
   - Specify the initial value for `number` and an initial message in the deployment parameters.
   - Deploy the contract to your desired Ethereum network.

## Contract Overview
### State Variables
- `uint256 private number`: Stores a numeric value that can be increased or decreased.
- `string public message`: Stores a public message string that can be updated by the contract owner.

### Constructor
The constructor initializes `number` and `message`:
```solidity
constructor(uint256 startingpoint, string memory _startingMessage) {
    number = startingpoint;
    message = _startingMessage;
}
