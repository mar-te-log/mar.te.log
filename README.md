# Il tuo blog — istruzioni

Questo è un sito Jekyll, il motore di blog gratuito integrato in GitHub Pages.
Non devi installare nulla sul computer: puoi fare tutto dal sito di GitHub, nel browser.

## 1. Crea un account GitHub (se non ce l'hai già)

Vai su https://github.com/join e registrati (gratis). Lo username che scegli qui
diventerà parte dell'indirizzo del tuo blog.

## 2. Crea il repository

1. Vai su https://github.com/new (accedi con l'account il cui username è `marcotedesco135-rgb`)
2. Nome del repository: **`marcotedesco135-rgb.github.io`** (esattamente così — questo nome
   speciale fa sì che GitHub pubblichi il sito automaticamente su
   `https://marcotedesco135-rgb.github.io`)
3. Lascialo **Public**
4. Clicca "Create repository" (non serve aggiungere README, .gitignore o licenza:
   li carichiamo noi)

## 3. Carica i file del sito

1. Nella pagina del repository appena creato, clicca **"uploading an existing file"**
   (o il pulsante "Add file" → "Upload files")
2. Trascina dentro **tutti i file e le cartelle** di questa cartella (`_config.yml`,
   `_layouts`, `_posts`, `_includes`, `assets`, `index.html`, `about.md`, `newsletter.md`,
   `Gemfile`, `.gitignore`, `README.md`)
3. Scorri in basso e clicca **"Commit changes"**

## 4. Attiva GitHub Pages

1. Nel repository, vai su **Settings → Pages** (menu a sinistra)
2. Sotto "Build and deployment", in "Source" scegli **"Deploy from a branch"**
3. In "Branch" scegli **main** e cartella **/ (root)**, poi **Save**
4. Aspetta 1-2 minuti: il tuo sito sarà online su `https://<tuo-username>.github.io`

## 5. Personalizza `_config.yml`

Apri il file `_config.yml` nel repository (icona matita per modificarlo online) e cambia:

- `title` / `tagline` / `description`: già impostati su "mar.te.log" — cambiali se vuoi
- `url`: già impostato su `https://marcotedesco135-rgb.github.io`
- `buttondown_username`: vedi punto 6 (unico campo che manca ancora)

Ogni volta che salvi ("Commit changes"), il sito si aggiorna da solo in 1-2 minuti.

## 6. Attiva la newsletter (Buttondown, gratis fino a 100 iscritti)

1. Vai su https://buttondown.com e crea un account gratuito
2. Scegli il tuo username Buttondown (es. se scegli `marco`, il tuo indirizzo
   sarà `buttondown.com/marco`)
3. Scrivi quel nome utente in `_config.yml` alla voce `buttondown_username`
4. Fatto: il modulo "Iscriviti alla newsletter" sul sito ora funziona. Quando pubblichi
   un nuovo articolo, vai su Buttondown, incolla il testo (o il link all'articolo) e
   invialo agli iscritti — non è automatico, è una scelta voluta: decidi tu quando mandare
   l'email, anche raggruppando più articoli insieme.

## 7. Pubblicare un nuovo articolo

1. Nel repository, vai nella cartella `_posts`
2. Clicca "Add file" → "Create new file"
3. Nome del file: **`AAAA-MM-GG-titolo-breve.md`** (es. `2026-10-03-un-pensiero.md`)
   — la data nel nome del file decide quando appare l'articolo
4. Scrivi il contenuto così:

   ```
   ---
   title: "Titolo del tuo articolo"
   date: 2026-10-03 09:00:00 +0200
   excerpt: "Una riga di anteprima che appare nella lista articoli."
   ---

   Qui scrivi il testo dell'articolo, in Markdown (puoi usare **grassetto**,
   *corsivo*, [link](https://esempio.com), immagini, ecc.)
   ```

5. Commit changes → dopo 1-2 minuti l'articolo è online, in cima alla lista

## 8. La pagina "Chi sono"

Apri `about.md` e scrivi la tua bio (2-4 frasi, resta pure vago/a quanto vuoi:
niente cognome, lavoro o città se non vuoi). Puoi anche rimuovere del tutto la riga
con l'email se preferisci non essere contattabile.

## Note

- Tutto questo è **gratis**: GitHub Pages non ha costi per siti come questo,
  Buttondown è gratis fino a 100 iscritti alla newsletter, e i lettori non pagano nulla.
- Se in futuro vuoi un dominio tuo (es. `tuonome.it`) invece di
  `<username>.github.io`, si può collegare in un secondo momento — non è necessario ora.
- Se preferisci scrivere gli articoli da un editor sul computer invece che dal
  browser di GitHub, puoi anche clonare il repository con Git e usare qualsiasi
  editor di testo: il formato dei file (Markdown) resta lo stesso.
