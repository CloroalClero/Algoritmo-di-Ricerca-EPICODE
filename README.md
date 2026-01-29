# Job Search (Algoritmo di ricerca) - Modulo JS

Mini web app che permette di cercare inserzioni di lavoro filtrando **per titolo** e **per location** contemporaneamente, usando JavaScript + DOM.

Il progetto include anche uno stile “web app” e una visualizzazione risultati in **card** con layout **masonry (stile Pinterest)**.

## Demo online

- Live (GitHub Pages): https://cloroalclero.github.io/Algoritmo-di-Ricerca-EPICODE/
- Repo: https://github.com/CloroalClero/Algoritmo-di-Ricerca-EPICODE

---

## Funzionalità

- Ricerca **per titolo + location** (entrambi richiesti)
- Ricerca **case-insensitive** (non importa maiuscole/minuscole)
- Risultati mostrati in pagina come **card**
- Conteggio totale dei risultati trovati
- Messaggi di feedback:
  - “Inserisci sia titolo che location” se manca un input
  - “Nessun risultato trovato” se non ci sono match
- Avvio ricerca anche con **Enter** dagli input

---

## Struttura progetto

- `index.html` -> struttura della pagina (input, bottone, risultati)
- `scaricabile.js` -> logica di ricerca + gestione DOM/eventi (include l’array `jobs` da non modificare)
- `style.css` -> styling opzionale (look “LinkedIn-ish” + masonry cards)

---

## Come usare

1. Apri `index.html` nel browser oppure usa la demo online.
2. Inserisci un **titolo** (es. `dev`, `developer`, `marketing`)
3. Inserisci una **location** (es. `US`, `London`, `NZ`)
4. Premi **Cerca** oppure **Enter**
5. Leggi i risultati e il conteggio.

Esempi:
- Titolo: `dev` + Location: `US`
- Titolo: `customer` + Location: `London`

---

## Note tecniche

- La ricerca usa `.toLowerCase()` per essere case-insensitive.
- Il match avviene tramite `.includes()` (es. `US` trova anche `US, NY, New York`).
- I listener sono gestiti con `addEventListener` e l’inizializzazione avviene in `window.onload`.

---

## Extra (CSS)

Il CSS non è obbligatorio per la consegna, ma è stato aggiunto come rifinitura estetica:
- layout “web app”
- risultati in card
- masonry responsive (3 colonne desktop, 2 tablet, 1 mobile)

---

## Autore

Michel Branche
