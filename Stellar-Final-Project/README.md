#Stellar Soroban: Digital Counter dApp

This is a **full-stack decentralized application (dApp)** developed as the Final Project for the Stellar Bootcamp. The project demonstrates a seamless integration between a Rust-based smart contract and a web frontend on the **Stellar Testnet**.

##Project Overview
The application is a decentralized "Global Counter". It allows users to interact with a smart contract deployed on the Stellar network to increment a shared value. Every interaction is cryptographically signed and recorded on the blockchain.

###Key Features
- **Smart Contract:** Developed with Soroban SDK in Rust for high performance and security.
- **Frontend Integration:** A clean UI that connects to the Stellar network via the **Freighter Wallet**.
- **Real-time State:** Fetches the current counter value directly from the Testnet.

---

##Tech Stack
- **Blockchain:** Stellar (Testnet)
- **Smart Contract:** Soroban (Rust)
- **Frontend:** HTML5, CSS3, JavaScript (Stellar SDK)
- **Wallet:** Freighter Wallet

---

##  How to Set Up & Run

### 1. Smart Contract Deployment
To compile and deploy the contract to the Stellar Testnet:

```bash
# Build the contract
soroban contract build

# Deploy to Testnet
soroban contract deploy \
  --network testnet \
  --source-account <YOUR_ACCOUNT_NAME> \
  --wasm target/wasm32-unknown-unknown/release/counter_contract.wasm

