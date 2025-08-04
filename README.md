# Clusterizza & Misura (Speciale Advanced SEO Tools 2025)

[![Apri in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/USER/REPO/blob/master/clusterizza_e_misura.ipynb)
![OpenRouter API](https://img.shields.io/badge/OpenRouter-API-blue)

Notebook per il clustering e la valutazione automatica di dati testuali tramite modelli LLM (Large Language Model) e API OpenRouter, pensato per essere eseguito su Google Colab.

Il significato di questo tool sarà rivelato ad Search Connect 2025! 

## ✨ Funzionalità principali

- **Clustering** di dati testuali tramite modelli LLM.
- **Valutazione della similarità semantica** tra output del modello e ground truth.
- **Gestione semplice di input/output CSV**.
- **Compatibilità diretta con Google Colab** (upload file, gestione segreti, ecc.).
- **Messaggi e interfaccia completamente in italiano**.

## 🚀 Come utilizzare il notebook

### 1. Carica il notebook su Google Colab


![Schermata di caricamento del file CSV su Colab](screenshots/1.caricamento.jpg)


- Vai su [Google Colab](https://colab.research.google.com/).
- Clicca su “File” → “Carica notebook” e seleziona `clusterizza_e_misura.ipynb` dal tuo computer.


### 2. Inserisci la chiave API di OpenRouter

![Inserisci la chiave API](screenshots/2.chiaveapi.jpg)

- Segui le istruzioni nella prima cella del notebook per inserire la tua chiave API (tramite Colab Secrets o campo diretto).


### 3. Carica il file CSV di input

![carica il file csv](screenshots/3.caricacsv.jpg)

- Utilizza la sezione dedicata per caricare il tuo file CSV.
- Il file deve contenere almeno le colonne `input` e `ground_truth`.
- poi seleziona col tasto detro "copia percorso"
- se ti serve un esempio seleziona "copia percorso" su test-30-martino.csv (ottimo se devi configurare il documento con le tue query)

### 4. Configura i Prompt di servizio

![configuriamo i prompts](screenshots/4.prompt.jpg)

In questa cella definisci i 2 prompt che saranno usati dal servizio.

- il primo prompt effettua la categorizzazione, per cui devi dire al modello con quali considerazioni adottare per clusterizzare una query e fornire degli esempi di come effettuarla.
- il secondo prompt applica una valutazione semantica sul risultato ottenuto dal primo prompt, confrontandolo con la "verità" (ground_truth) fornita nel file csv.

### 5. Configura i parametri

![configuriamo i parametri](screenshots/5.parametri.jpg)


- Imposta i modelli da utilizzare, gli altri parametri secondo le tue esigenze.
- incolla il percorso del file csv nel campo corrispondente

### 6. Avvia l’elaborazione

![Avvia il processo](screenshots/6.avvio.jpg)


- Esegui le celle del notebook una alla volta (Shift+Invio) seguendo l’ordine suggerito.
- Al termine, scarica i risultati dalla sezione “risultati”.

---

## 📂 Struttura del progetto

- `clusterizza_e_misura.ipynb` — Notebook principale, pronto per l’uso su Colab.
- `README.md` — Questo file.
- `test-30-martino.csv` - file di esempio  
- `screenshots` - immagini di queste istruzioni
  
---

## ℹ️ Note

- Il notebook è pensato per essere eseguito unicamente su Google Colab. L’esecuzione in ambiente locale richiede l’installazione manuale delle dipendenze e l’adattamento di alcune funzionalità (upload file, gestione segreti, ecc.). Per il mio esperimento non sono necessarie, ma se volete eseguirlo localmente dovete aggiungerle.
- Per assistenza o segnalazione bug, apri una issue su GitHub.

---

## ✍️ Crediti

- A cura di [Andrea Scarpetta](https://www.andreascarpetta.it), parte del collettivo [Search Foundry](https://www.searchfoundry.pro)

- File di esempio curato da [Martino Mosna](https://www.martinomosna.com).

## Licenza

Questo progetto è distribuito con licenza [MIT](LICENSE).

## Come contribuire

Se vuoi contribuire, proporre miglioramenti o segnalare problemi (e non sai usare le issue di github), puoi contattarmi direttamente su [LinkedIn](https://www.linkedin.com/in/andreascarpetta).

## FAQ

Work in progress.

---
© 2025 Andrea Scarpetta, Search Foundry

Made with ❤️, AI and [Jupyter](https://jupyter.org/) · Powered by [OpenRouter](https://openrouter.ai/)

Questo progetto è rilasciato a scopo didattico e sperimentale. Nessuna garanzia di funzionamento in produzione.

Se ti è stato utile, lascia una ⭐️ su GitHub!



