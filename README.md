# Cross-Chain Identity Vault   [👉website](https://cross-chain-vault.onrender.com)

<div align="center">
  <img src="generated-icon.png" alt="Cross-Chain Identity Vault Logo" width="200"/>
  <br/>
  <p><em>Bridge your identity across blockchain networks</em></p>
</div>

## 📖 Overview

Cross-Chain Identity Vault is a decentralized application that enables users to view and share their identity or reputation data (POAPs, NFTs, badges, messages) across different blockchain networks, specifically from Ethereum/Lisk to Polkadot-based chains. Built by Polkadot Junior Ambassadors and PBA-x students, this project demonstrates the power of cross-chain interoperability.

## 🌟 Features

- **Cross-Chain Identity Management**
  - Store and manage identity data across chains
  - Share reputation and achievements
  - View and verify cross-chain identity information

- **Multi-Chain Support**
  - Ethereum integration
  - Lisk compatibility
  - Polkadot/Moonbeam ecosystem

- **User-Friendly Interface**
  - Modern, responsive design
  - Real-time network status
  - Wallet connection management
  - Transaction history

- **Security Features**
  - Smart contract audits
  - Cross-chain verification
  - Secure key management
  - Rate limiting

## 🏗️ Architecture

### Tech Stack

#### Frontend
- React with TypeScript
- Vite for build tooling
- TailwindCSS for styling
- Polkadot.js for chain interaction
- Ethers.js for Ethereum integration

#### Backend
- Node.js with Express
- TypeScript
- Drizzle ORM
- PostgreSQL database
- WebSocket support

#### Smart Contracts
- Solidity
- Hardhat development environment
- OpenZeppelin contracts
- Moonbeam/Moonbase Alpha deployment

### Project Structure
```
CrossChainVault/
├── client/           # Frontend React application
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── hooks/        # Custom React hooks
│   │   ├── pages/        # Page components
│   │   └── utils/        # Utility functions
├── server/           # Backend Express server
│   ├── src/
│   │   ├── controllers/  # Route controllers
│   │   ├── models/       # Data models
│   │   ├── routes/       # API routes
│   │   └── services/     # Business logic
├── contracts/        # Smart contracts
│   ├── IdentityVault.sol
│   └── CrossChainBridge.sol
├── scripts/          # Deployment and utility scripts
└── shared/          # Shared types and utilities
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- MetaMask wallet
- Docker (optional, for local development)
- PostgreSQL database

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/CrossChainVault.git
cd CrossChainVault
```

2. Install dependencies:
```bash
# Install root dependencies
npm install

# Install client dependencies
cd client && npm install

# Install server dependencies
cd ../server && npm install
```

3. Set up environment variables:
Create `.env` files in the root, client, and server directories:

```env
# Root .env
PRIVATE_KEY=your_private_key
MOONBEAM_RPC_URL=your_moonbeam_rpc_url

# Client .env
VITE_API_URL=http://localhost:3000
VITE_WS_URL=ws://localhost:3000

# Server .env
DATABASE_URL=your_database_url
PORT=3000
```

### Development

1. Start the development server:
```bash
# Terminal 1 - Backend
npm run dev:server

# Terminal 2 - Frontend
npm run dev:client

# Terminal 3 - Hardhat Network
npx hardhat node
```

2. Access the application:
- Frontend: http://localhost:5173
- Backend API: http://localhost:3000
- Hardhat Network: http://localhost:8545

### Production Deployment

1. Build the application:
```bash
# Build client
cd client && npm run build

# Build server
cd ../server && npm run build
```

2. Deploy to your preferred hosting service:
- Frontend: Vercel, Netlify, or similar
- Backend: Render, Heroku, or similar
- Database: Managed PostgreSQL service

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `DATABASE_URL` | PostgreSQL connection string | Yes |
| `MOONBEAM_RPC_URL` | Moonbeam network RPC URL | Yes |
| `PRIVATE_KEY` | Wallet private key for deployment | Yes |
| `PORT` | Server port | No (default: 3000) |

### Network Configuration

The application is configured to work with:
- Moonbase Alpha (testnet)
- Ethereum Goerli (testnet)
- Local Hardhat network (development)

## 🧪 Testing

```bash
# Run smart contract tests
npx hardhat test

# Run frontend tests
cd client && npm test

# Run backend tests
cd server && npm test
```

## 📚 API Documentation

### Authentication Endpoints

```http
POST /api/auth/connect
Content-Type: application/json

{
  "address": "0x...",
  "signature": "..."
}
```

### Identity Endpoints

```http
GET /api/identity/:address
GET /api/identity/:address/reputation
POST /api/identity/share
```

## 👥 Contributors

### Core Team
- **Cheryl Owala** ([@cherrypick14](https://github.com/cherrypick14))
  - Polkadot Junior Ambassador (Kisumu)
  - PBA-x Student
  - Smart Contract Developer

- **Allan Robinson** ([@Githaiga22](https://github.com/Githaiga22))
  - Polkadot Junior Ambassador (Kisumu)
  - PBA-x Student
  - Full Stack Developer

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines

- Follow the TypeScript style guide
- Write tests for new features
- Update documentation as needed
- Use conventional commits

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Moonbeam Network for EVM compatibility
- Polkadot.js team for their excellent tools
- OpenZeppelin for secure contract patterns
- Polkadot Blockchain Academy (PBA-x) for the comprehensive blockchain education
- Polkadot Ambassador Program for the opportunity to contribute to the ecosystem

## 🔗 Links

- [Live Demo](https://cross-chain-vault.onrender.com)


## Documentation

For Documentation, please:
1. Check the [pitch-deck](https://www.canva.com/design/DAGmyhUHdDI/qgTgcyvoSysGa6wJj7BxQw/view?utm_content=DAGmyhUHdDI&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hd3862c7146)
