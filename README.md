# Spesa — Budget — versione V8.8

Contenuto:
- Budget totale e per categoria
- Inserimento rapido prezzo + quantità
- Anteprima senza registrazione finché non premi `+`
- Lista della spesa
- Archivio prodotti e storico prezzi
- Catalogo prezzi con salvataggio manuale e importazione di spese precedenti
- Prezzo originario prioritario e offerte conservate separatamente
- Selezione dei prodotti già presenti durante l'inserimento
- Supermercati e prezzi per supermercato
- Dispensa con quantità e soglia minima
- Statistiche
- Storico movimenti
- Ricerca
- Backup / ripristino
- Categorie personalizzabili
- Salvataggio permanente in localStorage
- Migrazione della chiave `spesaBudgetData`
- PWA installabile e cache offline

Per pubblicarla: caricare `index.html`, `manifest.webmanifest` e `sw.js` nello stesso percorso su un hosting HTTPS.

## V8.8 — gestione dello storico prezzi
- Modifica delle singole registrazioni dello storico (data, categoria, punto vendita e prezzi).
- Eliminazione di una singola registrazione senza toccare gli scontrini.
- Individuazione e rimozione, solo su conferma, delle copie perfettamente identiche nello storico.
- La modifica di un'anagrafica esistente non genera automaticamente una nuova osservazione di prezzo; la creazione di una nuova anagrafica con prezzo iniziale continua a registrare la prima osservazione.
- Chiave localStorage invariata: `spesaBudgetData`.
