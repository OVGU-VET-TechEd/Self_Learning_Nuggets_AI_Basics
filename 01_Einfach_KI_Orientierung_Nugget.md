<!--
author: UNESCO ASSET Team
email: asset-project@unesco.org
version: 1.0.0
language: de
narrator: German Female
comment: Self-Learning Nugget - Orientierung statt Overload: Einführung in KI
link: https://raw.githubusercontent.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/refs/heads/main/ASSET_basic.css
-->

# Einfach machen mit KI: Orientierung statt Überforderung

![KI Intro](media/intro.png)
@@ Bild einfügen @@
---

## Willkommen

Herzlich willkommen zu diesem Self-Learning Nugget **„Einfach machen mit KI: Orientierung statt Überforderung“**.  
Dieses Modul gibt Ihnen eine strukturierte Einführung in die Grundlagen von Künstlicher Intelligenz (KI) und zeigt, wie Sie den Überblick behalten, ohne in Informationsflut zu geraten.

> **Kursintention:** Orientierung schaffen, Kernbegriffe klären, Risiken verstehen und KI Beispiele kennenlernen.

**Dauer:** ca. 15 Minuten | **Format:** Selbstlernen mit Reflexion | **Level:** Einstieg

---

## Lernziele
@@ bitte alle Ziele untereinander auflisten @@
Am Ende dieses Nuggets können Sie:
1. Wichtige historische Meilensteine der KI benennen.
2. Zentrale Begriffe im Umgang mit KI erklären.
3. Chancen und Risiken aktueller KI-Anwendungen einschätzen.
4. Grundregeln für effektives Prompten anwenden.
@@ Punkt/Ziel Nr.4 sollte zu einem anderen Lernnugget @@
6. KI-Praxisbeispiele kritisch reflektieren.

---

## Modul 1: Geschichte der KI

### 1956 – Die Geburtsstunde der KI
- Dartmouth Summer School (USA)  
- Begriff „Artificial Intelligence“ entsteht  
- Vision: Maschinen simulieren menschliches Denken  

### Meilensteine
- **1966:** ELIZA – erstes Chatbot-Programm  
- **1997:** Deep Blue besiegt Schachweltmeister Garry Kasparov  
- **2012:** Deep Learning als Durchbruch  
- **2022:** ChatGPT wird veröffentlicht  
- **2024:** Reasoning & Multimodalität
@@ bitte in einem Zeitstrahl darstellen. Alles auf einer Slide @@
@@ ggf die Meilensteine verändern , damit es der Präsentation nicht zu ähnlich @@ 
![Meilensteine der KI](media/milestones.png)

---
## Modul 2: Definition: Was ist KI

@@ danach eine SLide dazu wie schnell die Entwicklung von KI im Vergelich zu anderen Technologien sicht verbreitet hat @@
## Modul 3: Zentrale Begriffe

KI klingt oft kompliziert – dabei steckt vieles schon in ein paar Schlüsselbegriffen. Schauen wir uns die wichtigsten gemeinsam an, um schnell einen klaren Überblick zu bekommen:

@keyConceptBox(Prompt = Eingabe, mit der man ein KI-Modell steuert. Beispiel: „Schreib mir eine Bewerbung“)

@keyConceptBox(Token = Sprachbausteine, meist Wortfragmente oder Wörter, in die ein Text zerlegt wird.)

@keyConceptBox(Bias (Verzerrung) = Vorurteile in der KI, verursacht durch einseitige Trainingsdaten.)

@keyConceptBox(Halluzination = Wenn KI plausible, aber falsche Informationen erzeugt.)

@keyConceptBox(LLM = Large Language Model – z. B. ChatGPT.)

@keyConceptBox(NLP = Natural Language Processing – Verarbeitung und Verstehen natürlicher Sprache.)

@keyConceptBox(Reasoning = Fähigkeit logische Schlüsse zu ziehen.)

@keyConceptBox(Neuronales Netz = Rechenmodell inspiriert vom menschlichen Gehirn.)

@@ den Begriff Deep Learning ergänzen und erklären @@
@@ am liebsten in einer Art Tabelle darstellen @@

---

## Modul 4: Chancen & Risiken von KI

### Modellübergreifende Hinweise
1. Ergebnisse immer kritisch prüfen.  
2. Prompts bewusst und klar formulieren.  
3. KI nicht ohne Kontrolle in sensiblen Bereichen einsetzen.

### Typische Fehlerquellen
- Keine echte „Intelligenz“, nur statistische Muster  
- Halluzinationen und falsche Fakten  
- Daten- und Datenschutzrisiken  
- Bias & ethische Risiken

@scenarioBox(Ein KI-Tool soll Schülerleistungen bewerten. Welche Risiken sehen Sie?)

---

@@@ Tabelle anlegen mit 4 Spalten: Tool, Stärken, Nachteile, Nutzung. Zeilen: ChatGPT (Open AI), Claude AI, Gemini (Google), Perplexity Al, Mistral, NotebookLM. siehe Folie 7 der Präsi @@@

