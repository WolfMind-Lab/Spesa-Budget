# Spesa — Budget V10.0

Versione V10.0 integrata sul progetto completo V9.0. Sono stati mantenuti `index.backup.html`, manifest, service worker e README preesistenti; la chiave di archiviazione resta `spesaBudgetData`.

## Novità V10.0

### Lavatrice
- Area dedicata con anagrafiche Lavatrice, formati e scorte per formato.
- Residuo della confezione aperta e data di apertura; stima dei lavaggi residui e dose consigliata modificabile.
- Registrazione lavaggi con più prodotti e dosi separate; dose suggerita dal rapporto formato/numero lavaggi, modificabile.
- Cronologia lavaggi consultabile, modificabile, duplicabile ed eliminabile con ripristino dei consumi.
- Consumo automatico sulle confezioni aperte e apertura di una confezione sigillata quando necessario; registrazione manuale del consumo.
- Conferma facoltativa per aggiornare le scorte Lavatrice dagli acquisti registrati nello scontrino.

### Comparatore e lista intelligente
- Confronto in schede e tabella, filtro per supermercato/punto vendita e ricerca.
- Prezzi storici con data visibile, normalizzazione €/kg, €/L e €/pezzo quando i dati lo consentono.
- Confronto dei formati multipli della sezione Lavatrice.
- Scheda prodotto con indicatori: prezzo unitario più conveniente, migliore qualità personale e punteggio equilibrato (50% prezzo, 50% qualità) quando sono disponibili i dati.
- Alternative di categoria mostrate come suggerimenti con controllo di somiglianza del tipo di prodotto, senza sostituzione automatica.
- Lista intelligente con quantità modificabili, importazione dei prodotti non completati dalla lista esistente, confronto dei totali parziali per supermercato e simulazione del carrello suddiviso.
- Dati mancanti segnalati e non conteggiati come costo zero. I prezzi storici sono etichettati con la data e non sono garanzia di disponibilità attuale.
- Importazione nella lista intelligente degli elementi non completati della lista della spesa già esistente.

## Compatibilità e dati
- `localStorage` continua a usare la chiave `spesaBudgetData`.
- La migrazione aggiunge `washLog`, `smartBasket` e ID stabili ai prodotti senza eliminare le strutture precedenti.
- Backup e importazioni includono i nuovi dati; l'unione dei backup conserva gli elementi già presenti.
- Il file `index.backup.html` è conservato senza sovrascriverlo.

## Verifiche e limiti
- Controllo sintattico JavaScript eseguito con Node.js.
- Il tentativo di apertura automatizzata con Chromium headless non si è concluso nell'ambiente disponibile; non sono quindi dichiarati test end-to-end o test su iPhone.
- La lettura ottica degli scontrini (OCR) e la scansione EAN tramite fotocamera non sono incluse in questa versione.
