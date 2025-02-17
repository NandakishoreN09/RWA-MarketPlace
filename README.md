
# Real World Assets (RWA) Marketplace

A decentralized marketplace for tokenizing and trading real-world assets on the blockchain. Built with Next.js, TypeScript, and Ethereum.

## Features

- 🏠 Tokenize real-world assets (Real Estate, Art, Collectibles)
- 💰 Buy and sell assets using cryptocurrency
- 🔐 Secure ownership transfer on the blockchain
- 👛 Wallet integration with Web3
- 🎨 Modern UI with shadcn/ui components
- 1️⃣ 1% platform fee on transactions

## Tech Stack

- **Frontend**
  - Next.js 14 (App Router)
  - TypeScript
  - Tailwind CSS
  - shadcn/ui
  - wagmi/viem (Web3 Integration)
  - RainbowKit (Wallet Connection)

- **Blockchain**
  - Solidity (Smart Contracts)
  - Hardhat (Development Environment)
  - Sepolia Testnet

## Getting Started

### Prerequisites

- Node.js 18+
- npm/yarn
- MetaMask or any Web3 wallet

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/rwa-marketplace.git
cd rwa-marketplace
```

2. Install dependencies
```bash
# Install frontend dependencies
cd frontend
npm install

# Install blockchain dependencies
cd ../
npm install
```

3. Set up environment variables
```bash
# Frontend (.env.local)
NEXT_PUBLIC_PROJECT_ID=your_wallet_connect_project_id
NEXT_PUBLIC_MARKETPLACE_ADDRESS=your_contract_address

# Blockchain (.env)
PRIVATE_KEY=your_private_key
SEPOLIA_RPC_URL=your_sepolia_rpc_url
ETHERSCAN_API_KEY=your_etherscan_api_key
```

4. Run the development server
```bash
# Run frontend
cd frontend
npm run dev

# Run local blockchain
npx hardhat node
```

### Smart Contract Deployment

1. Compile contracts
```bash
npx hardhat compile
```

2. Deploy to Sepolia testnet
```bash
npx hardhat run scripts/deploy.ts --network sepolia
```

3. Verify contract
```bash
npx hardhat verify --network sepolia <CONTRACT_ADDRESS>
```

## Project Structure

```
real-world-marketplace/
├── frontend/               # Next.js frontend application
│   ├── src/
│   │   ├── app/           # Next.js app router pages
│   │   ├── components/    # UI components
│   │   ├── hooks/         # Custom hooks
│   │   └── providers/     # Context providers
├── contracts/             # Smart contracts
├── scripts/              # Deployment scripts
└── test/                 # Contract tests
```

## Features in Development

- [ ] IPFS integration for asset images
- [ ] Advanced search and filtering
- [ ] Price history charts
- [ ] Auction functionality
- [ ] Multi-signature ownership
- [ ] Asset fractional ownership
- [ ] Mobile app

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Built With

- [Ethereum](https://ethereum.org/)
- [Next.js](https://nextjs.org/)
- [shadcn/ui](https://ui.shadcn.com/)
- [RainbowKit](https://www.rainbowkit.com/)
- [Wagmi](https://wagmi.sh/)
