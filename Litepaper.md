# **ZaaNet Litepaper**  
**A Decentralized Internet Sharing Platform for Everyone**

**Version:** 1.0  
**Date:** April 2025

## **1. Introduction**

Access to affordable and reliable internet remains a major challenge in many parts of Africa and other underserved regions of the world. Despite increasing connectivity, internet access remains expensive or unreliable for a large portion of the population. ZaaNet seeks to solve this by introducing a decentralized, peer-to-peer WiFi sharing platform powered by blockchain technology.

Derived from the Dagbani word “Zaa,” meaning “everyone,” ZaaNet is built on the mission to democratize access to the internet. It empowers individuals with internet connections to earn income by securely sharing their WiFi with nearby users in exchange for stablecoin payments.

## **2. Problem Statement**

In many urban and semi-urban communities:
- Internet access is costly or unreliable.
- Many individuals and small businesses have excess data or broadband that goes unused.
- There is no trusted, transparent way to share or sell internet access securely.
- Traditional ISPs offer rigid pricing models with no peer-to-peer incentives.

## **3. Solution Overview**

ZaaNet offers a decentralized platform where:
- **WiFi Hosts** can list their available internet connections, set access prices, and earn from unused bandwidth.
- **WiFi Guests** can browse nearby networks, pay using stablecoins, and receive the access credentials for a limited time.

The entire process is secured through blockchain technology and governed by smart contracts that enforce payment logic, session duration, and platform fees.

## **4. Key Features**

### a. Peer-to-Peer WiFi Marketplace
WiFi owners register their networks, input details such as SSID, password, and pricing, and publish them on the platform. Users nearby can discover and pay for access.

### b. Crypto Payments with Stablecoins
Payments are made using USDT (Tether) on Arbitrum or Optimism, reducing friction caused by volatile tokens or fiat onboarding. Once a payment is confirmed, the smart contract emits the access credentials.

### c. Session-Based Access
Each transaction grants access for a fixed session (e.g., 1 hour). The timer is tracked off-chain but verified via the backend once the session expires.

### d. Platform Revenue Model
A small percentage (5-10%) is taken from each transaction as a platform fee. The rest is automatically transferred to the WiFi host’s wallet.

### e. Transparent and Non-Custodial
ZaaNet does not store user funds or credentials centrally. Smart contracts govern the flow of funds, and hosts maintain control over their WiFi passwords and pricing.

## **5. Technical Architecture**

### a. Frontend
- Built with **Next.js** and **Tailwind CSS**
- Fully responsive and mobile-first
- Wallet integration with **RainbowKit** and **Wagmi**
- Guest and Host dashboards
- Timer screen for active sessions

### b. Backend
- Developed using **Node.js (Express)**
- **MongoDB** for storing hosts, sessions, and metadata
- REST APIs for managing hosts, fetching sessions, and confirming payments

### c. Smart Contract
- Written in **Solidity**, deployed on **Arbitrum One**
- Accepts payments in ETH or USDT
- Splits payment: 90–95% to host, rest to platform admin
- Emits session events with timestamps and payment details

### d. Wallet Support
- Compatible with MetaMask, WalletConnect, Rainbow Wallet, and other EVM-compatible wallets

## **6. Target Users**

### a. Hosts
- Small internet cafés
- Individuals with excess mobile data or broadband
- Shops and kiosks with reliable internet

### b. Guests
- Students, workers, and travelers in need of temporary, affordable internet
- People in areas where data is unreliable or expensive

## **7. Roadmap**

| Phase | Timeline | Milestone |
|-------|----------|-----------|
| MVP Launch | Q2 2025 | Deploy on Arbitrum testnet with real WiFi host in Ghana |
| Feedback Loop | Q3 2025 | Collect real-world usage data and refine UX |
| Mainnet Rollout | Q4 2025 | Launch on Arbitrum mainnet and expand to other cities |
| Mobile App | Q1 2026 | Release wrapped mobile app using React Native |
| Decentralized Router Integration | Q2 2026 | Integrate with mesh WiFi hardware for auto access |

## **8. Monetization and Sustainability**

ZaaNet’s core monetization strategy revolves around:
- Platform fees from each transaction
- Premium features in the future such as session analytics, bandwidth controls, and reputation scoring
- Partnerships with hardware providers for router integration

## **9. Limitations & Considerations**

- ZaaNet in its MVP does not control or enforce disconnection after session expiry; enforcement is manual.
- Passwords are shared as plaintext after payment and rely on host honesty.
- Real-time location scanning is not supported in MVP (networks are listed manually).
- Future versions may include zero-knowledge proofs, encrypted access credentials, or mesh-router integration.

## **10. Vision**

ZaaNet aims to be more than a utility app — it is a movement to unlock economic and digital opportunity. By turning internet access into a peer-to-peer economy, ZaaNet can help:
- Increase financial inclusion for underserved individuals
- Lower the barrier to internet access in rural and peri-urban areas
- Encourage local innovation in last-mile connectivity

## **11. Contact and Community**

- Website: [Coming Soon]
- GitHub: [Coming Soon]
- Email: team@zaanet.org
- Telegram: t.me/zaanet
- Twitter: [Comming Soon]