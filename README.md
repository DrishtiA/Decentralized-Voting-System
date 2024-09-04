# Decentralized Voting System

## Project Overview
This project is a decentralized voting system built on the Ethereum blockchain. It utilizes **Solidity** smart contracts to ensure secure and transparent voting processes, covering candidate registration, vote counting, and voter authentication. The frontend is developed using **React.js** and interacts with the blockchain via **ethers.js** to provide real-time voting and status updates through **MetaMask**.

## Key Features
- **Decentralized Voting:** Solidity smart contracts manage voting operations, ensuring a tamper-proof election process.
- **Real-Time Interaction:** The React.js frontend allows users to vote, monitor vote counts, and check the remaining voting time.
- **Blockchain Integration:** Deployed on an Ethereum testnet using **Hardhat**, ensuring robust contract execution and testing.
- **MetaMask Integration:** Secure user authentication and transaction signing through MetaMask.
- **Gas Efficiency:** Optimized smart contracts for minimizing transaction costs on the Ethereum network.

## Technology Stack
- **Solidity:** Smart contract development.
- **React.js:** Frontend user interface.
- **ethers.js:** Blockchain interaction from the frontend.
- **Hardhat:** Development and testing of smart contracts.
- **MetaMask:** Ethereum wallet management and transaction signing.

## Installation

After you clone the repository, you need to install the packages using

```shell
npm install
```

You first need to compile the contract and upload it to the blockchain network. Run the following commands to compile and upload the contract.

```shell
npx hardhat compile
npx hardhat run --network volta scripts/deploy.js
```

Once the contract is uploaded to the blockchain, copy the contract address and copy it in the .env file. You can also use another blockchain by writing the blockchain's endpoint in hardhat-config.

Once you have pasted your private key and contract address in the .env file, simply run command

```shell
npm start
```

## Usage

- **Connect Wallet:** Users must connect their MetaMask wallet to participate in the voting process.
- **Register Candidates:** New candidates can be registered by the contract owner.
- **Vote:** Users can cast their votes, with the smart contract ensuring that each user can only vote once.
- **Track Voting:** The application displays real-time voting results and the remaining time until voting ends.
