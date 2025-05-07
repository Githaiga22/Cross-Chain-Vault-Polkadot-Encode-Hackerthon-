# Cross-Chain Identity Vault

A decentralized application that enables users to view and share their identity or reputation data (POAPs, NFTs, badges, messages) across different blockchain networks, specifically from Ethereum/Lisk to Polkadot-based chains.

## 🎯 Project Goal

The primary goal of this project is to create a bridge between different blockchain networks, allowing users to:
- Store and manage their identity data
- Share reputation and achievements across chains
- View and verify cross-chain identity information
- Interact with the system using familiar Ethereum tools (thanks to Moonbeam's EVM compatibility)

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- MetaMask wallet
- Docker (optional, for local development)

### Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd CrossChainVault
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
Create a `.env` file in the root directory with the following variables:
```env
DATABASE_URL=your_database_url
MOONBEAM_RPC_URL=your_moonbeam_rpc_url
PRIVATE_KEY=your_private_key
```

### Running the Application

The application consists of three main components that need to be running simultaneously:

1. Start the backend server:
```bash
npm run dev:server
```

2. Start the frontend client:
```bash
npm run dev:client
```

3. Start the local Hardhat network (for development):
```bash
npx hardhat node
```

The application will be available at:
- Frontend: http://localhost:5173
- Backend API: http://localhost:3000
- Hardhat Network: http://localhost:8545

## 🏗️ Project Structure

```
CrossChainVault/
├── client/           # Frontend React application
├── server/           # Backend Express server
├── contracts/        # Smart contracts
├── scripts/          # Deployment and utility scripts
└── shared/          # Shared types and utilities
```

## 🗺️ Development Roadmap

### Milestone 1: Ecosystem Understanding
- [x] Research Polkadot ecosystem
- [x] Choose Moonbeam as the target chain
- [x] Set up Polkadot.js integration

### Milestone 2: Development Environment
- [x] Set up Node.js environment
- [x] Configure Hardhat for smart contract development
- [x] Initialize React frontend with Vite
- [x] Set up Express backend

### Milestone 3: Smart Contract Development
- [x] Implement identity storage contract
- [x] Add cross-chain data verification
- [x] Deploy to Moonbase Alpha testnet

### Milestone 4: Cross-Chain Integration
- [x] Implement Ethereum data fetching
- [x] Add Lisk integration
- [x] Create data verification system

### Milestone 5: Frontend Development
- [x] Build wallet connection interface
- [x] Create identity display components
- [x] Implement sharing functionality

## 🛠️ Technologies Used

- **Frontend**:
  - React
  - Vite
  - TailwindCSS
  - Polkadot.js
  - Ethers.js

- **Backend**:
  - Node.js
  - Express
  - Drizzle ORM
  - PostgreSQL

- **Smart Contracts**:
  - Solidity
  - Hardhat
  - OpenZeppelin

## 🔒 Security

- Smart contracts are audited and tested
- Cross-chain verification mechanisms
- Secure key management
- Rate limiting and access control

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Contributors

### Core Team
- **Cheryl Owala** ([@cherrypick14](https://github.com/cherrypick14))
  - Polkadot Junior Ambassador (Kisumu)
  - PBA-x Student
  - Rust Developer

- **Allan Robinson** ([@Githaiga22](https://github.com/Githaiga22))
  - Polkadot Junior Ambassador (Kisumu)
  - PBA-x Student
  - Smart Contract Developer

## 🙏 Acknowledgments

- Moonbeam Network for EVM compatibility
- Polkadot.js team for their excellent tools
- OpenZeppelin for secure contract patterns
- Polkadot Blockchain Academy (PBA-x) for the comprehensive blockchain education
- Polkadot Ambassador Program for the opportunity to contribute to the ecosystem 