### KI Tools
 
CHATGPT (OpenAl)
Sehr vielseitig (Text, Code. Bild - je nach Version), Gute Dialogfuhrung, Große
Community & Plug-ins
Teils veraltetes Wissen je nach Version), "Halluzinationen" möglich.
Keine echte Quellenprüfung
Schreiben, Brainstorming, Lernen, _Automatisieren, Codieren

Claude (Anthropic)
Extrem großer Kontext (100.000+ Token)
Fokus auf Sicherheit & „harmlosen Output"
Manchmal vorsichtiger als notig
(overcautious"
Keine echte Websuche
Dokumentenanalyse.
ethisch sensible Kontexte. Bildung

Gemini (Google)
Google-Integration (Docs, Suche etc.) Multimodal (Text, Bild, ggf. bald Video)
Starke Web-Recherche
Teils inkonsistent in Antworten Weniger transparent als OpenAl
Recherchen, Zusammenfassungen, Visualisierungen, Workspace-Tools

Perplexity Al
Sehr gute Recherche mit Quellenangabe
Fokus auf Aktualitat Schnell & prägnant
Kein Dialogverständnis wie bei ChatGPT
Quellen nicht immer tief geprüft
Datenschutz fragwürdig
Echtzeit-Recherche, Faktenchecks.
Zitierfähige Infos

Mistral
Open Source, performant & effizient Lokal einsetzbar (Datenschutz!)
Firmensitz in der EU
Erfordert technisches Know-how
Weniger Trainiert als ChatGPT oder andere große Modelle
Eigene Kl-Anwendungen, Forschung.
Unternehmenslösungen

NotebookLM
Nutzt nur eigene Dokumente
Quellenangaben
Einfach zu bedienen
Nur Englisch
Kein Internetzugriff
Begrenzte Verfügbarkeit
Dokumente analysieren
Fragen an eigene Inhalte stellen Unterricht & Recherche

## Modul 5: Richtig Prompten

„KI ist wie ein wissbegieriges Kind: Sie kennt unglaublich viel, versteht aber nicht automatisch alles und braucht klare, genaue Anweisungen.“

### Tipps vor dem Prompten
- Chat-Training ausschalten, wenn sensible Daten verwendet werden.  
- Immer Quellen prüfen.  
- Bias bewusstmachen.  
- Datenschutz sicherstellen.

### Übung: Prompt-Variationen
Formulieren Sie einen Prompt für eine Präsentation über **„Chancen und Risiken von KI in der Medizin“**.  
- Version A: „Schreib mir etwas über KI in der Medizin.“  
- Version B: „Schreibe einen strukturierten Artikel (ca. 500 Wörter) zum Thema ‚Chancen und Risiken von KI in der Medizin‘. Nutze sachliche Sprache, gliedere ihn in Einleitung, Hauptteil, Fazit.“  

> [[___]] Welche Unterschiede erwarten Sie bei den Ergebnissen?

---

## Modul 6: Praxisbeispiele

### Recherche
„Ich muss einen Überblicksbericht zu Start-ups in Baden-Württemberg verfassen. Welche Programme gibt es vom Land?“

### Zusammenfassung
„Fasse den folgenden wissenschaftlichen Artikel in maximal 5 Sätzen so zusammen, dass ihn Schüler*innen der 10. Klasse verstehen können.“

### Strukturierte Texte
„Schreibe einen Blogartikel zum Thema ‚Chancen und Risiken von KI in der Medizin‘.“

### Anonymisierung von Interviews (Forschung)
- Namen der Interviewer:innen → I1, I2 …  
- Namen der Befragten → T1, T2 …  
- Alle anderen Eigennamen anonymisieren (z. B. Heinz Müller → H. M.)

@scenarioBox(Überlegen Sie: Welche Vorteile hat automatisierte Anonymisierung für die Forschung? Welche Risiken?)  

---

## Reflexion

<div class="reflection-section">

**Fragen zur Selbstreflexion**

1. Welche 3 Begriffe aus dem Nugget waren für Sie neu?  
   [[___]]  

2. Wo sehen Sie aktuell die größten Chancen von KI in Ihrem Berufsfeld?  
   [[___]]  

3. Welche Risiken erscheinen Ihnen am wichtigsten, kritisch zu hinterfragen?  
   [[___]]  

</div>

---

## Weiterführende Ressourcen

- [UNESCO AI Competency Framework](https://unesdoc.unesco.org/ark:/48223/pf0000391104)  
- [Stanford HAI Principles](https://hai.stanford.edu/about)  
- [Partnership on AI – Education](https://partnershiponai.org/program/education/)  

---

## Abschluss

🎉 Herzlichen Glückwunsch! Sie haben das Self-Learning Nugget **„Einfach KI – Orientierung statt Overload“** abgeschlossen.  

<div class="contact-info">
Kontakt: Maike Haag – [LinkedIn](https://www.linkedin.com/in/maike-haag-3964b2198) | maikehaag@web.de
</div>

