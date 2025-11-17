# 📤 Come caricare su GitHub

## Metodo 1: Interfaccia Web (più facile)

### Passo 1: Crea un nuovo repository
1. Vai su https://github.com e fai login
2. Clicca sul "+" in alto a destra → "New repository"
3. Dai un nome (es: "spartiti-pdf-editor")
4. Lascia Public (o scegli Private se vuoi)
5. ✅ Spunta "Add a README file"
6. Clicca "Create repository"

### Passo 2: Carica i file
1. Nel repository, clicca "Add file" → "Upload files"
2. Trascina questi file:
   - `index.html`
   - `icon-180.png`
3. Scrivi un messaggio (es: "Prima versione")
4. Clicca "Commit changes"

### Passo 3: Sostituisci il README
1. Clicca sul file `README.md` esistente
2. Clicca sull'icona della matita (Edit)
3. Sostituisci tutto il contenuto con quello del file README.md che hai
4. Clicca "Commit changes"

### Passo 4: Pubblica su GitHub Pages (opzionale)
1. Vai su "Settings" del repository
2. Clicca "Pages" nel menu laterale
3. Sotto "Source" seleziona "main" branch
4. Clicca "Save"
5. Dopo qualche minuto, il sito sarà online a:
   `https://tuousername.github.io/spartiti-pdf-editor`

---

## Metodo 2: Da Terminale (per utenti avanzati)

Se hai Git installato:

```bash
# 1. Vai nella cartella con i file
cd /percorso/dei/tuoi/file

# 2. Inizializza Git
git init

# 3. Aggiungi i file
git add index.html icon-180.png README.md .gitignore

# 4. Crea il primo commit
git commit -m "Prima versione dell'editor spartiti"

# 5. Collega al repository GitHub (sostituisci USERNAME e REPO)
git remote add origin https://github.com/USERNAME/REPO.git

# 6. Carica i file
git branch -M main
git push -u origin main
```

---

## ✅ File da caricare

Assicurati di caricare questi file:
- ✅ `index.html` (il file principale)
- ✅ `icon-180.png` (l'icona dell'app)
- ✅ `README.md` (la documentazione)
- ✅ `.gitignore` (opzionale)

---

## 🌐 Condividere l'app

Dopo aver caricato su GitHub Pages, puoi condividere il link:
- Apri il link su Safari (iPad)
- "Condividi" → "Aggiungi a Home"
- L'app è installata! 🎉

---

## 🆘 Problemi comuni

**"GitHub Pages non funziona"**
- Aspetta 5-10 minuti dopo l'attivazione
- Controlla che il branch sia "main" e non "master"
- Il file DEVE chiamarsi `index.html` (minuscolo)

**"L'icona non appare"**
- Controlla che `icon-180.png` sia nella stessa cartella di `index.html`
- Ricarica la pagina con Ctrl+F5 o Cmd+Shift+R

**"I file sono troppo grandi"**
- GitHub ha un limite di 100 MB per file
- Il tuo index.html e icon dovrebbero essere molto sotto questo limite
