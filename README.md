# Spesa — Budget V10.1

Versione V10.1, aggiornamento grafico e funzionale della V10.0, costruita sul progetto completo V9.0. Sono mantenuti `index.backup.html`, manifest, service worker e README; la chiave di archiviazione resta `spesaBudgetData`.

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
