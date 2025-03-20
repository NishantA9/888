# CodeMiners - Decentralized NFT Marketplace

## Group Members
1. **Nishant Acharekar** - 801363902  
2. **Mihir Phatak** - 801358341  
3. **Shubham Kakade** - 801413848  
4. **Calvin Pinto** - 801320115  
5. **Deepiga Sengottuvelu Ravichandran** - 801370629  
6. **Sandesh Mahajan** - 801366489  

---

## Project Overview

**NOTE** The project is still under development so please don't try to run this project for now as the final readme.md file would be different than this one, you can refer the code for now.

This project is a **Decentralized NFT Marketplace** built on the **Internet Computer (ICP) blockchain** using **Motoko** for smart contracts and **React.js** for the frontend. The platform enables users to **mint, buy, sell, and trade NFTs** while ensuring secure transactions and decentralized ownership. 

Our project references and extends concepts from various sources, including foundational ideas from the **London App Brewery's Web Developer Bootcamp 2024** and other blockchain-related implementations. The code has been adapted and improved to fit the use cases specific to this project, ensuring originality and enhanced functionality.

---

## Features
- **NFT Minting**: Users can upload assets and mint them into NFTs.
- **Listing NFTs for Sale**: Sellers can set prices and list their NFTs.
- **Buying NFTs**: Users can purchase NFTs with ICP tokens.
- **Ownership Transfer**: Secure on-chain ownership transfer upon purchase.
- **Viewing Owned NFTs**: A dedicated section for users to track their NFTs.
- **NFT Discovery**: A dynamic gallery showcasing trending and newly minted NFTs.

---

## Installation and Setup

### **1. Start Local Replica**
```bash
dfx start --clean
```

### **2. Install and Run the Frontend**
```bash
npm install
npm start
```

### **3. Deploy Canisters**
```bash
dfx deploy
```

### **4. Mint NFT via Command Line**
```bash
dfx canister call nft mint '("CryptoDunks #123", principal "your-principal-id", (vec {137; 80; 78; 71;}))'
```

### **5. Start the Application**
Head to:  
http://localhost:8080/

---

## **Smart Contract Interaction**
### **Query NFT Details**
```bash
dfx canister call nft getName
dfx canister call nft getOwner
dfx canister call nft getAsset
```

### **List NFT for Sale**
```bash
dfx canister call opend listItem '(principal "<NFT_CANISTER_ID>", 2)'
```

### **Transfer NFT Ownership**
```bash
dfx canister call <NFT_CANISTER_ID> transferOwnership '(principal "<MARKETPLACE_CANISTER_ID>", true)'
```

---

## **Acknowledgments & References**
This project was inspired by multiple sources, including open-source blockchain implementations and NFT marketplaces. Some concepts and snippets were adapted from the **London App Brewery's NFT-related courses** and modified for our specific use case.
- [Internet Computer Developer Docs](https://internetcomputer.org/docs/current/developer-docs/setup/deploy-locally)
- [Motoko Programming Language](https://internetcomputer.org/docs/current/motoko/main/motoko)
- [NFT Marketplace Standards](https://blog.nftbooks.info/nft-technology-and-standards-a-comprehensive-guide/)

This project is licensed under the **Apache License 2.0**. See the full license details [here](http://www.apache.org/licenses/LICENSE-2.0).

---


🚀 **Developed by CodeMiners** 🚀
