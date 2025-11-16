# AgriTrace DAO

## 📄 Project Overview

AgriTrace DAO is a blockchain-powered agricultural supply chain traceability platform built on Algorand. The project revolutionizes food traceability by creating transparent, verifiable records of every product's journey from farm to fork.

**Key Features:**
- 🌾 **Farmer Dashboard**: Register crops, upload certifications, and generate unique QR codes for product batches
- 🔍 **Consumer Verification**: Scan QR codes to view complete product history, eco-ratings, and origin information
- 🗳️ **DAO Governance**: Community-driven decision making for platform improvements and sustainability initiatives
- 🎁 **Rewards System**: Earn ASA tokens for participating in the ecosystem and making sustainable choices
- 🌱 **Carbon-Negative**: Built on Algorand's environmentally sustainable blockchain

**Purpose:**
AgriTrace DAO empowers farmers with fair market access, protects consumers with product transparency, and promotes sustainable agriculture through decentralized governance. All product data is immutably stored on Algorand blockchain, ensuring complete traceability and trust.

---

## ⚙️ Setup & Installation

### Prerequisites
- Node.js (v18 or higher)
- Python 3.10+
- AlgoKit CLI
- Algorand wallet (Pera Wallet recommended)

### Local Setup

```bash
# Clone the repository
git clone https://github.com/shariya1612/AgriTraceDAO-HackSeries-Algofinity.git
cd AgriTraceDAO-HackSeries-Algofinity

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Add your contract app ID and other config

# Run development server
npm run dev

# Build for production
npm run build
```

---

## 🔗 Deployed Contract & Asset Links

### Smart Contracts on Algorand TestNet

**Main Application Contract:**
- **App ID**: `748497472`
- **Verification Link**: [View on Lora](https://lora.algokit.io/testnet/application/748497472)
Check the box storages

---

## 🧠 Architecture & Components

### System Architecture

```
┌─────────────────┐         ┌──────────────────┐         ┌─────────────────┐
│   Frontend      │         │    Backend       │         │   Algorand      │
│   (Next.js)     │◄───────►│    (Python)      │◄───────►│   Blockchain    │
│                 │         │                  │         │                 │
│  - Farmer UI    │         │  - API Server    │         │  - Smart        │
│  - Consumer UI  │         │  - Web3          │         │    Contracts    │
│  - DAO Portal   │         │    Integration   │         │  - ASA Tokens   │
└─────────────────┘         └──────────────────┘         └─────────────────┘
```

### Core Components

#### 1. **Smart Contract Layer**
- **Batch Registration Contract**: Stores crop batch details (batch ID, farmer info, crop type, location, certifications, harvest date)
- **Governance Contract**: Manages DAO proposals and voting mechanisms
- **Token Contract**: ASA tokens for rewards and incentives
- **Verification Logic**: Ensures data integrity and authenticity

#### 2. **Backend Service**
- **Language**: Python with Flask/FastAPI
- **Algorand SDK**: py-algorand-sdk for blockchain interactions
- **Database**: PostgreSQL for off-chain indexing
- **Functions**:
  - Register farmers and batches
  - Query blockchain for batch verification
  - Handle wallet connections
  - Manage DAO proposals and voting
  - Process token rewards

#### 3. **Frontend Application**
- **Framework**: Next.js with TypeScript
- **Styling**: Tailwind CSS
- **Web3**: @algorandfoundation/algokit-utils, @perawallet/connect
- **Features**:
  - **Farmer Dashboard**: Multi-step registration form, batch management, QR code generation
  - **Consumer Scanner**: QR code scanning, product history viewer, sustainability ratings
  - **DAO Governance**: Proposal listing, voting interface, member statistics
  - **Wallet Integration**: Pera Wallet connect/disconnect

#### 4. **Data Flow**
1. Farmer registers batch → Backend validates → Smart contract stores on-chain → QR code generated
2. Consumer scans QR → Backend queries blockchain → Display verified product data
3. Community member votes → Frontend signs transaction → Governance contract updates vote count

---

## 🌐 Deployed Application

**Live Frontend**: [https://agritrace-wheat.vercel.app/](https://agritrace-wheat.vercel.app/)

**Available Pages:**
- `/` - Home page with project overview
- `/farmers` - Farmer registration and dashboard
- `/consumers` - Product verification scanner
- `/dao` - Governance portal with active proposals
- `/about` - Mission, values, and technology information

---

## 🚀 Key Technologies

- **Blockchain**: Algorand (TestNet)
- **Smart Contracts**: PyTeal / Python
- **Frontend**: Next.js 14, React, TypeScript, Tailwind CSS
- **Backend**: Python, Flask/FastAPI
- **Web3**: AlgoKit, Pera Wallet SDK
- **Deployment**: Vercel (Frontend), AWS/Railway (Backend)
- **Tools**: AlgoKit CLI, Lora Explorer

---

## 📊 Project Status

✅ Smart contracts deployed on Algorand TestNet  
✅ Frontend deployed and functional  
✅ Wallet integration working  
✅ DAO governance system implemented  
✅ QR code generation and scanning  
🔄 Backend API optimization in progress  
🔄 Mobile responsive improvements  
📋 Future: Mainnet deployment, mobile app, advanced analytics  

---

**Built for Algorand Hackathon Series - Algofinity** 🌟
