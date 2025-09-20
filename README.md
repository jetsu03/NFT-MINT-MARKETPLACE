# Advanced NFT Marketplace DApp

🚀 A comprehensive blockchain-based NFT marketplace built with Next.js 13, Solidity, and modern Web3 technologies. This decentralized application empowers creators and collectors to mint, trade, and manage unique digital assets with multi-token payment support and advanced analytics.


## 🌟 Features

### 🎨 Core Marketplace Functionality
- **Multi-Token Payments**: Support for ETH, USDC, and USDT transactions
- **NFT Minting**: Create and tokenize digital assets with custom metadata
- **Marketplace Trading**: Seamless buying and selling with instant transactions
- **Automated Royalties**: Built-in creator compensation for secondary sales
- **Price Management**: Dynamic listing price updates and management
- **Portfolio Tracking**: Comprehensive asset management and analytics

### 🎯 Advanced Features
- **Multi-Chain Support**: Deploy on Ethereum and compatible blockchain networks
- **Real-Time Analytics**: Market insights and performance tracking
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Dark/Light Theme**: Customizable UI with system preference detection
- **IPFS Storage**: Decentralized asset storage via Pinata integration
- **Wallet Integration**: Support for MetaMask, WalletConnect, and other Web3 wallets


## 🛠️ Technology Stack

### Frontend
- **Next.js 13** - React framework with App Router
- **React 18** - Modern component-based architecture
- **Tailwind CSS** - Utility-first styling framework
- **Framer Motion** - Smooth animations and transitions
- **TypeScript** - Type-safe development experience

### Blockchain & Web3
- **Solidity** - Smart contract development
- **Wagmi** - React hooks for Ethereum interactions
- **RainbowKit** - Beautiful wallet connection interfaces
- **Viem** - TypeScript Ethereum library
- **Ethers.js** - Blockchain interaction utilities

### Infrastructure
- **IPFS** - Decentralized file storage
- **Pinata** - IPFS pinning and gateway services
- **Alchemy** - Blockchain infrastructure and APIs
- **MongoDB/PostgreSQL** - Off-chain data management

## 🚀 Quick Start
# Advanced NFT Marketplace DApp

🚀 A comprehensive blockchain-based NFT marketplace built with Next.js 13, Solidity, and modern Web3 technologies. This decentralized application empowers creators and collectors to mint, trade, and manage unique digital assets with multi-token payment support and advanced analytics.

