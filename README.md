# Plague Ai Data Indexer

This service indexes transaction data for the Plague Ai project

## Overview

The indexer serves as a high-performance data orchestration layer, connecting to MongoDB and continuously polling the Solscan API to fetch and store transaction data related to the Plague Ai token. By maintaining an optimized database of pre-processed on-chain events, it eliminates the need for resource-intensive block scanning at runtime, enabling lightning-fast web application performance. The system tracks token transfers, swaps and other on-chain activities with minimal latency.

## Features

- Fetches transaction data from Solscan API every minute
- Stores transaction details including:
  - Transaction signature
  - From/to addresses
  - Amount transferred
  - Block time and slot
  - Activity type
- Maintains transaction history in MongoDB
- Handles pagination and only indexes new transactions
- Prevents duplicate processing with concurrency control

## Getting Started

### Prerequisites

- **Node.js** (v14.x or higher)
- **MongoDB** database access (you can use MongoDB Atlas for a cloud database)

### Installation

**Clone the repository**:

```bash
git https://github.com/plague-ai/plague-indexer.git
cd plague-indexer
npm install
npm run dev
```

### Environmental Variables

The project requires the following environment variables:

- **MONGODB_URI**
- **SOLSCAN_API_KEY**
- **RPC_ENDPOINT**
- **TOKEN_ADDRESS**

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
