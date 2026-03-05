# Unique Stellar dApp: Increment Counter

This is a full-stack decentralized application built for the Stellar Bootcamp Final Project.

##  Features
- **Smart Contract:** Written in Rust using Soroban SDK.
- **Frontend:** Simple HTML/JS interface.
- **Network:** Deployed on Stellar Testnet.

## How to Setup
1. **Contract:** - Compile: `soroban contract build`
   - Deploy: `soroban contract deploy --network testnet --source-account YOUR_ACCOUNT --wasm target.wasm`
2. **Frontend:**
   - Open `index.html` in your browser.
   - Connect your Freighter wallet to interact.

## Description
The contract stores a global counter on the Stellar blockchain. Users can call the `increment` function to increase the number.
