# Right-to-Use-Core

<a name="readme-top"></a>

<br />
<div align="center">
  <a href="https://github.com/codeEzzy/lightlink">
    <img src="./diagrams/right.png" alt="Logo" width="200" height="55">
  </a>

  <h3 align="center">The Right to Use (RYTU)</h3>

</div>

Welcome to the official RYTU Core Repository. This repository houses the foundational components enabling the seamless minting, management, and trading of digital content rights through NFTs on the XRPL EVM Sidechain. RYTU's mission is to empower creators with transparent, decentralized, and scalable solutions for intellectual property management.This repository is organized into three main components:

- RYTU-Frontend: The user-facing interface for interaction.
- RYTU-Backend: Handles API requests, business logic, and data orchestration.
- RYTU-Contract: Solidity-based smart contracts that implement the marketplace's logic. This is deployed on XRPL EVM Sidechain

## Repository Overview:
The repository is organized into three main components:
```
RYTU-Core/
├── rytu-frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   ├── README.md
├── rytu-backend/
│   ├── dist/
│   ├── src/
│   ├── package.json
│   ├── README.md
├── rytu-contract/
│   ├── docs/
    ├── lib/
    ├── script/
│   ├── src/
│   ├── test/
│   ├── foundary.toml
│   ├── README.md
└── README.md
```
## System Design and Narrative
RYTU combines blockchain technology, smart contracts, and an intuitive UI to redefine digital content rights licensing. The core is built with:

- Frontend: React.js + Next.js
- Backend: Node.js + GraphQL
- Smart Contracts: Solidity on XRPL EVM Sidechain

## Architecture Diagram
Refer to the /diagrams folder for an architectural representation of the platform and its XRPL integrations.

# Quick Start Guide
## RYTU-Frontend
#### Installation Instructions
 - Git clone the repository
 - Navigate to the ```rytu-frontend directory```
 ```
 bash

 cd rytu-frontend
 ```
 - Install dependencies:
```
npm install or yarn install
```

- Start the development server:
```
npm start

```

![Alt text](./diagrams/rytuui.png?raw=true "Rytu on Testnet")


### Fronted code located in:
[Click to view](https://github.com/Dynamic-Flakes/rytu-frontend)

### RYTU-Backend
#### Installation Instructions
- Git clone the repository
- Navigate to the rytu-backend directory:
```
cd rytu-backend
```
- Install dependencies:
```
npm install or yarn install
```
- Start the server:
```
npm start or yarn start
```
# Backend code located in:
[Click to view](https://github.com/Dynamic-Flakes/rytu-backend)

### RYTU-Contract
##### Compilation and Deployment
- Git clone the repository
- Foundry: Install it by running:
```
curl -L https://foundry.paradigm.xyz | bash
foundryup
```
- Navigate to the rytu-contract directory:
```
cd rytu-contract
```
- Build the contract to generate the ABI and bytecode in the out/ directory.

```
forge build
```
- Deployment : 

  - Configuration: Ensure the deployment environment variables are set in a .env file:
  ```
  RPC_URL="https://your-network-rpc-url"
  PRIVATE_KEY="your-private-key"

  ```
  - Script Execution: Use a prewritten deployment script in the script/ directory. Example:
  ```
  forge script script/Deploy.s.sol --rpc-url $RPC_URL --private-key $PRIVATE_KEY --broadcast
  ```
  - Verify deployment
  ```
  forge verify-contract <contract_address> <source_file> --chain-id <sidechain_chain_id> --etherscan-api-key <api_key>
  ```
 
#### Smart contracts code located in:
 [Click to view](https://github.com/Dynamic-Flakes/rytu-contract)


## Key Features
## RYTU-Frontend
Description
The frontend is built using React.js, Nextjs, Typescript, Graphql and styled with Tailwind CSS, providing a seamless user experience for minting, managing, and trading RYTU NFTs.

Key Features
- Seamless onboarding and Wallet integration (XRP Ledger).
- Minting and verify ownership interface.
- Create Rytu 
- Request Rytu
- Verification certification
- Explore marketplace

### RYTU-Backend
Description:
The backend is powered by Node.js, Graphql and Express.js, responsible for handling API requests, transaction validation, and integration with the XRPL.

#### Key Features
- API for querying NFT metadata and marketplace transactions.
- Authentication and user management.
- Analytics and reporting on NFT activity.


### RYTU-Contract
Description
The smart contract layer implements the core RYTU NFT marketplace logic, deployed on the XRPL EVM Sidechain.

#### Key Features
- Minting ERC-721 and ERC-1155 NFTs.
- Royalty distribution and fractional ownership.
- Auction and bidding mechanisms.

## XRPL Integration
RYTU uses XRPL's EVM Sidechain for:
- NFT Tokenization: Fast minting and metadata storage for scalable and verifiable rights management.
- Global Payments: Leveraging XRPL's low-fee infrastructure for seamless cross-border transactions.
- On-Chain Automation: Smart contract-based licensing and royalty disbursement.

### Product Roadmap
- Phase 1: Research, Design, and Prototype Development (Months 1–3)
:
   - Research and define integration strategies with XRPL’s infrastructure.
   - Design a seamless user interface for onboarding creators and buyers, focusing on intuitive workflows
   - Develop prototype smart contracts for minting RYTU NFTs (ERC-721 and ERC-1155 standards) and royalty distribution.
   - Set up a test environment on XRPL Devnet to validate initial functionalities.
 
- Phase 2: Core Platform Development (Months 4–6)
    - Implement marketplace features: bidding system, unlockable content, and personal NFT collections
    - Integrate XRPL wallet solutions for secure transactions and user authentication.
    - Conduct internal testing for stability, performance, and functionality.

    - Implement advanced auction mechanics.

- Phase 3: Beta Launch and Community Engagement (Months 7–9)
  - Launch beta version of the platform on XRPL Testnet with select creators and users.
  - Implement feedback-driven improvements to enhance user experience and platform reliability
  - Develop educational materials and marketing campaigns to onboard creators and buyers.
  - Integrate additional features such as analytics for creators and sustainability tracking tools.
  - Launch a comprehensive marketing campaign targeting content creators, investors, and brands.
   - Partner with influencers and creator hubs to encourage the adoption of the RYTU platform.
   - Expand XRPL wallet integrations to include popular wallets like Xumm.
 

- Phase 4: Full Launch and Scaling  (10-12 months):
   - Scale platform with gamified rewards.
   - Introduce sustainability-focused features.
   - Deploy the final version of RYTU on XRPL Mainnet.
   - Implement advanced features like ad-space purchasing and royalty distribution among collaborators
   - Initiate global partnerships and expand outreach campaigns to drive adoption.
   - Establish ongoing support mechanisms for users and a feedback loop for platform updates.
  - Release the production version of RYTU, with features for cross-border licensing, royalty tracking, and dispute resolution.
   - Establish partnerships with media companies and brands to encourage bulk licensing on the platform.
   - Scale platform security and infrastructure to support global adoption.



## Security and Compliance
 - GDPR and CCPA compliance for data privacy.
- Use of XRPL's transparency for verifiable licensing records.
- Cybersecurity measures, including encryption and multi-factor authentication.

## License
This project is licensed under the MIT License.

Contributors:

- Sunday Aroh
- Odoh David
