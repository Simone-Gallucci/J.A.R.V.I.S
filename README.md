# J.A.R.V.I.S
A virtual assistant, its name comes from Tony Stark's (IronMan) ally and personal assistant. Inside there will also be a small guide to help you in the first steps of using it.
# 🤖 Jarvis - Assistente Virtuale da Terminale

Jarvis è un assistente virtuale intelligente, sviluppato in Python per funzionare da terminale su Linux (supporta anche Termux e VPS come Hetzner). Ti permette di interagire in modo naturale, gestire eventi, progetti, appunti, e molto altro.

---

## 🚀 Funzionalità principali

### ✅ Comandi naturali
Jarvis comprende frasi del tipo:
- `ciao jarvis`
- `quanti anni ho?`
- `come mi chiamo?`
- `cerca cosa vuol dire json su google`
- `cerca video divertenti su youtube`

### 📚 Gestione della memoria
Jarvis memorizza:
- nome
- età
- indirizzo
- orientamento
- preferenze

E risponde correttamente anche a domande come:
- `come mi chiamo?`
- `qual è il mio orientamento?`

### 🗂 Gestione eventi, progetti e appunti
Usa comandi tipo:
- `/evento aggiungi 25/04 Riunione - Incontro con il team alle 10:00`
- `/progetto aggiungi Sito Portfolio - In costruzione con Flask`
- `/appunto aggiungi JSON - È un formato di interscambio dati`

Puoi anche:
- Visualizzare: `/evento mostra`, `/progetto mostra`, `/appunto mostra`
- Eliminare: `/evento elimina nome`, ecc.

### 🔔 Sveglia/Notifica automatica
Ogni mattina (Lun-Ven) alle 8:00 invia un messaggio di "Buongiorno" (supportato sia da desktop che da Termux con notifica locale).

### 🔄 Comando `/reset`
Per cancellare tutta la memoria salvata per l'utente corrente.

### 🔍 Ricerca Google e YouTube
Interpreta comandi come:
- `cerca yugioh su google`
- `cerca gameplay su youtube`

⚠️ Su server senza interfaccia grafica (es. Hetzner), viene solo stampato il link da aprire manualmente.

### 🧠 IA integrata (via OpenRouter / Mistral / altri)
Jarvis integra una risposta IA per gestire input generici o domande complesse, usando API intelligenti.

---

## 🛠 Requisiti
- Python 3.10+
- pacchetti: `spacy`, `flask`, `webbrowser`, `requests`, ecc.
- Modello italiano per spaCy:
  ```bash
  pip install spacy
  python3 -m spacy download it_core_news_sm
  ```

---

## 📂 Struttura dei file
```
Jarvis/
├── main.py                  # Programma principale
├── comando_cerca.py         # Ricerca Google / YouTube
├── gestione_comando.py      # Comandi naturali
├── comandi_eventi.py        # Eventi
├── comandi_progetti.py      # Progetti
├── comandi_appunti.py       # Appunti
├── mostra_comandi.py        # /help
├── jarvis_core.py           # Memoria, IA e funzioni base
├── sveglia.py               # Notifica del buongiorno
├── config/                  # (opzionale) configurazioni extra
├── memoria.json             # File della memoria utente
```

---

## 💾 Avvio
```bash
python3 main.py
```

---

## 📌 Note
- Supporta `tmux`, `nohup`, `screen` per avvio persistente su server
- Funziona anche su Termux
- La memoria è salvata localmente in `memoria.json`

---

## 📧 Autore
Creato da **Szymon** ✨

Per suggerimenti, migliorie o collaborazione, sentiti libero di aprire una issue o una pull request!
