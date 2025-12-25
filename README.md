# Crimson Tide (Built for Base)

Crimson Tide is a read-only onchain tool that helps developers validate network identity, inspect balances, retrieve block information, and explore smart contracts deployed on Base networks, leveraging Coinbase Wallet SDK and Base RPC endpoints for verification through Basescan.

## Features

- **Coinbase Wallet SDK** integration for seamless wallet access via EIP-1193  
- **Base Mainnet (8453)** and **Base Sepolia (84532)** chainId validation  
- **Network snapshot functionality**, including block number, gas usage, and gas price  
- **Address inspection**, showing balance, transaction count, and bytecode presence  
- **ERC-20 token inspection**, fetching token metadata, total supply, and holder balances  
- **Basescan verification links** to check deployed contracts and addresses independently  

---

## Repository Structure

- **app.crimson-tide.ts**  
  Main script that connects to Coinbase Wallet and interacts with the Base RPC, performing read-only queries.

- **contracts/**  
  Solidity contracts deployed on Base Sepolia for testnet validation:
  - `arrays.sol` — minimal contract for deployment validation  

- **package.json**  
  Dependency manifest that includes references to Base and Coinbase SDKs and libraries.

- **README.md**  
  Full documentation providing instructions for setting up and using the repository.

---

## Supported Networks

- **Base Sepolia**  
  ChainId (decimal): 84532  
  Explorer: [sepolia.basescan.org](https://sepolia.basescan.org)  

- **Base Mainnet**  
  ChainId (decimal): 8453  
  Explorer: [basescan.org](https://basescan.org)

---

## Tooling & Dependencies

This repository integrates the following official tools:
- **Coinbase Wallet SDK** for wallet connection  
- **OnchainKit** for interacting with Base-native primitives  
- **Viem** for typed RPC communication with Base  
- Direct dependencies from Base and Coinbase GitHub repositories  

---

## License

MIT License

Copyright (c) 2025 YOUR_NAME

## Author contacts

GitHub: [https://github.com/your-handle](https://github.com/laugh-detours)  

Email: laugh.detours.0v@icloud.com

## Testnet Deployment (Base Sepolia)

As part of pre-production validation, one or more contracts may be deployed to the Base Sepolia test network to confirm correct behavior and tooling compatibility.

**Network**: Base Sepolia  
**ChainId (decimal)**: 84532  
**Explorer**: [sepolia.basescan.org](https://sepolia.basescan.org)

**Contract arrays.sol address**:  
0xdbF7C9Ace11c4467A350C19d936166b47604Fe0C

**Deployment and verification**:
- [Deployment link](https://sepolia.basescan.org/address/0xdbF7C9Ace11c4467A350C19d936166b47604Fe0C)
- [Code verification](https://sepolia.basescan.org/0xdbF7C9Ace11c4467A350C19d936166b47604Fe0C/0#code)

These deployments will be used to validate Base tooling and network compatibility before moving to Mainnet.
