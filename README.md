# 🔐 Blockchain-Based Anti-Counterfeiting Product Identification

A secure, decentralized, and tamper-proof product authentication system built on Ethereum. This project leverages blockchain technology, smart contracts, and QR code integration to fight the rising problem of counterfeit goods across global supply chains.

---

## 📜 Abstract

The proliferation of counterfeit products poses serious threats to consumer safety, brand reputation, and supply chain integrity. This project presents a Blockchain-Based Anti-Counterfeiting Product Identification System using a private Ethereum-based blockchain. Each product is uniquely tagged with a QR code linked to its blockchain-stored metadata, enabling real-time verification by any stakeholder.

The system ensures:
- Immutable product data using smart contracts
- Real-time verification with QR scanning
- Transparent product lifecycle tracking
- Tamper-proof registration and validation

---

## 🚀 Features

- ✅ Product registration via smart contracts
- 📲 QR code generation & verification
- 🛠️ Real-time product authentication
- 🔗 Blockchain-backed supply chain tracking
- 🧑‍💻 Secure wallet-based user interaction via MetaMask
- 🌐 Responsive UI for manufacturers and consumers

---

## 🧰 Tech Stack

| Layer       | Technology Used                  |
|------------|----------------------------------|
| Frontend   | HTML, CSS, JavaScript            |
| Backend    | Node.js, Express.js, Web3.js     |
| Blockchain | Ethereum (Private via Ganache)   |
| Contracts  | Solidity, Truffle                |
| Wallet     | MetaMask                         |
| Tools      | Ganache, QR Code Generator       |

---

## 🏗️ System Architecture

Manufacturer ⟶ [Frontend UI] ⟶ [Node.js Backend] ⟶ [Smart Contracts]
⤷ QR Code ↔ [Blockchain via Web3.js & Ganache]
⤶ MetaMask for Transaction Signing
⤶ Consumer Scans QR → Verifies via Blockchain


---

## 🔁 Workflow

1. **Manufacturer registers product** with details: name, batch no, date, etc.
2. A **unique QR code** is generated and linked to the product's smart contract.
3. **Product moves through the supply chain** (logged on the blockchain).
4. **Consumer scans QR code** to validate authenticity via a web interface.
5. The system verifies the blockchain entry and confirms **authentic/counterfeit** status.

---

## 📦 Project Structure

├── contracts/
│ └── ProductRegistry.sol # Smart contract for product registration
├── migrations/
│ └── deploy_contracts.js # Truffle deployment script
├── public/
│ └── index.html # Frontend UI
├── src/
│ ├── app.js # Node.js backend logic
│ └── qrgen.js # QR code generation
├── test/
│ └── product.test.js # Smart contract tests
├── truffle-config.js
├── package.json
└── README.md


---

## ⚙️ Installation & Setup

### Prerequisites
- Node.js & npm
- Truffle Suite
- Ganache
- MetaMask Extension in Browser
  
 ### Clone and Install
git clone https://github.com/your-username/blockchain-anti-counterfeit.git
cd blockchain-anti-counterfeit
npm install

Start Ganache
Open Ganache and create a new workspace.

Compile and Deploy Smart Contract

truffle compile
truffle migrate --network development

Run Backend
node src/app.js


Access Frontend
Open public/index.html in a browser with MetaMask configured to Ganache network.

✅ Results
Counterfeit detection improved by blockchain transparency

Product traceability from manufacturer to consumer

Real-time, QR-based verification with no third-party reliance

🔮 Future Scope
Integration with IoT sensors for dynamic tracking

Mobile app for QR scanning

NFT-based unique product tokens

Public blockchain and cross-chain interoperability

👨‍💻 Authors
Kanumareddy Tarun

Nallajarla Naga Krishna Manikanta

Pondugala Ramya

🏫 Department of CSE, Amrita Sai Institute of Science and Technology, Paritala, Andhra Pradesh, India

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.

📚 References
IEEE Access - Blockchain for Product Authentication

MediLedger Project

IBM Food Trust

LVMH Aura Blockchain

OECD Reports on Counterfeit Trade

---

Let me know if you want me to generate:
- The **actual `ProductRegistry.sol` smart contract**
- A **simple frontend (HTML + JS)**
- A working **Node.js backend sample**
- Or help deploy this on GitHub Pages or Render

Just say the word!



## Packages Required:-
- Truffle v5.6.7 (core: 5.6.7)
- Ganache v7.5.0
- Solidity v0.5.16 (solc-js)
- Node v16.20.0
- Web3.js v1.7.4
- npm 7.5.1

## Other Requirements:-
1. Any chromium based browser i.e. Chrome 
2. Metamask browser extension
    
## setup process 

1. Clone the project

git clone https://github.com/

2. Extract the zip file 

3. Go to the project folder, open terminal there and run following command to install required node_modules:-

npm install / npm i

4. Compile contract source files. (Compilation and deployment can be done using truffle migrate):-

truffle compile

5. Open Ganache, (to setup local blockchain)
    - crerate new workspace
    - add truffle-config.js  in truffle project 
    - change port to 7545 in server settings (same as port in truffle-config.js)

truffle migrate

6. In chrome, open metamask 
   - add new test network using  
        - NETWORK NAME (i.e. same as ganache workspace name)
        - NETWORK ID (i.e. 5777 ,from Ganache Server settings) 
        - RPC SERVER (i.e HTTP://127.0.0.1:7545 ,from Ganache Server settings)
        - CHAIN CODE (i.e. 1337)
   - import account using private key of any account from local blockchain available in Ganache.
7. In terminal, run following commands:-
- Run migrations to deploy contracts.

truffle migrate


- To start a server and it will open a homepage (index.html) file in the default browser.

npm run dev 
 
8. Login to metamask ,and connect the added account to local blockchain manually (i.e.localhost:3000)
9. Interact with website
