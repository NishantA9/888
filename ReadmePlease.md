# CodeMiners - Decentralized NFT Marketplace

## Group Members
1. **Nishant Acharekar** - 801363902  
2. **Mihir Phatak** - 801358341  
3. **Shubham Kakade** - 801413848  
4. **Calvin Pinto** - 801320115  
5. **Deepiga Sengottuvelu Ravichandran** - 801370629  
6. **Sandesh Mahajan** - 801366489  

---
## Features
- **NFT Minting**: Users can upload assets and mint them into NFTs.
- **Listing NFTs for Sale**: Sellers can set prices and list their NFTs.
- **Buying NFTs**: Users can purchase NFTs with ICP tokens.
- **Ownership Transfer**: Secure on-chain ownership transfer upon purchase.
- **Viewing Owned NFTs**: A dedicated section for users to track their NFTs.
- **NFT Discovery**: A dynamic gallery showcasing trending and newly minted NFTs.
---

### **1. Start Local Replica Open 3 terminals**
```bash
dfx start --clean
```

### **2. On Second Terminal deploy the caniseter**

```
dfx deploy --argument='("CryptoDunks #123", principal "hosul-rjfsa-n5acb-pbddr-q3hbc-g7umk-ybwt4-xfyjz-633jk-mm6ar-rqe", (vec {137; 80; 78; 71; 13; 10; 26; 10; 0; 0; 0; 13; 73; 72; 68; 82; 0; 0; 0; 10; 0; 0; 0; 10; 8; 6; 0; 0; 0; 141; 50; 207; 189; 0; 0; 0; 1; 115; 82; 71; 66; 0; 174; 206; 28; 233; 0; 0; 0; 68; 101; 88; 73; 102; 77; 77; 0; 42; 0; 0; 0; 8; 0; 1; 135; 105; 0; 4; 0; 0; 0; 1; 0; 0; 0; 26; 0; 0; 0; 0; 0; 3; 160; 1; 0; 3; 0; 0; 0; 1; 0; 1; 0; 0; 160; 2; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 160; 3; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 0; 0; 0; 0; 59; 120; 184; 245; 0; 0; 0; 113; 73; 68; 65; 84; 24; 25; 133; 143; 203; 13; 128; 48; 12; 67; 147; 94; 97; 30; 24; 0; 198; 134; 1; 96; 30; 56; 151; 56; 212; 85; 68; 17; 88; 106; 243; 241; 235; 39; 42; 183; 114; 137; 12; 106; 73; 236; 105; 98; 227; 152; 6; 193; 42; 114; 40; 214; 126; 50; 52; 8; 74; 183; 108; 158; 159; 243; 40; 253; 186; 75; 122; 131; 64; 0; 160; 192; 168; 109; 241; 47; 244; 154; 152; 112; 237; 159; 252; 105; 64; 95; 48; 61; 12; 3; 61; 167; 244; 38; 33; 43; 148; 96; 3; 71; 8; 102; 4; 43; 140; 164; 168; 250; 23; 219; 242; 38; 84; 91; 18; 112; 63; 0; 0; 0; 0; 73; 69; 78; 68; 174; 66; 96; 130;}))'
```

### **3. Start NPM server on 3rd Terminal**

```
npm start
```

### **4. Creating NFT for Testing**

1. Mint an NFT on the command line to get NFT into mapOfNFTs:

```
dfx canister call opend mint '(vec {137; 80; 78; 71; 13; 10; 26; 10; 0; 0; 0; 13; 73; 72; 68; 82; 0; 0; 0; 10; 0; 0; 0; 10; 8; 6; 0; 0; 0; 141; 50; 207; 189; 0; 0; 0; 1; 115; 82; 71; 66; 0; 174; 206; 28; 233; 0; 0; 0; 68; 101; 88; 73; 102; 77; 77; 0; 42; 0; 0; 0; 8; 0; 1; 135; 105; 0; 4; 0; 0; 0; 1; 0; 0; 0; 26; 0; 0; 0; 0; 0; 3; 160; 1; 0; 3; 0; 0; 0; 1; 0; 1; 0; 0; 160; 2; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 160; 3; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 0; 0; 0; 0; 59; 120; 184; 245; 0; 0; 0; 113; 73; 68; 65; 84; 24; 25; 133; 143; 203; 13; 128; 48; 12; 67; 147; 94; 97; 30; 24; 0; 198; 134; 1; 96; 30; 56; 151; 56; 212; 85; 68; 17; 88; 106; 243; 241; 235; 39; 42; 183; 114; 137; 12; 106; 73; 236; 105; 98; 227; 152; 6; 193; 42; 114; 40; 214; 126; 50; 52; 8; 74; 183; 108; 158; 159; 243; 40; 253; 186; 75; 122; 131; 64; 0; 160; 192; 168; 109; 241; 47; 244; 154; 152; 112; 237; 159; 252; 105; 64; 95; 48; 61; 12; 3; 61; 167; 244; 38; 33; 43; 148; 96; 3; 71; 8; 102; 4; 43; 140; 164; 168; 250; 23; 219; 242; 38; 84; 91; 18; 112; 63; 0; 0; 0; 0; 73; 69; 78; 68; 174; 66; 96; 130;}, "CryptoDunks #123")'

rno2w-sqaaa-aaaaa-aaacq-cai
```

