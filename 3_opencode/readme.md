# **OpenCode Desktop – Installation & Setup Guide**

**OpenCode Desktop** ist ein **lokaler AI Coding Agent**, der als eigenständige Desktop-Anwendung arbeitet (kein IDE-Plugin).
Der Fokus liegt auf **agentischem Pair Programming auf Repository-Ebene**.

OpenCode kombiniert:

* **modellagnostische LLM-Anbindung** (OpenAI, Mistral, Anthropic, OpenAI-kompatibel)
* **Task- & Agent-getriebenes Coding** statt Inline-Autocomplete
* **transparente Agent-Aktionen** (File-Changes, Planung, Iteration)
* **Chat + Repository-Kontext + Agent-Execution**

Dieser Guide führt durch:

1. Installation
2. Auswahl & Konfiguration eines LLM-Providers
3. Erste Funktionstests

---

# **1. Installation**

### **Offizielle Downloads**

Lade **OpenCode Desktop** für dein Betriebssystem herunter:

➡️ **[https://opencode.ai/download](https://opencode.ai/download)**

1. Wähle dein Betriebssystem (macOS / Windows / Linux)
2. Installiere OpenCode wie gewohnt
3. Starte anschließend **OpenCode Desktop**

---

# **2. LLM-Provider auswählen**

OpenCode nutzt **System-weite API-Keys** (Environment Variables).
Wenn diese bereits gesetzt sind, erkennt OpenCode die verfügbaren Provider automatisch.

Unterstützt werden u. a.:

* **Mistral**
* **OpenAI**
* **Anthropic**
* **OpenAI-kompatible APIs** (z. B. KIARA, LM Studio, Ollama)

➡️ Die Provider-Auswahl erfolgt **direkt im UI** von OpenCode Desktop.

---

## **2.1 Beispiel: Mistral AI (empfohlen)**

Für den Workshop empfehlen wir **Mistral – devstral-Modelle**.

### Voraussetzungen

API-Key lokal setzen (Beispiel macOS / Linux):

```bash
export MISTRAL_API_KEY="sk-..."
```

(Windows PowerShell entsprechend mit `setx` oder via *Systemumgebungs Variablen* über das *Start-Menü*)

### In OpenCode Desktop

1. OpenCode starten
2. Provider-Auswahl öffnen
3. **Mistral** auswählen
4. Als Modell wählen:

   ```
   Devstral 2
   ```

---

## **2.2 OpenAI / Anthropic (optional)**

Falls ihr OpenAI oder Anthropic nutzt:

* API-Keys müssen **vorab im System** gesetzt sein
* OpenCode erkennt diese automatisch
* Provider & Modell können anschließend im UI ausgewählt werden

---

# **3. Projekt öffnen**

1. In OpenCode Desktop:

   * *Open Project* wählen
   * Einen bestehenden Projektordner öffnen
     **oder**
   * Einen neuen, leeren Ordner anlegen

2. OpenCode analysiert automatisch:

   * Projektstruktur
   * Dateien
   * Kontext

---

# **4. Erste Tests**

## **Test 1: Chat / Agent aktiv**

Im Chat eingeben:

> „Analysiere dieses Repository und erkläre mir kurz, was es macht.“

Wenn eine sinnvolle Antwort kommt → LLM & Kontext funktionieren.

---

## **Test 2: Agentische Aufgabe**

> „Erstelle ein einfaches TicTacToe-Spiel in Python und erkläre mir die wichtigsten Teile.“

OpenCode sollte:

* einen Plan vorschlagen
* Dateien anlegen oder ändern
* die Schritte transparent anzeigen

---

# **5. Wichtige Hinweise**

* OpenCode ist **kein Editor für Inline-Edits**
* Es eignet sich besonders für:

  * größere Tasks
  * Feature-Implementierungen
  * Refactorings
  * Lernen durch gemeinsames Denken
* Für schnelles UI-Editing oder Autocomplete → **VOID nutzen**

---

# **6. Troubleshooting**

### **Kein Provider sichtbar**

→ API-Key nicht gesetzt
→ Terminal neu starten
→ OpenCode neu starten

### **Keine Antwort**

→ Falsches Modell ausgewählt
→ Rate-Limit erreicht
→ Netzwerk / Firewall prüfen

---

# **7. Weitere Infos**

* Website: [https://opencode.ai](https://opencode.ai)
* Docs: [https://opencode.ai/docs](https://opencode.ai/docs)

---
