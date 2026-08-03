# 💼 Gigmint — Decentralized Freelance Marketplace

[![Flutter](https://img.shields.io/badge/Flutter-3.22+-02569B?logo=flutter&logoColor=white)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/Dart-3.4+-0175C2?logo=dart&logoColor=white)](https://dart.dev)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

**Gigmint** is a decentralized freelance marketplace that replaces traditional platform fees (20–30%) with **smart contract escrow**, enabling freelancers to receive **instant USDC payments**, milestone-based releases, and transparent dispute resolution through bonded arbitrators.

---

## 📖 Overview

Gigmint empowers clients and freelancers with a trustless payment system powered by blockchain.

## Core Benefits

- 💰 Instant USDC payouts
- 🔒 Smart contract escrow
- ⚖️ Decentralized dispute resolution
- 📁 IPFS-backed deliverables
- ⛽ Gas abstraction for better UX
- 🛡️ Sybil-resistant identity verification

---

## ✨ Features

### 🔐 Smart Contract Escrow

Funds are securely locked in smart contracts and released only after milestone approval.

## 💵 Instant USDC Payments

Payments settle in **under 30 seconds** on Polygon.

## ⚖️ Bonded Arbitrator Disputes

Independent arbitrators stake funds to ensure honest dispute resolution without requiring a platform token.

## ⛽ Gas Abstraction

Users pay gas fees in USDC while the platform subsidizes the first five transactions.

## 📁 IPFS Deliverables

Project submissions are stored on IPFS, creating tamper-proof proof of work.

## 🛡️ Sybil Resistance

Identity verification combines:

- Gitcoin Passport
- Wallet reputation
- Optional staking

## ⏳ Automatic Release

Funds automatically release after:

- 7-day review period
- 3-day challenge window

---

## 🏗 Project Structure

```text
lib/
├── core/
│   ├── constants/
│   ├── exceptions/
│   ├── services/
│   └── utils/
│
├── features/
│   ├── auth/
│   ├── dashboard/
│   ├── find_work/
│   ├── create_gig/
│   ├── submit_deliverable/
│   ├── dispute/
│   └── profile/
│
├── models/
├── repositories/
├── widgets/
└── main.dart
```

---

## 🏛 Architecture

```text
Flutter Mobile App
        │
        ▼
Riverpod / Bloc
        │
        ▼
Repository Layer
        │
        ▼
Blockchain Services
        │
 ┌──────┴─────────┐
 │                │
IPFS         WalletConnect
 │                │
 └──────┬─────────┘
        ▼
Polygon Smart Contracts
        │
        ▼
USDC Escrow & Arbitration
```

---

## 🛠 Tech Stack

| Category | Technology ||----------|------------|
| Mobile | Flutter 3.22+, Dart 3.4+ |
| State Management | Riverpod / Bloc |
| Blockchain | Polygon zkEVM |
| Smart Contracts | Solidity |
| Web3 | web3dart, WalletConnect v2 |
| Storage | IPFS (Pinata), Hive |
| Notifications | Firebase Cloud Messaging |
| Architecture | Feature-first, Repository Pattern, Dependency Injection |

---

## 🚀 Getting Started

### Prerequisites

- Flutter SDK 3.22+
- Dart SDK
- Android Studio or VS Code
- MetaMask or another Web3 wallet

---

## Installation

```bash
# Clone repository
git clone https://github.com/yourusername/gigmint.git

# Navigate to project
cd gigmint

# Install dependencies
flutter pub get

# Run the application
flutter run
```

---

### ⚙ Environment Variables

Create a `.env` file in the project root.

```env
RPC_URL=https://polygon-rpc-url

PINATA_API_KEY=YOUR_PINATA_KEY

PINATA_SECRET=YOUR_PINATA_SECRET

WALLETCONNECT_PROJECT_ID=YOUR_PROJECT_ID

USDC_CONTRACT_ADDRESS=YOUR_USDC_CONTRACT
```

---

### 📱 Core Modules

| Module | Description |
|---------|-------------|
| Authentication | Wallet connection and onboarding |
| Dashboard | Active contracts and earnings overview |
| Find Work | Browse jobs and submit proposals |
| Create Gig | Client-side project creation |
| Deliverables | Upload files to IPFS |
| Disputes | Arbitration workflow |
| Profile | Reputation, verification and settings |

---

### 📊 Platform Metrics

| Metric | Value |
|---------|-------|
| Platform Fee | **1.5%** *(0% for gigs under $100)* |
| Payment Settlement | **<30 seconds** |
| Dispute Resolution | **<48 hours** |
| Review Period | **7 days** |
| Challenge Window | **3 days** |
| Arbitrator Stake | **100 USDC** |
| Arbitrator Reward | **5% (minimum 10 USDC)** |

---

### 🔮 Roadmap

- [ ] Multi-chain deployment
- [ ] AI-powered proposal matching
- [ ] Decentralized freelancer reputation
- [ ] Cross-chain escrow
- [ ] Team workspaces
- [ ] DAO governance
- [ ] Mobile notifications
- [ ] Fiat on/off ramps

---

### 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Open a Pull Request

---

### 📄 License

This project is licensed under the **MIT License**.

See the **LICENSE** file for more information.

---

### 👨‍💻 Developed By

### **TOE Tech**

Building decentralized products that make Web3 accessible to everyone.

---

## ⭐ Support

If you like this project, consider giving it a **star** on GitHub to support future development.
