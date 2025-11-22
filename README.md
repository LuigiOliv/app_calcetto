# ⚽ Calcetto Rating App

App per valutare i compagni di calcetto e bilanciare le squadre.

---

## 📁 Struttura

```
calcetto-app/
├── index.html    ← Apri questo nel browser!
├── styles.css    ← CSS separato (facile da modificare)
└── README.md     ← Questo file
```

---

## 🚀 Come Usare

1. **Apri `index.html`** nel browser (doppio click)
2. Inserisci la tua email per accedere
3. Associa il tuo profilo (prima volta)
4. Inizia a votare!

---

## 👥 Sviluppo Collaborativo

### Chi lavora su cosa:

| Persona | File | Cosa modifica |
|---------|------|---------------|
| **Grafico** | `styles.css` | Colori, font, layout |
| **Tutti** | `index.html` | Logica e componenti |

### Come Collaborare:

1. **BACKUP** → Prima di modificare, copia l'intera cartella
2. **MODIFICA** → Lavora sulla tua copia locale
3. **TESTA** → Apri index.html e verifica che funzioni
4. **CARICA** → Se funziona, sostituisci nella cartella condivisa
5. **AVVISA** → Scrivi nel gruppo cosa hai modificato

---

## 📝 Guida alle Sezioni (index.html)

L'HTML è organizzato in **15 sezioni** chiaramente marcate:

| Sezione | Riga ~  | Cosa contiene |
|---------|---------|---------------|
| 1 | ~25 | **CONFIGURAZIONE** - Giocatori, skill, ruoli |
| 2 | ~75 | **STORAGE** - Funzioni localStorage |
| 3 | ~95 | **UTILITIES** - Calcoli medie e overall |
| 4 | ~130 | **LOGIN PAGE** - Pagina di accesso |
| 5 | ~165 | **CLAIM MODAL** - "Chi sei?" |
| 6 | ~220 | **ROLE MODAL** - Selezione ruoli |
| 7 | ~280 | **HEADER** - Barra superiore |
| 8 | ~310 | **PLAYERS LIST** - Griglia giocatori |
| 9 | ~355 | **RATING FORM** - Form votazione |
| 10 | ~420 | **RADAR CHART** - Grafici pentagono |
| 11 | ~480 | **PLAYER PROFILE** - Profilo con grafici |
| 12 | ~560 | **CLASSIFICHE** - Classifica generale |
| 13 | ~630 | **SETTINGS** - Impostazioni utente |
| 14 | ~720 | **ADMIN PAGE** - Pannello admin |
| 15 | ~850 | **APP** - Componente principale |

### Per trovare una sezione:

Cerca nel file: `SEZIONE 1:` oppure `SEZIONE 14:` ecc.

---

## 🎨 Modificare gli Stili (styles.css)

### Cambiare colori principali:

```css
/* Trova queste righe e cambia i colori */
#667eea  →  colore primario (viola)
#764ba2  →  secondo colore gradiente
#48bb78  →  verde (tattiche)
#f56565  →  rosso (fisiche)
```

### Cambiare font:

```css
body {
    font-family: 'Arial', sans-serif;  /* Cambia qui */
}
```

---

## ⚙️ Aggiungere un Giocatore (index.html)

Trova **SEZIONE 1: CONFIGURAZIONE** e aggiungi alla lista `INITIAL_PLAYERS`:

```javascript
{ id: 'player19', name: 'Mario Rossi', avatar: null, preferredRole: null, otherRoles: [] },
```

---

## 🔧 Account Admin

**Email admin:** luigi.oliviero@gmail.com

L'admin può:
- ✏️ Modificare nomi
- 📊 Modificare valutazioni
- 🗑️ Eliminare giocatori
- ➕ Aggiungere giocatori

Per cambiare admin, modifica in SEZIONE 1:
```javascript
const ADMIN_EMAIL = 'nuova.email@esempio.com';
```

---

## 🐛 Problemi?

### L'app non carica:
- Prova Chrome o Firefox
- Svuota cache: `Ctrl+Shift+R`

### Dati corrotti:
- Apri console (F12)
- Digita: `localStorage.clear()`
- Ricarica pagina

---

**Versione:** 2.1  
**Ultimo aggiornamento:** Novembre 2024
