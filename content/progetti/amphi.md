+++
title = "AMPHI: Ticketing NFT & P2P Marketplace" # Titolo descrittivo
date = 2025-04-27T21:21:00+02:00 # Data/ora attuale o di inizio progetto
draft = false
weight = 10 # Diamo un peso basso per farlo apparire tra i primi progetti?
tags = ["Blockchain", "NFT", "Ticketing", "Web App", "Anti-Scalping", "AI"] # Conferma o modifica i tag più appropriati
# Manteniamo la coerenza nascondendo metadati e ToC
[paige.pages]
  disable_keywords = true       # Nasconde i tag sulla pagina singola
  disable_date = true           # Nasconde la data
  disable_word_count = true   # Nasconde conteggio parole
  disable_reading_time = true # Nasconde tempo lettura
  disable_toc = true           # Nasconde l'indice
+++

**AMPHI** è un progetto che affronta un problema noto e frustrante nel mondo degli eventi dal vivo: il **secondary ticketing non trasparente, lo scalping e l'azione dei bot** che danneggiano fan, artisti e organizzatori.

### La Soluzione: Biglietti NFT su Blockchain

L'idea centrale di AMPHI è trasformare i biglietti per eventi in **Non-Fungible Tokens (NFT)** gestiti su blockchain (attualmente testato su Polygon Amoy). Questo approccio permette di introdurre:

* **Trasparenza:** Ogni biglietto è unico e la sua storia (emissione, passaggi di proprietà) è tracciabile on-chain.
* **Controllo:** È possibile implementare regole direttamente nello smart contract del biglietto o nel marketplace per limitare pratiche scorrette.
* **Nuove Possibilità:** Gli NFT aprono le porte a esperienze aggiuntive per i fan (collezionabili digitali, contenuti esclusivi, meccanismi di loyalty).

### L'MVP (Minimum Viable Product)

Ho sviluppato un **MVP (Minimum Viable Product) / Demo funzionante** che dimostra le funzionalità core:

1.  **Vendita Primaria (Minting):** Emissione di biglietti NFT associati a eventi specifici.
2.  **Marketplace Secondario P2P:** Una piattaforma dove gli utenti possono rivendere i propri biglietti NFT ad altri utenti.
3.  **Meccanismo Anti-Scalping:** Implementazione di un **price cap** nel marketplace secondario per impedire la rivendita a prezzi maggiorati rispetto all'originale.
4.  **Gestione Wallet:** Supporto sia per wallet gestiti internamente (custodial ibrido) sia per il collegamento di wallet esterni (es. MetaMask).

### Stack Tecnologico (Panoramica)

Il progetto è strutturato come **monorepo** e utilizza:

* **Smart Contracts:** Solidity (standard ERC721) con framework Hardhat su Polygon Amoy.
* **Backend:** API REST costruita con Node.js ed Express, interagisce con la blockchain tramite Ethers.js e gestisce un database PostgreSQL come cache off-chain.
* **Frontend:** Single Page Application sviluppata con Vue.js 3 e Vite, utilizzando Pinia per lo state management e Axios per le chiamate API.

### Stato Attuale e Codice

L'MVP dimostra la fattibilità tecnica del concetto. Lo sviluppo è in corso, focalizzato sull'integrazione dei flussi di pagamento e sul supporto completo dei wallet esterni.

Il codice sorgente completo è disponibile pubblicamente su GitHub:
**[github.com/modernage12/ticketing-nft](https://github.com/modernage12/ticketing-nft/tree/main)**