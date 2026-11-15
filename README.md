# Spesa — Budget V8.9

Versione completa aggiornata a partire dal progetto ricevuto dall'utente.

## Novità V8.9
- Gestione selettiva delle anagrafiche: seleziona/deseleziona tutte, elimina selezionate dopo conferma, esporta selezionate senza trascinare lo storico prezzi.
- Gestione selettiva del catalogo prezzi: seleziona/deseleziona, elimina selezionati dopo conferma, esporta selezionati scegliendo se includere lo storico prezzi.
- Importazione selettiva dei soli scontrini da un backup JSON, senza importare catalogo, anagrafiche o storico prezzi.
- Barra di chiusura unica e sempre raggiungibile in alto nelle finestre: gli eventuali pulsanti di chiusura duplicati vengono nascosti, mantenendo i riferimenti interni per compatibilità.
- Conservata la chiave locale `spesaBudgetData` e il file `index.backup.html` originale.

## Note
L'esportazione delle anagrafiche e quella del catalogo prezzi sono file separati. L'esportazione del catalogo consente di includere o escludere lo storico. L'importazione dei soli scontrini non modifica i prodotti o gli storici già presenti.


## V9.0 — Estensione sezione Lavatrice
- Schede Lavatrice con tipologia, formati multipli, quantità/unità, numero lavaggi, EAN, fotografia per formato, prezzo normale/offerta e scorta per formato.
- Scorta generale per anagrafica con soglia minima e comandi rapidi +/− nel catalogo prodotti.
- Migrazione compatibile: i campi nuovi vengono inizializzati senza rimuovere quelli esistenti.
- La chiave localStorage resta `spesaBudgetData`.
