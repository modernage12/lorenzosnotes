+++
title = "Sito Personale con Framework Hugo"
date = 2025-04-27T13:55:00+02:00 # Data iniziale o aggiornata
draft = false
weight = 50 # O il peso che preferisci per l'ordine
tags = ["Hugo", "Sito Web", "Portfolio", "GitHub Pages", "GitHub Actions", "Paige Theme", "Static Site", "Google Analytics"] # Aggiunto GA
# Nascondiamo i metadati/etc per coerenza
[paige.pages]
  disable_keywords = true
  disable_date = true
  disable_word_count = true
  disable_reading_time = true
  disable_toc = true
+++

Questo è il progetto di creazione e sviluppo continuo del mio sito/portfolio personale, lo spazio digitale in cui ti trovi ora! È stato costruito utilizzando il generatore di siti statici **Hugo** e il tema **Paige**.

### Obiettivo:
Creare uno spazio online per presentarmi in modo più completo rispetto a un CV tradizionale, mostrando esperienze lavorative e formative, progetti personali, interessi e competenze in modo dinamico e autentico.

### Tecnologie e Strumenti Utilizzati:
* **Generatore Sito Statico:** Hugo (v0.141.0 Extended)
* **Tema:** Paige (integrato come Git Submodule)
* **Linguaggio Contenuti:** Markdown con Front Matter TOML
* **Hosting:** GitHub Pages (configurato per deployment gratuito)
* **Deployment Automatico:** GitHub Actions (workflow custom con `peaceiris/actions-gh-pages` per build e push su branch `gh-pages`)
* **Dipendenze Build:** Dart Sass (installato nel workflow Actions per compilare SCSS del tema)
* **Controllo Versione:** Git e GitHub
* **`Analytics: Google Analytics (GA4) per il monitoraggio delle visite e del comportamento utente.`**

### Cosa ho Imparato e Sfide Superate:
Questo progetto è stato un’ottima palestra per approfondire diversi aspetti dello sviluppo web e del workflow moderno:
* **Configurazione Avanzata di Hugo:** Gestione di `hugo.toml`, `baseURL`, parametri del tema ([params.paige], [params.paige.site], [params.paige.subpages]), menu personalizzato, gestione `weight` per ordinamento.
* **Gestione Contenuti:** Strutturazione in sezioni (`content/`), uso di `_index.md`, personalizzazione Front Matter per singole pagine e sezioni (es. nascondere metadati/ToC).
* **Personalizzazione Tema:** Override di partials del tema (es. `head.html` per GA, `site-footer-last.html` per link social) per inserire funzionalità custom mantenendo aggiornabile il tema principale.
* **Gestione Asset Statici:** Utilizzo della cartella `static` per file come il CV PDF.
* **Deployment Automatizzato:** Configurazione e debug approfondito di GitHub Actions, sperimentando diversi workflow (actions/deploy-pages vs `peaceiris/actions-gh-pages`), gestendo permessi (`contents: write`) e risolvendo dipendenze di build nell’ambiente Actions (versioni Hugo, installazione Dart Sass).
* **`Integrazione Analytics: Implementazione manuale dello snippet di Google Analytics (GA4) (tramite override del partial 'head.html' di Hugo/Paige) con l'obiettivo di tracciare le visite al sito, analizzare le user journey e raccogliere dati aggregati sull'utilizzo delle diverse sezioni.`**
* **Problem Solving:** Affrontare e risolvere errori 404 (link errati, deployment non completato), errori di build (incompatibilità Hugo/Tema, dipendenze Sass), errori di permessi su GitHub Actions.
* **Utilizzo Base HTML/CSS:** Inserimento di HTML inline (link CV, icone social) e stili base tramite parametri del tema.

### Stato Attuale:
Il sito è **attualmente online** su GitHub Pages e viene aggiornato automaticamente ad ogni `push` sul branch `master` del repository GitHub. È in continua evoluzione con l'aggiunta di nuovi contenuti e progetti.

*(Link al Repository: [github.com/modernage12/lorenzosnotes](https://github.com/modernage12/lorenzosnotes) - puoi aggiungerlo se vuoi)*