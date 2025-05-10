# ZaaNet Litepaper  
**A Decentralized Internet Sharing Platform for Everyone**  
**Version:** 1  
**Date:** May 2025

---

## 1. Introduction

Access to affordable and reliable internet remains a significant challenge across Africa and other underserved regions. Despite expanding mobile and broadband coverage, internet access remains either prohibitively expensive or unreliable for large portions of the population.

ZaaNet addresses this problem by introducing a decentralized, peer-to-peer WiFi sharing platform powered by smart contracts on Arbitrum Sepolia. Derived from the Dagbani word _"Zaa,"_ meaning _"everyone,"_ ZaaNet’s mission is to democratize internet access — enabling anyone with a high-speed internet connection to monetize their network securely, and allowing users nearby to access affordable, time-limited connectivity.

---

## 2. Problem Statement

In many urban, peri-urban, and rural areas:

- Internet access is costly compared to average incomes.  
- Many individuals and small businesses have surplus broadband capacity that goes unused.  
- There is no decentralized, trusted way to securely share or sell internet access.  
- Centralized ISPs dominate pricing models, offering little flexibility or peer-to-peer options.  
- Current WiFi sharing relies on static passwords without security enforcement, leading to misuse and revenue loss.

> Without decentralized, affordable solutions, millions remain digitally excluded, limiting education, entrepreneurship, and economic growth potential.

---

## 3. Solution Overview

ZaaNet provides a decentralized platform where:

- Hosts can securely share their WiFi through a local proxy device and earn income through direct, time-limited payments on Arbitrum.  
- Guests can discover available networks, pay small session fees using USDT, and access high-speed internet securely and fairly.  
- Smart contracts manage payments, access authorization, and enforce session-based disconnections automatically.  
- **Account Abstraction (AA)** integrated, providing seamless user experience for both crypto-native and non-crypto users via smart contract wallets.

By decentralizing internet access control and payment, ZaaNet transforms internet bandwidth into a peer-to-peer, blockchain-powered utility economy.

---

## 4. Key Features

### a. Decentralized WiFi Access Marketplace  
Hosts register through the ZaaNet platform, configure a public SSID ("ZaaNetWiFi"), and connect a local proxy device that manages access control automatically.

### b. Secure Crypto Payments with Account Abstraction  
Guests pay session fees (e.g., $0.50 USDT) via smart accounts that abstract away gas fees and signing complexity. ZaaNet uses **ZeroDev** and **Web3Auth** to onboard non-technical users.

### c. Automated Session Management  
Using device-specific authentication tokens and a local proxy server, Guests are automatically disconnected after their paid session expires — ensuring fair usage without manual Host intervention.

### d. Minimal Hardware Requirements  
Hosts need only a standard WiFi router and a Raspberry Pi device running the ZaaNet proxy app.

### e. Transparent, Non-Custodial Design  
Funds flow directly from Guests to Hosts via smart contracts. ZaaNet does not custody user funds or control private credentials beyond session validation.

---

## 5. Technical Architecture

### a. Frontend  
- Built with **Next.js** and **Tailwind CSS**  
- Mobile-first and responsive  
- Smart account integration via **ZeroDev**, **Web3Auth**  
- Guest and Host dashboards for session management and earnings tracking

### b. Backend  
- Developed with **Node.js** and **Express.js**  
- **MongoDB** database for minimal metadata (sessions, device fingerprints)  
- Secure APIs to validate session tokens and monitor session expiration

### c. Smart Contracts  
- Written in **Solidity**, deployed on **Arbitrum Sepolia**  
- Accept payments in **USDT**  
- Handle session issuance, Host registration, and fee distribution transparently  
- Integrated with **ZeroDev Kernel V3.1** for account abstraction support

### d. Local Proxy Server  
- Lightweight **Node.js proxy** running on Raspberry Pi devices  
- Enforces session expiry by blocking Guest devices after their paid time ends  
- Handles IP address management and access control locally without requiring central servers

---

## 6. Target Users

### a. Hosts  
- Households with Starlink, fiber, or reliable 4G/5G broadband  
- Small shops, cafés, and coworking spaces  
- Community centers and schools offering public internet

### b. Guests  
- Students, entrepreneurs, remote workers needing short-term internet access  
- Visitors and travelers seeking affordable high-speed connectivity  
- Residents in areas where mobile data is expensive or unreliable

---

## 7. Roadmap

| Phase               | Timeline  | Milestone                                                                 |
|---------------------|-----------|---------------------------------------------------------------------------|
| MVP Launch          | Q2 2025   | Deploy smart contracts to Arbitrum Sepolia; launch proxy app; onboard Hosts |
| Pilot Program       | Q2 2025   | 10 Hosts onboarded; 1,000 Guest sessions completed; Dune Analytics dashboard live |
| Scaling & Optimization | Q3 2025 | Expand to 20+ Hosts; UX optimization; DNS filtering integration           |
| Mobile App Launch   | Q1 2026   | Release React Native mobile app for auto-authentication                  |
| Mesh Network Integration | Q2 2026 | Integrate OpenWRT/mesh routers for session-based WiFi                    |

---

## 8. Monetization and Sustainability

ZaaNet’s sustainability plan includes:

- **Platform Fees:** 10% transaction fee on each WiFi session  
- **Premium Host NFTs:** $5–$10/month for analytics, bandwidth management  
- **Institutional Partnerships:** For deployments in cafés, campuses, etc.  
- **Scalable Expansion:** Gradual rollout across Ghana and West Africa

---

## 9. Limitations and Considerations (MVP)

- **Initial Raspberry Pi Deployment:** Hosts need a device to manage sessions  
- **Offline Session Enforcement:** Proxy must stay online after payment  
- **User Education:** Onboarding required for smart accounts and tokens  
- **Scaling Infrastructure:** High-traffic Hosts may need cloud proxy fallback

---

## 10. Vision

ZaaNet’s long-term vision is to create an open, decentralized, community-driven network of affordable internet access points across underserved regions.

By turning internet access into a blockchain-based peer-to-peer service, ZaaNet aims to:

- Expand financial and digital inclusion  
- Lower barriers to education, remote work, and entrepreneurship  
- Pioneer practical **DePIN** (Decentralized Physical Infrastructure) use cases on Arbitrum

---

## 11. Contact and Community

- **Website:** Coming Soon  
- **Twitter:** Coming Soon
