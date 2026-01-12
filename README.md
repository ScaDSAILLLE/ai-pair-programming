# Willkommen beim ai-pair-programming Workshop: Co-Coding mit KI zum programmieren lernen oder um kleine Projekte á la *vibe coding*. 
**Viel Spaß!** \
*Weitere Infos findest du in der [Präsentation](260115_scads_ai_pair_programming_workshop.pdf)*

---

## 📚 Table of Contents

* [Einführung](#einfuehrung)
* [Tools](#tools)

  * [VOID](#void)
  * [Goose](#goose)
  * [opencode](#opencode)
* [Beispiele & Tutorials](#beispiele--tutorials)
* [Ablauf des Workshops](#ablauf-des-workshops)
* [Lizenz](#lizenz)

---

## 🛠️ <a name="einfuehrung">Einführung</a>

Dieses Repository enthält **alles, was ihr für den Vibe Coding Contest benötigt**:

* Installations- & Setup-Guides
* Beispielprojekte & Tutorials
* Vorlagen für Präsentationen
* Hinweise zu API-Keys & Modellnutzung
* Best Practices für AI-gestütztes Pair & Vibe Coding

Das Material entstand im Rahmen des **ScaDS.AI Meetups „Vibe Coding Contest“**.
👉 *Der direkte Repo-Link ist auf Slide 14 der Intro-Präsentation zu finden.*

---

## 🧰 <a name="tools">Tools</a>

Im Workshop arbeiten wir mit **drei komplementären AI-Coding-Tools**, die bewusst **unterschiedliche Paradigmen** abdecken:

---

### <a name="void">VOID</a>

➡️ **Ordner im Repo:** `/1_void`
➡️ **Website:** [https://voideditor.com/](https://voideditor.com/)

VOID ist ein **Open-Source AI Code Editor**, basierend auf VS Code – vergleichbar mit Cursor, aber **kostenlos und offen**.

**Kurzüberblick:**

* Klassische **VS-Code-UX** mit integrierten LLM-Features
* Inline-Coding, Chat, Refactoring, Explain, Generate
* Alternative zu Cursor / GitHub Copilot
* **Model-agnostisch:**
  OpenAI, Claude, lokale Modelle (Ollama, vLLM, LM Studio), OpenAI-kompatible APIs
* Ideal für **klassisches Pair Programming mit KI**

➡️ Vollständige Setup- & Nutzungsanleitungen im `/1_void`-Ordner.

---

### <a name="goose">Goose</a>

➡️ **Ordner im Repo:** `/2_goose`
➡️ **Docs:** [https://block.github.io/goose/](https://block.github.io/goose/)

Goose ist **kein IDE-Plugin**, sondern ein **eigenständiger AI-Agent-Workspace** (Desktop & CLI).

**Charakteristika:**

* **Task- & Conversation-Driven UI** statt Datei-/Editor-Fokus
* Arbeit beginnt mit einer **natürlichen Aufgabenbeschreibung**, nicht mit Codezeilen
* Unterstützt **agentische Workflows** für Development & Automatisierung

**Besondere Features:**

* **Recipes:**
  Wiederverwendbare, strukturierte Agent-Workflows (z. B. Project-Setup, Refactoring, Analysen)
* **Automatisch gespawnte Sub-Agents:**
  Goose erzeugt aus natürlicher Sprache spezialisierte Agenten (z. B. Recherche, Coding, Review)
* **Explizite Tool- & Execution-Kontrolle:**
  File-Writes, Commands, Netzwerkzugriffe sind sichtbar und nachvollziehbar

**Modell-Support:**

* OpenAI, Anthropic
* OpenAI-kompatible APIs (z. B. KIARA, LM Studio, Ollama)

➡️ Setup- & Nutzungsanleitungen im `/2_goose`-Ordner.

---

### <a name="opencode">OpenCode</a>

➡️ **Ordner im Repo:** `/3_opencode`
➡️ **Docs:** [https://opencode.ai/docs](https://opencode.ai/docs)

OpenCode ist ein **AI Coding Agent**, mit dem du deine Projekte und Code-Ideen gemeinsam umsetzen kannst.

**Was OpenCode auszeichnet:**

* **Agent statt Editor-Feature:**
  OpenCode arbeitet auf Repository-Ebene und versteht Projektstruktur, Kontext und Historie
* **Plan → Execute → Iterate:**
  Aufgaben werden geplant, umgesetzt und gemeinsam mit dem Menschen iterativ verfeinert
* **Explizite Agent-Aktionen:**
  File-Änderungen, Commands, Refactorings sind transparent und steuerbar; zahlreiche nützliche *Slash (/) commands*
* **Ideal für größere Tasks:**
  Features, Bugfixes, Migrationen, Refactorings

**Technisch:**

* CLI-basiert / Desktop Variante vorhanden
* Model-agnostisch (lokal & Cloud)
* Stark geeignet für **AI Pair Programming jenseits von Autocomplete**; state-of-the-art features, wie skills, plugins & starke (open-source) community

➡️ Setup- & Nutzungsanleitungen im `/3_opencode`-Ordner.

---

## 🎮 <a name="beispiele--tutorials">Beispiele & Tutorials</a>

➡️ **Ordner:** `/4_beispiele_fuers_vibe_coding`

Die Beispiele sind so gewählt, dass ihr **schnell ins Tun kommt**, unabhängig vom Tool:

---

### Beispiel 1 – TicTacToe

Varianten:

* Python in der Goose-Sandbox
* HTML + CSS + JS in VOID

➡️ Enthält ein **vollständiges Anfänger-Tutorial**.

---

### Beispiel 2 – Virtuelle Klaviatur

Ein interaktives Web-Instrument (JS + HTML + Audio).
Ideal für UI-Experimente und KI-gestützte Erweiterungen.

---

### Beispiel 3 – Programmieren lernen mit KI (Python)

Ein interaktiver Einstieg in Python:
Lernen über Chat, Beispiele und gemeinsames Coden mit dem Agenten.

---

## 🧩 <a name="ablauf-des-workshops">Ablauf des Workshops</a>

* Findet euch in Teams oder arbeitet alleine
* Macht euch mit **VOID, Goose & OpenCode** vertraut
* Nutzt die Beispiele oder bringt eigene Ideen ein
* **Ausprobieren → Lernen → Iterieren**
* Fragen, Ideen & Zwischenergebnisse jederzeit teilen 😉
* Ziel: Spaß haben **und** Inspiration für ein eigenes AI-Coding-Setup mitnehmen

---

## 🤖 Empfohlene Modelle

* **KIARA:** `vllm-meta-llamna-llama-3-3-70b-instruct`
  *(URZ-gehostetes LLM-Cluster, free)*

* **Mistral:** `devstral-2512`
  *(aktuelles Coding-LLM, Stand 01/2026 ebenfalls free)*

* **OpenAI:** `gpt-5.1-codex-max`
  Input: ~$1.25 / MTok · Output: ~$10 / MTok

* **Anthropic:** `claude-sonnet-4-5`
  Input: ~$3 / MTok · Output: ~$15 / MTok

---

## 📜 <a name="lizenz">Lizenz</a>

Workshop-Material steht unter **CC BY 4.0**, Oliver Welz\
Code: MIT-Lizenz (see [LICENSE](LICENSE.md))

---
