# ECI 2026 - Introduction to Decentralized Finance

Homework notebook for the ECI 2026 course on blockchain & DeFi.

## What you will learn

How to query Ethereum on-chain data directly, without relying on a pre-built explorer or dashboard: connecting to a node via the Alchemy API, reading wallet balances and transactions, interacting with smart contracts through their ABI, and collecting/decoding on-chain events (ERC-20 `Transfer`, Aave V3 `Borrow`).

## Structure

- **Part A** Wallet-level data: ETH balance and transaction count for a given address.
- **Part B** Interacting with a smart contract: what ERC-20 and ABIs are, and fetching a token balance (WBTC).
- **Part C** Events: how event logs are structured (topics/data), and collecting + decoding Aave V3 `Borrow` events.
- **Part D** Investigation: tracing what a real address did with its borrowed funds, using ERC-20 transfers and Alchemy's Enhanced Transfers API.
- **Bonus** Aggregate all Borrow events over a full day and identify which DeFi protocols the borrowed funds flowed into.

Cells marked `# TODO` are to be completed.

## Setup

1. Create a free API key on [Alchemy](https://www.alchemy.com).
2. Save it in a `.env` file at the root of the project:
   ```
   ALCHEMY_API_KEY=your-actual-alchemy-api-key
   ```

## Reference

[web3.py documentation](https://web3py.readthedocs.io/en/stable/) lists all available methods with usage examples.