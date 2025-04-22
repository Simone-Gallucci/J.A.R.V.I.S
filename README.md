# 🤖 J.A.R.V.I.S. — Assistente Virtuale Intelligente

J.A.R.V.I.S. (Just A Rather Very Intelligent System) è un assistente virtuale personale programmabile, modulare e multi-piattaforma, ispirato all’iconico Jarvis di Tony Stark. Funziona sia da terminale (Linux/Windows) che su Telegram.

## 🚀 Caratteristiche

- ✅ Riconoscimento linguaggio naturale (nome, età, indirizzo, preferenze…)
- ✅ Compatibile con **Windows, Linux e Telegram**
- ✅ Gestione di:
  - 📅 Eventi (con data e titolo)
  - 🗒️ Appunti (con titolo e testo)
  - 📁 Progetti (con cartelle e file associati)
- ✅ Memoria persistente (nome, preferenze, scuola, ecc.)
- ✅ Creazione e lettura file `.txt`
- ✅ Navigazione tra cartelle come un file manager
- ✅ Comandi vocali (in sviluppo)
- ✅ Integrazione con OpenRouter / GPT tramite `gpt_module.py`

---

## 🧩 Struttura del progetto

```
J.A.R.V.I.S/
├── main.py                  # Avvio del Jarvis da terminale
├── core.py                  # Funzioni principali: memoria, file, comandi
├── telegram_bot.py          # Avvio come bot Telegram
├── memory_manager.py        # Gestione memoria utente su file JSON
├── gpt_module.py            # Collegamento con OpenRouter/AI
├── risposte_preimpostate.py #Risposte automatiche custom
└── Jarvis/                  # Cartella con sottocartelle progetti/eventi/appunti
```

---

## ⚙️ Requisiti

- Python 3.8+
- `python-telegram-bot`
- `requests` (per OpenRouter)
- `readline` (già incluso su Unix)

Installa tutto con:

```bash
pip install -r requirements.txt
```

---

## 🖥️ Uso da Terminale

```bash
python main.py
```

**Esempi comandi da terminale:**
- `mi chiamo Marco`
- `ho 21 anni`
- `mi piace programmare e guardare film`
- `crea appunto Lista della spesa`
- `entra nella cartella progetti`
- `leggi file progetto1.txt`

---

## 💬 Uso su Telegram

Avvia `telegram_bot.py`, configura il tuo token e inizia a chattare con Jarvis!

**Esempi comandi da Telegram:**
- `crea progetto AI_Bot`
- `crea file codice.txt`
- `elimina appunto Lista della spesa`
- `che preferenze ho?`
- `dove vivo?`

---

## 🧠 Memoria

Jarvis ricorda:
- 🧍 Nome
- 🎂 Età
- 🏠 Indirizzo o città
- 🎓 Scuole frequentate
- ❤️ Preferenze personali

Puoi cancellare tutto con:
```
protocollo tabula rasa
```

---

## 🛡️ Licenza

Distribuito sotto licenza **MIT**. Usalo, modificalo e contribuisci!

---

## 👨‍💻 Autore

Creato con ❤️ da **Szymon** — un assistente degno di Iron Man!
