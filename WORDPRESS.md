# Come mettere questa pagina su alislam.it (WordPress)

La pagina è pronta in due forme. Prima fate vedere la versione online (link GitHub Pages) per l'approvazione, poi pubblicate così.

## Metodo A – blocco "HTML personalizzato" (consigliato)
1. In WordPress: **Pagine → Aggiungi nuova**, titolo «Rishta Nata – moduli e istruzioni».
2. Aggiungete un blocco **HTML personalizzato** (cercate "HTML").
3. Aprite `wordpress/rishta-nata-embed.html` in questo repository, cliccate **Raw**, copiate tutto e incollate nel blocco.
4. Caricate i PDF nella **Libreria media** (cartella `forms/`). Poi, nel codice incollato, cambiate la riga `var RN_BASE='...'` con l'indirizzo della cartella dei PDF (es. `https://alislam.it/wp-content/uploads/2026/11/`). Se i PDF restano su GitHub, non cambiate nulla.
5. **Anteprima**, poi **Pubblica**.

Gli stili sono isolati (`.rn`), quindi non cambiano il resto del sito.

## Metodo B – incorporare (iframe), senza copiare nulla
Blocco HTML personalizzato con:
`<iframe src="https://ataulwasihtariq.github.io/rishta-nata/" style="width:100%;height:2400px;border:0" title="Rishta Nata"></iframe>`
Più veloce, ma la pagina vive su GitHub (meno bene per SEO).

## Se il blocco HTML non è disponibile
Con alcuni ruoli WordPress lo script viene rimosso. In quel caso chiedete all'amministratore di incollarlo, o di caricare la cartella intera con FTP in `/rishta-nata/`.

Nota: nessun modulo compilato va mai caricato. Qui ci sono solo moduli vuoti.
