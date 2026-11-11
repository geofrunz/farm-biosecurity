# Farm Biosecurity Designer — scenari JSON scelti dal docente

Questo sito funziona con GitHub Pages e mostra **solo i file JSON presenti nella cartella `scenari/`**. Non contiene scenari predefiniti.

## Prima pubblicazione

1. Estrai `Farm_Biosecurity_Scenari_Dinamici_GitHub.zip`.
2. Crea un repository pubblico GitHub, per esempio `farm-biosecurity`.
3. Carica **nella radice del repository** il file `index.html`, `simulatore.html`, questo README e **la cartella `scenari/`** (contiene inizialmente soltanto `.gitkeep`).
4. Nelle impostazioni del repository scegli **Settings → Pages → Build and deployment → Source: Deploy from a branch → main → /(root) → Save**.
5. Abilita GitHub Actions se necessario per l'elaborazione Jekyll. **Non aggiungere `.nojekyll`**: Jekyll serve per riconoscere automaticamente tutti i JSON disponibili.
6. Dopo la pubblicazione, apri l'indirizzo fornito da GitHub Pages e genera **un solo QR code per quell'indirizzo**.

## Per aggiungere uno scenario

1. Apri il simulatore **DOCENTE** sul tuo computer.
2. Prepara e approva la base con **Blocca strutture · Avvia esercizio**, quindi premi **Salva progetto**.
3. Rinomina il file con un nome utile, per esempio `Gruppo_1.json` oppure `Allevamento_polli.json`.
4. Su GitHub apri la cartella `scenari/` e scegli **Add file → Upload files**.
5. Carica il JSON, poi conferma con **Commit changes**.
6. Terminata la pubblicazione GitHub Pages, il nuovo scenario compare nella lista pubblica, con nome derivato dal nome del file (gli underscore diventano spazi).

## Aggiornare, rimuovere o aggiungere più scenari

- **Aggiungere:** carica un altro `.json` nella stessa cartella.
- **Sostituire una base:** sostituisci il file con **lo stesso nome** nella cartella `scenari/`, poi fai commit. Se l'interfaccia GitHub non offre la sostituzione diretta, elimina il vecchio e carica il nuovo nello stesso percorso.
- **Rimuovere:** elimina il file `.json` dalla cartella e fai commit.
- **Ordine:** gli scenari sono mostrati per nome file in ordine alfabetico. Usa `01_`, `02_`, `03_` per ordinarli.

L'indirizzo del sito e il QR code **restano identici** quando cambiano i JSON. I cambiamenti saranno visibili nei nuovi accessi dopo la pubblicazione; non modificano automaticamente lavori già aperti o file JSON già scaricati dagli studenti.

## Cosa fanno gli studenti

1. Aprono il QR code e vedono **soltanto gli esercizi che hai caricato**.
2. Premono **Apri il simulatore**: la base viene caricata automaticamente.
3. Aggiungono interventi (nuove strutture, ampliamenti e demolizioni con costo), percorsi, barriere e dispositivi.
4. Con **Salva progetto** scaricano il JSON finale sul loro dispositivo.
5. Con **Apri JSON** possono riaprire un lavoro già salvato.
6. Consegnano il file usando Moodle, Teams o altro canale che indichi tu.

## Requisiti dei JSON

I JSON devono essere file di progetto validi creati dal **simulatore docente** e salvati **dopo la conferma della base**. Un JSON di sola configurazione, non approvato, non viene aperto dalla versione studenti.

## Limiti importanti

- **GitHub Pages è un sito pubblico:** chiunque abbia il link può visualizzare e scaricare i JSON pubblicati. Non pubblicare informazioni riservate o dati personali.
- Gli studenti vedono e aprono dal sito **solo i JSON pubblicati**, ma possono sempre importare un proprio file JSON locale per riprendere il lavoro. Questo è intenzionale.
- Non caricare l'applicazione docente nel repository pubblico.
- Il sito non raccoglie automaticamente i lavori. Il QR code permette l'accesso, non la consegna.
- I nomi dei JSON devono essere univoci e terminare con `.json`; evita caratteri speciali complicati. Per i titoli degli scenari usa i nomi file.
- GitHub Pages va usato con il generatore **Jekyll attivo**; per questo il pacchetto non ha `.nojekyll`.
