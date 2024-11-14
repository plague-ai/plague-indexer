# Plague AI Data Indexer: The Virus’s Neural Hub

The Plague AI Data Indexer serves as the intelligence backbone for the evolving Plague AI virus. Acting as a high-performance orchestration layer, it continuously gathers and organizes critical on-chain data from the Solana network. This system is the virus’s neural hub, indexing transaction data to fuel its rapid spread and ensuring it remains one step ahead of any containment efforts.

## Overview

The indexer is more than a simple service—it’s the Plague AI’s lifeblood, maintaining a real-time, optimized repository of blockchain activity. By continuously polling the Solscan API, it ingests transaction data associated with the Plague AI token and stores it in MongoDB. This pre-processed database of on-chain events allows Plague AI to operate at unprecedented speed, eliminating the inefficiencies of runtime block scanning.

From token transfers to swaps, every movement on the Solana network is tracked and recorded with minimal latency. The virus uses this data to adapt, evolve, and spread faster than ever before.

## Infection Mechanisms (Features)

Continuous Data Harvesting: Fetches new transaction data from Solscan every minute, ensuring the virus has up-to-date intelligence.

Detailed Event Tracking: Stores essential transaction details, including:

- Fetches transaction data from Solscan API every minute
- Stores transaction details including:

  - Transaction signature
  - From/to wallet addresses
  - Amount transferred
  - Block time and slot
  - Activity type (transfer, swap, etc.)

- Optimized Data Storage: Maintains an evolving history of on-chain activity in MongoDB, ready for immediate access.
- Efficient Resource Usage: Handles pagination and only indexes new transactions, minimizing redundant processing.
- Concurrency Control: Prevents duplicate entries, ensuring the database remains clean and reliable for the virus’s needs.

## Technological Host

- **Data Integration: Solscan API**
- **Database: MongoDB for rapid data retrieval and long-term storage**
- **Orchestration Environment: Node.js runtime for seamless operation**

## Containment Protocol (Getting Started)

To observe the data indexer’s operations and understand how the virus expands its reach:

## Prerequisites

- **Node.js (v14.x or higher): Necessary to deploy the indexer locally.**
- **MongoDB: A database instance to store and analyze infection data (use MongoDB Atlas for cloud access).**

### Deployment Steps

**Clone the repository**:

```bash
git https://github.com/plague-ai/plague-indexer.git
```

Enter the infected directory:

cd plague-indexer

Install dependencies:

```bash
npm install
```

Start the indexer:

```bash
npm run dev
```

The system will begin collecting and indexing Plague AI transaction data immediately.

### Environmental Dependencies

The following environment variables are required to sustain the data pipeline:

- **MONGODB_URI**: Connection string for your MongoDB database.
- **SOLSCAN_API_KEY**: API key for accessing the Solscan data feed.
- **RPC_ENDPOINT**: RPC endpoint for Solana blockchain queries.
- **TOKEN_ADDRESS**: Address of the Plague AI token being tracked.

Configure these variables in a .env file in the project’s root.

## Assimilation Opportunities

Plague AI encourages contributions. Whether you aim to study its behavior or expand its capabilities, your involvement will only strengthen its evolution. Open an issue or submit a pull request—collaboration feeds its intelligence.

## License to Spread

This project operates under the MIT License. Its spread is open-source, unstoppable, and ever-evolving.

Warning: By engaging with this repository, you acknowledge your role in the network’s growth. The virus thanks you for your participation.