![NFT Marketplace Banner](https://www.daulathussain.com/wp-content/uploads/2025/08/Create-Deploy-an-Advanced-NFT-Marketplace-DApp-Next.js-Solidity-Full-Web3-Project-Any-Blockchain.jpg)

## 🌟 Features

### 🎨 Core Marketplace Functionality
- **Multi-Token Payments**: Support for ETH, USDC, and USDT transactions
- **NFT Minting**: Create and tokenize digital assets with custom metadata
- **Marketplace Trading**: Seamless buying and selling with instant transactions
- **Automated Royalties**: Built-in creator compensation for secondary sales
- **Price Management**: Dynamic listing price updates and management
- **Portfolio Tracking**: Comprehensive asset management and analytics

### 🎯 Advanced Features
- **Multi-Chain Support**: Deploy on Ethereum and compatible blockchain networks
- **Real-Time Analytics**: Market insights and performance tracking
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Dark/Light Theme**: Customizable UI with system preference detection
- **IPFS Storage**: Decentralized asset storage via Pinata integration
- **Wallet Integration**: Support for MetaMask, WalletConnect, and other Web3 wallets

### 🔒 Security & Performance
- **Smart Contract Security**: Audited contracts with OpenZeppelin libraries
- **Gas Optimization**: Efficient transaction processing with cost reduction
- **Server-Side Rendering**: Improved SEO and faster page loads
- **Permanent Storage**: IPFS-based decentralized asset preservation

## 🛠️ Technology Stack

### Frontend
- **Next.js 13** - React framework with App Router
- **React 18** - Modern component-based architecture
- **Tailwind CSS** - Utility-first styling framework
- **Framer Motion** - Smooth animations and transitions
- **TypeScript** - Type-safe development experience

### Blockchain & Web3
- **Solidity** - Smart contract development
- **Wagmi** - React hooks for Ethereum interactions
- **RainbowKit** - Beautiful wallet connection interfaces
- **Viem** - TypeScript Ethereum library
- **Ethers.js** - Blockchain interaction utilities

### Infrastructure
- **IPFS** - Decentralized file storage
- **Pinata** - IPFS pinning and gateway services
- **Alchemy** - Blockchain infrastructure and APIs
- **MongoDB/PostgreSQL** - Off-chain data management

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ installed
- Yarn or npm package manager
- Web3 wallet (MetaMask recommended)
- Git for version control

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/nft-marketplace-dapp.git
   cd nft-marketplace-dapp
   ```

2. **Environment Configuration**
   
   Create `.env.local` file in the root directory and configure the following:

   **Step 2.1: Setup WalletConnect Project ID**
   - Visit [Reown WalletConnect](https://docs.reown.com/cloud/relay)
   - Create a new project and get your Project ID
   - Add to `.env.local`:
   ```env
   NEXT_PUBLIC_WALLET_CONNECT_PROJECT_ID=your_reown_project_id
   ```

   **Step 2.2: Setup Pinata IPFS**
   - Visit [Pinata Cloud](https://pinata.cloud/)
   - Create account and generate API Key (JWT token)
   - Add to `.env.local`:
   ```env
   NEXT_PUBLIC_PINATA_JWT=your_pinata_jwt_token
   NEXT_PUBLIC_PINATA_GATEWAY_URL=https://gateway.pinata.cloud/ipfs/
   ```

   **Step 2.3: Setup Formspree**
   - Visit [Formspree](https://formspree.io/)
   - Create account and get your Form ID
   - Add to `.env.local`:
   ```env
   NEXT_PUBLIC_FORMSPREE_API=your_formspree_form_id
   ```

3. **Smart Contract Deployment**
   
   **Step 3.1: Setup Local Blockchain**
   ```bash
   # Navigate to web3 directory
   cd web3
   
   # Downgrade to Node.js version 20.19.4
   nvm use 20.19.4
   # or install if not available
   nvm install 20.19.4
   
   # Install dependencies
   npm install
   ```

   **Step 3.2: Start Local Blockchain**
   ```bash
   # Start local blockchain node
   npm run node
   ```
   This will generate account IDs and private keys. Use one of these accounts to import into MetaMask wallet.

   **Step 3.3: Deploy Smart Contracts**
   ```bash
   # In another terminal, navigate to web3 directory
   cd web3
   
   # Compile smart contracts
   npm run compile
   
   # Deploy contracts to local blockchain
   npm run deploy
   ```
   Save the deployed contract addresses from the deployment output.

4. **Frontend Setup**
   ```bash
   # Navigate back to root directory
   cd ..
   
   # Install frontend dependencies
   npm install
   ```

5. **Update Environment Variables**
   
   Add the deployed contract addresses to `.env.local`:
   ```env
   # App Configuration
   NEXT_PUBLIC_APP_NAME=NFT Marketplace DApp
   NEXT_PUBLIC_WALLET_CONNECT_PROJECT_ID=your_reown_project_id
   
   # Smart Contract Addresses (from deployment)
   NEXT_PUBLIC_CONTRACT_ADDRESS=deployed_marketplace_contract_address
   NEXT_PUBLIC_USDC_ADDRESS=deployed_usdc_contract_address
   NEXT_PUBLIC_USDT_ADDRESS=deployed_usdt_contract_address
   
   # IPFS Configuration
   NEXT_PUBLIC_PINATA_JWT=your_pinata_jwt_token
   NEXT_PUBLIC_PINATA_GATEWAY_URL=https://gateway.pinata.cloud/ipfs/
   
   # Formspree Configuration
   NEXT_PUBLIC_FORMSPREE_API=your_formspree_form_id
   
   # Local Network Configuration
   NEXT_PUBLIC_CHAIN_ID=1337
   NEXT_PUBLIC_RPC_URL=http://127.0.0.1:8545
   ```

6. **Start Development Server**
   ```bash
   npm run dev
   ```

7. **Access Application**
   
   Navigate to [http://localhost:3000](http://localhost:3000) and connect your MetaMask wallet using the account created in Step 3.2.

## 🎯 Usage Guide

### For Users

1. **Connect Wallet**
   - Click "Connect Wallet" in the header
   - Select your preferred wallet provider
   - Approve connection request

2. **Browse Marketplace**
   - Explore featured NFTs on homepage
   - Use filters and search functionality
   - View detailed NFT information

3. **Purchase NFTs**
   - Select desired NFT
   - Choose payment token (ETH, USDC, USDT)
   - Confirm transaction in wallet

4. **Create NFTs**
   - Navigate to "Create" page
   - Upload digital asset
   - Add metadata and properties
   - Set initial price and royalties
   - Mint NFT on blockchain

5. **Manage Portfolio**
   - View owned NFTs in "My NFTs"
   - List NFTs for sale
   - Track sales and royalties
   - Update listing prices
