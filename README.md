# 📄 PDF Editor Web

Editor PDF avanzato completamente web-based, progettato per modificare spartiti musicali e documenti PDF direttamente nel browser senza installazioni.

## ✨ Caratteristiche principali

### 🔓 Gestione PDF protetti
- **Importazione automatica** di PDF con protezione/encryption
- **Conversione intelligente** in immagini ad alta qualità (scala 4.5)
- **Nessuna pagina bianca** durante l'export

### 📝 Editing avanzato

#### 🔄 Rotazione
- Rotazione rapida 90° sinistra/destra
- **Rotazione fine** con slider (-10° a +10°, step 0.5°)
- Griglia di riferimento per allineamento preciso

#### ✂️ Ritaglio
- Ritaglio manuale con handles ridimensionabili
- **Auto-raddrizza** con rilevamento automatico degli angoli

#### 🎨 Filtri colore
- Regolazione contrasto (50%-150%)
- Regolazione luminosità (50%-150%)
- Anteprima in tempo reale

#### 🔍 Zoom e visualizzazione
- Zoom 25%-200% per editing preciso
- Miniature ridimensionabili (50px-300px)
- Anteprima sempre ad alta qualità

### 💾 Export intelligente

#### PDF non protetti
- **Mantiene qualità vettoriale originale** se senza modifiche
- Dimensione file identica all'originale
- Solo le pagine modificate vengono convertite in immagini

#### PDF protetti
- Tutte le pagine convertite in immagini JPEG ad alta qualità
- Compressione ottimizzata (qualità 60%)
- File più grande ma completamente funzionante

### 🎯 Gestione pagine
- **Drag & drop** per riordinare
- **Selezione multipla** (Ctrl+Click, Shift+Click)
- Duplica, elimina, rinumera pagine
- Operazioni batch su selezioni multiple

### ↩️ Undo/Redo
- Sistema di history completo (max 50 stati)
- Scorciatoie tastiera (Ctrl+Z, Ctrl+Y)
- Salvataggio intelligente degli stati

## 🚀 Utilizzo

### Importazione
1. Clicca su **"📁 Carica file"** o trascina file nell'area
2. Supporta: PDF, PNG, JPG, JPEG, WEBP
3. Importazione multi-pagina per PDF

### Editing
1. Clicca su una miniatura per selezionare la pagina
2. Clicca su un tab (Rotazione/Ritaglio/Colori/Zoom) per attivare gli strumenti
3. Applica le modifiche desiderate
4. Le modifiche si vedono in tempo reale nell'anteprima

### Export
1. Clicca su **"💾 Esporta PDF"**
2. Scegli un nome file
3. Download automatico del PDF modificato

## 🔧 Tecnologie utilizzate

- **pdf-lib** (1.17.1) - Manipolazione PDF
- **PDF.js** (3.11.174) - Rendering PDF ad alta qualità
- **jsPDF** (2.5.1) - Creazione PDF
- HTML5 Canvas API - Processing immagini
- Vanilla JavaScript - Nessun framework pesante

## 📊 Comportamento conversione

### Quando converte in immagini:
- ✅ PDF con protezione/encryption
- ✅ Rotazione fine applicata (≠ 0°)
- ✅ Filtri colore applicati (≠ 100%)
- ✅ Ritaglio applicato
- ✅ Auto-raddrizza applicato

### Quando mantiene vettoriale:
- ✅ PDF non protetto senza modifiche
- ✅ Solo rotazioni 90° (no rotazione fine)
- ✅ Solo riordinamento pagine
- ✅ Duplicazione pagine

## ⚙️ Parametri di qualità

### Rendering PDF
- Scala: 3.5x per anteprima
- Scala: 4.5x per conversione immagini

### Compressione JPEG
- Qualità originale: 98%
- Qualità export: 60%
- Formato: image/jpeg

### Miniature
- Scala: 0.5x
- Qualità: 70%
- Altezza default: 150px

## 💡 Tips & Tricks

1. **Per file pesanti**: Riduci la qualità JPEG nel codice (riga ~COMPRESSION_QUALITY)
2. **Per rotazioni veloci**: Usa i pulsanti 90° invece della rotazione fine
3. **Per selezioni multiple**: Ctrl+Click per aggiungere, Shift+Click per range
4. **Per UNDO**: Ctrl+Z funziona anche con la tastiera
5. **PDF protetti**: Si aprono normalmente, ma l'export sarà più grande

## 🐛 Limitazioni note

- **UNDO**: Dopo Undo, potrebbe essere necessario ricliccare sulla miniatura per vedere l'anteprima aggiornata
- **Rotazione fine**: La prima applicazione su PDF richiede conversione (1-2 secondi)
- **File size**: PDF protetti diventano più grandi dopo l'export (conversione immagini)

## 📝 Note

- **Single-file app**: Tutto in un unico file HTML
- **100% client-side**: Nessun dato caricato su server
- **Privacy first**: Tutto il processing avviene nel browser
- **No installation**: Funziona direttamente aprendo il file HTML

## 📄 Licenza

MIT License - Libero per uso personale e commerciale

## 🤝 Contributi

Contributi benvenuti! Apri una issue o pull request su GitHub.

---

**Versione**: 2.0  
**Ultimo aggiornamento**: Novembre 2024  
**Browser supportati**: Chrome, Firefox, Edge, Safari (moderne versioni)
