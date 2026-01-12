# **Workshop-Aufgabe: Python für Anfänger – mit Coding Agent**

Ziel: Du baust in kurzer Zeit ein **mini Python-Projekt**, lernst **Variablen, Funktionen, Bedingungen, Listen** – und übst, wie man mit einem Coding Agent **richtig** arbeitet: nachfragen, testen, kleine Schritte.

Wir arbeiten nach Best Practice:

* **eigener Projektordner**
* **uv-Umgebung** (oder venv)
* **kleine Schritte + Rückfragen**
* **Hands-on Mini-Tasks**

---

## 📁 **1) Projekt anlegen (1 Min)**

Ordner erstellen, z. B.:

```bash
mkdir -p ~/vibe_projects/python_intro
cd ~/vibe_projects/python_intro
```

👉 Öffne diesen Ordner in deinem Tool (Goose/OpenCode/VOID).

---

## 🐍 **2) Python-Umgebung mit uv (2–3 Min)**

**Prompt an den Coding Agent:**

> Erstelle mir in diesem Ordner eine moderne Python-Projektstruktur mit `uv`:
>
> * `pyproject.toml` minimal
> * virtuelle Umgebung
> * eine Datei `main.py`
>   Bitte erkläre kurz, welche Befehle du nutzt und wie ich sie ausführe.

Typische Befehle (Agent soll sie dir geben, du führst sie aus):

```bash
uv init
uv venv
```

**Mini-Task (du!):**
👉 Frage nach: „Wofür ist eine virtuelle Umgebung gut?“
👉 Lass dir erklären, wie man sie aktiviert (oder wie uv sie automatisch nutzt).

---

## ✅ **3) Dein erstes Programm: “Greeter” (5 Min)**

**Prompt an den Coding Agent:**

> Lege `main.py` an, die Folgendes macht:
>
> 1. Fragt den Namen per `input()` ab
> 2. Gibt „Hallo <Name>!“ aus
> 3. Wenn der Name leer ist, soll „Hallo Stranger!“ kommen
>    Bitte erkläre den Code zeilenweise.

**Starte es (Agent soll dir den genauen Befehl sagen):**
z. B.

```bash
python main.py
```

**Mini-Task (du!):**

* Ändere „Stranger“ zu „Vibe Coder“.
* Frage den Agenten: „Warum braucht `input()` immer einen String?“

---

## 🔁 **4) Wiederholung/Übung: kleine Aufgaben (5–7 Min)**

Jetzt bewusst **selbst** kleine Änderungen machen. Wenn du hängen bleibst: fragen.

### Aufgabe A (leicht)

* Frage ein Alter ab
* Wenn Alter < 18 → „Du bist noch nicht volljährig.“
* Sonst → „Willkommen im Erwachsenenleben.“

### Aufgabe B (leicht)

* Lege eine Liste an: `hobbies = ["music", "sports", "coding"]`
* Lass den Nutzer ein Hobby eingeben
* Prüfe, ob es in der Liste ist → Ausgabe „Cool!“ / „Auch spannend!“

**Wichtig: Rückfragen üben (du!)**
Frag den Agenten z. B.:

* „Welche Datentypen haben `age` und `input()`?“
* „Warum brauche ich `int()`?“
* „Wie debugge ich das, wenn ein ValueError kommt?“

---

## ⭐ **5) Goodie (5–8 Min): Mini-Webseite mit FastAPI (optional, fühlt sich nach “wow” an)**

Ziel: Eine kleine Web-App lokal: **Name eingeben → HTML Greeting**
*(Wenn die Zeit knapp ist, nur starten lassen und kurz zeigen.)*

### Prompt-Vorlage (copy-paste)

> Baue mir ein Mini-Projekt mit **FastAPI + Templates** in diesem Ordner:
>
> * `uv`-Setup (falls noch nicht)
> * Abhängigkeiten installieren: fastapi, uvicorn, jinja2
> * Ordnerstruktur:
>
>   * `app.py`
>   * `templates/index.html` (Formular mit Name)
> * Route `GET /`: zeigt Formular
> * Route `POST /greet`: nimmt Name und rendert HTML mit „Hallo <Name>!“
>   Bitte gib mir einen **Step-by-step Guide**, wie ich das starte (inkl. uv-Befehle) und wie ich es im Browser nutze.

**Wichtig:** Lass den Agenten **wirklich erklären**:

* welche Commands er nutzt (uv add / uv run)
* wie du startest
* welche URL im Browser

*(Der Agent sollte sowas liefern wie: `uv add fastapi uvicorn jinja2` und dann `uv run uvicorn app:app --reload`.)*

---

## ✔️ Fertig – was du gelernt hast

* wie man ein kleines Python-Projekt sauber startet (Ordner + Environment)
* `input()`, Variablen, `if/else`, Listen, einfache Logik
* **wie man den Coding Agent richtig nutzt**:

  * kleine Schritte
  * testen
  * Rückfragen stellen
  * selbst mini-Änderungen machen

---