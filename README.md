# database-immagini

Archivio pubblico di immagini originali delle fonti, organizzato per la ricerca editoriale e l'utilizzo dei collegamenti Raw.

**1490 immagini uniche**, **1556 associazioni alle notizie**. I duplicati binari condividono lo stesso file conservando tutte le fonti.
Sono escluse grafiche AI e caroselli creati da noi, anteprime di QA e contenuti privati del workspace. La tecnica usata dalle fonti per creare le loro immagini non è stata verificata.
I blocchi GPS eventualmente presenti sono rimossi dalle sole copie pubbliche; il flusso JPEG non viene ricodificato e i pixel sono verificati identici. I crediti non sono rimossi.

## Trova un'immagine

- [Catalogo JSON per IA e automazioni](catalogo/immagini.json)
- [Catalogo CSV con tutti i link Raw](catalogo/immagini.csv)
- [Statistiche e copertura](catalogo/statistiche.json)
- `index.html`: galleria con ricerca, filtri e copia del link Raw; scaricare il repository e aprire il file nel browser. GitHub Pages non è attivato.

- [videocardz.com](catalogo/fonti/videocardz-com.md): 143 associazioni immagine/notizia.
- [tomshardware.com](catalogo/fonti/tomshardware-com.md): 514 associazioni immagine/notizia.
- [techpowerup.com](catalogo/fonti/techpowerup-com.md): 627 associazioni immagine/notizia.
- [guru3d.com](catalogo/fonti/guru3d-com.md): 266 associazioni immagine/notizia.
- [ollama.com](catalogo/fonti/ollama-com.md): 2 associazioni immagine/notizia.
- [reactos.org](catalogo/fonti/reactos-org.md): 1 associazioni immagine/notizia.
- [eu.store.ui.com](catalogo/fonti/eu-store-ui-com.md): 1 associazioni immagine/notizia.
- [anbernic.com](catalogo/fonti/anbernic-com.md): 1 associazioni immagine/notizia.
- [github.com](catalogo/fonti/github-com.md): 1 associazioni immagine/notizia.

## Struttura e link

`immagini/canale/fonte/anno/mese/data_argomento_hash.estensione`

Ogni immagine ha un identificatore SHA256 e un nome che include parte dell'hash. Non rinominare, sovrascrivere o cancellare immagini già usate nei post: aggiungere un nuovo file per ogni versione.
`raw_url` è l'indirizzo diretto, accessibile senza login. `raw_url_immutabile`, quando presente, punta al commit che conserva la versione verificata.
Usare questi URL nei campi media dello strumento di pubblicazione. Incollare un URL nel testo di un post non equivale a caricare l'immagine.

## Come scegliere per articoli e news

Il JSON separa `images` (file unici) da `news` (contesti editoriali). Cercare titolo, fonte o `keywords_it`, collegare `news.image_id` a `images.image_id`, leggere fonte e dimensioni, quindi usare il Raw.
Le parole chiave sono ricavate automaticamente dal titolo e vanno valutate nel contesto. Non sono una descrizione visiva verificata né un alt text pronto.
La qualità `miniatura` indica un lato inferiore a 300 px; `media` almeno 300 px su entrambi i lati; `alta` almeno 600 px su entrambi i lati. Sono soglie di selezione interne, non certificazioni di compatibilità social.

## Provenienza e copertura

Web: copertine già archiviate per le notizie dal 17 agosto al 15 settembre 2026 dei quattro siti scelti. Il catalogo originario comprende 1641 schede, di cui 91 senza immagine recuperata; non si tratta di tutte le fotografie interne agli articoli.
Newsletter: immagini originali recuperate dalle pagine pubbliche delle cinque notizie già archiviate il 18 settembre. Nessuna nuova scansione della casella email. La data di riferimento di questi file indica l'edizione editoriale, non la data originale della fotografia.
`missing_images` mantiene le schede web prive di copertina, senza inventare link Raw.

## Crediti e diritti

La fonte editoriale e l'URL originale sono conservati; l'autore della singola foto non viene inventato. Le immagini restano dei rispettivi titolari. L'accessibilità pubblica o la presenza di un Raw non costituisce una licenza di riutilizzo: `rights_status` resta `da_verificare` dove la licenza non è documentata.
Il repository non attribuisce una licenza libera alle immagini di terzi.

## Aggiornamenti

Questa è una raccolta puntuale. Nessuna sincronizzazione automatica, nuova iscrizione a newsletter o pubblicazione social è attivata. Per aggiungere immagini seguire AGENTS.md e aggiornare i cataloghi senza alterare i collegamenti esistenti.