2. List the item into mapOfListings:

```
dfx canister call opend listItem '(principal "<REPLACE WITH NFT CANISTER ID>", 2)'

dfx canister call opend listItem '(principal "rno2w-sqaaa-aaaaa-aaacq-cai", 2)'

renrk-eyaaa-aaaaa-aaada-cai

```


3. Get OpenD canister ID:

```
dfx canister id opend

eg: ryjl3-tyaaa-aaaaa-aaaba-cai
```

4. Get Name, Owner and asset

dfx canister call nft getName
dfx canister call nft getOwner
dfx canister call nft getAsset

5. Mint another NFT on the command line to get NFT into mapOfNFTs

dfx canister call opend mint '(vec {137; 80; 78; 71; 13; 10; 26; 10; 0; 0; 0; 13; 73; 72; 68; 82; 0; 0; 0; 10; 0; 0; 0; 10; 8; 6; 0; 0; 0; 141; 50; 207; 189; 0; 0; 0; 1; 115; 82; 71; 66; 0; 174; 206; 28; 233; 0; 0; 0; 68; 101; 88; 73; 102; 77; 77; 0; 42; 0; 0; 0; 8; 0; 1; 135; 105; 0; 4; 0; 0; 0; 1; 0; 0; 0; 26; 0; 0; 0; 0; 0; 3; 160; 1; 0; 3; 0; 0; 0; 1; 0; 1; 0; 0; 160; 2; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 160; 3; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 0; 0; 0; 0; 59; 120; 184; 245; 0; 0; 0; 113; 73; 68; 65; 84; 24; 25; 133; 143; 203; 13; 128; 48; 12; 67; 147; 94; 97; 30; 24; 0; 198; 134; 1; 96; 30; 56; 151; 56; 212; 85; 68; 17; 88; 106; 243; 241; 235; 39; 42; 183; 114; 137; 12; 106; 73; 236; 105; 98; 227; 152; 6; 193; 42; 114; 40; 214; 126; 50; 52; 8; 74; 183; 108; 158; 159; 243; 40; 253; 186; 75; 122; 131; 64; 0; 160; 192; 168; 109; 241; 47; 244; 154; 152; 112; 237; 159; 252; 105; 64; 95; 48; 61; 12; 3; 61; 167; 244; 38; 33; 43; 148; 96; 3; 71; 8; 102; 4; 43; 140; 164; 168; 250; 23; 219; 242; 38; 84; 91; 18; 112; 63; 0; 0; 0; 0; 73; 69; 78; 68; 174; 66; 96; 130;}, "CryptoDunks #133")'


6. At the last you will see the new id copy that and paste it below and list the second id

dfx canister call opend listItem '(principal "<REPLACE WITH NFT CANISTER ID>", 2)'

dfx canister call opend listItem '(principal "renrk-eyaaa-aaaaa-aaada-cai", 4)'


7. Tansfer

```
dfx canister call <REPLACE WITH NFT CANISTER ID> transferOwnership '(principal "<REPLACE WITH OPEND CANISTER ID>", true)'

rno2w-sqaaa-aaaaa-aaacq-cai (This is id 1)
renrk-eyaaa-aaaaa-aaada-cai (This is id 2)

dfx canister call rno2w-sqaaa-aaaaa-aaacq-cai transferOwnership '(principal "renrk-eyaaa-aaaaa-aaada-cai", true)'

```


## Project Overview

This project is a **Decentralized NFT Marketplace** built on the **Internet Computer (ICP) blockchain** using **Motoko** for smart contracts and **React.js** for the frontend. The platform enables users to **mint, buy, sell, and trade NFTs** while ensuring secure transactions and decentralized ownership. 

Our project references and extends concepts from various sources, including foundational ideas from the **London App Brewery's Web Developer Bootcamp 2024** and other blockchain-related implementations. The code has been adapted and improved to fit the use cases specific to this project, ensuring originality and enhanced functionality.

## **Acknowledgments & References**
This project was inspired by multiple sources, including open-source blockchain implementations and NFT marketplaces. Some concepts and snippets were adapted from the **London App Brewery's NFT-related courses** and modified for our specific use case.
- [Internet Computer Developer Docs](https://internetcomputer.org/docs/current/developer-docs/setup/deploy-locally)
- [Motoko Programming Language](https://internetcomputer.org/docs/current/motoko/main/motoko)
- [NFT Marketplace Standards](https://blog.nftbooks.info/nft-technology-and-standards-a-comprehensive-guide/)

This project is licensed under the **Apache License 2.0**. See the full license details [here](http://www.apache.org/licenses/LICENSE-2.0).

---

🚀 **Developed by CodeMiners** 🚀