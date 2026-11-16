# Spesa — Budget V10.2

Versione V10.2, aggiornamento di V10.1 con identità grafica e supporto icone per l’installazione PWA. La base funzionale include le modifiche introdotte in V10.1. Sono mantenuti `index.backup.html`, manifest, service worker e README; la chiave di archiviazione resta `spesaBudgetData`.

## Aggiornamenti V10.1
- Modulo anagrafica più ordinato: identità del prodotto separata dai dati commerciali della confezione.
- Per la categoria Lavatrice, EAN, formato, prezzi e supermercato vengono gestiti nel singolo formato, evitando campi duplicati nell'intestazione.
- Scorta, soglia minima, residuo della confezione aperta, data di apertura e foto restano associati al singolo formato.
- Il numero di lavaggi è un campo del formato.
- Rimosso il campo dose consigliata dalla registrazione del formato; nel registro lavaggi la quantità consumata viene inserita manualmente.
- Le anagrafiche non Lavatrice mantengono il modulo commerciale generale.
- Nessuna modifica alla chiave localStorage `spesaBudgetData`; i dati già presenti nei formati e nello storico vengono mantenuti.

## Compatibilità e limiti
- L'aggiornamento non cancella i dati esistenti e conserva il backup `index.backup.html`.
- Il codice JavaScript e l'integrità dell'archivio ZIP sono verificati staticamente.
- Non è stata completata una prova end-to-end in browser né una verifica su iPhone; si consiglia di provare prima una copia/backup dei dati.
- La scansione OCR degli scontrini e la scansione EAN tramite fotocamera non sono incluse.

## V10.2 — Icona e installazione PWA
- Aggiunte icone PNG 192x192 e 512x512 per la PWA.
- Aggiunta variante maskable 512x512.
- Aggiunta apple-touch-icon 180x180 e favicon 32x32.
- Aggiornati manifest, riferimenti HTML e cache service worker alla V10.2.
- Aggiunta la registrazione del service worker nell’HTML.
- Aggiunta l’icona maskable 512x512 effettivamente richiamata da manifest e cache.
- Il backup index.backup.html è conservato senza modifiche.
