# Right-to-Use-Core

<a name="readme-top"></a>

<br />
<div align="center">
  <a href="https://github.com/codeEzzy/lightlink">
    <img src="./diagrams/right.png" alt="Logo" width="200" height="55">
  </a>

  <h3 align="center">The Right to Use (RYTU)</h3>

</div>

Welcome to the RYTU Core Repository, which contains the essential components of the RYTU platform, enabling seamless minting, management, and trading of content rights through NFTs. This repository is organized into three main components:

- RYTU-Frontend: The user-facing interface for interaction.
- RYTU-Backend: Handles API requests, business logic, and data orchestration.
- RYTU-Contract: Solidity-based smart contracts that implement the marketplace's logic. This is deployed on XRPL EVM Sidechain

## Repository Structure
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

### Fronted code located in:
[Click to view](https://github.com/Dynamic-Flakes/rytu-frontend)

### RYTU-Backend
Description:
The backend is powered by Node.js, Graphql and Express.js, responsible for handling API requests, transaction validation, and integration with the XRPL.

#### Key Features
- API for querying NFT metadata and marketplace transactions.
- Authentication and user management.
- Analytics and reporting on NFT activity.

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


# Smart contracts code located in:
 [Click to view](https://github.com/Dynamic-Flakes/rytu-contract)

