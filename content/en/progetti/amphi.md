+++
title = "AMPHI: NFT Ticketing & P2P Marketplace" # Descriptive title
date = 2025-04-27T21:21:00+02:00 # Current date/time or project start
draft = false
weight = 10 # Should we give it a low weight to make it appear among the first projects?
tags = ["Blockchain", "NFT", "Ticketing", "Web App", "Anti-Scalping", "AI"] # Confirm or modify the most appropriate tags
# Let's maintain consistency by hiding metadata and ToC
[paige.pages]
  disable_keywords = true       # Hides tags on the single page
  disable_date = true           # Hides the date
  disable_word_count = true   # Hides word count
  disable_reading_time = true # Hides reading time
  disable_toc = true           # Hides the table of contents
+++

**AMPHI** is a project that tackles a well-known and frustrating problem in the world of live events: **non-transparent secondary ticketing, scalping, and bot activity** that harm fans, artists, and organizers.

### The Solution: NFT Tickets on Blockchain

The core idea of AMPHI is to transform event tickets into **Non-Fungible Tokens (NFTs)** managed on a blockchain (currently tested on Polygon Amoy). This approach allows for the introduction of:

* **Transparency:** Each ticket is unique, and its history (issuance, ownership transfers) is traceable on-chain.
* **Control:** Rules can be implemented directly in the ticket's smart contract or the marketplace to limit unfair practices.
* **New Possibilities:** NFTs open doors to additional experiences for fans (digital collectibles, exclusive content, loyalty mechanisms).

### The MVP (Minimum Viable Product)

I have developed a working **MVP (Minimum Viable Product) / Demo** that demonstrates the core functionalities:

1.  **Primary Sale (Minting):** Issuing NFT tickets associated with specific events.
2.  **P2P Secondary Marketplace:** A platform where users can resell their NFT tickets to other users.
3.  **Anti-Scalping Mechanism:** Implementation of a **price cap** in the secondary marketplace to prevent resale at prices higher than the original.
4.  **Wallet Management:** Support for both internally managed wallets (hybrid custodial) and connecting external wallets (e.g., MetaMask).

### Technology Stack (Overview)

The project is structured as a **monorepo** and uses:

* **Smart Contracts:** Solidity (ERC721 standard) with the Hardhat framework on Polygon Amoy.
* **Backend:** REST API built with Node.js and Express, interacts with the blockchain via Ethers.js and manages a PostgreSQL database as an off-chain cache.
* **Frontend:** Single Page Application developed with Vue.js 3 and Vite, using Pinia for state management and Axios for API calls.

### Current Status and Code

The MVP demonstrates the technical feasibility of the concept. Development is ongoing, focusing on integrating payment flows and full support for external wallets.

The complete source code is publicly available on GitHub:
**[github.com/modernage12/ticketing-nft](https://github.com/modernage12/ticketing-nft/tree/main)**