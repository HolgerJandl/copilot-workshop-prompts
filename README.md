# Copilot Workshop: Prompts zum Mitmachen

Alle Prompts aus der Live-Demo zum Kopieren. Rechts oben in jedem grauen Kasten auf das Kopier-Symbol klicken und in Copilot einfügen. Die Beispiele spielen im fiktiven Unternehmen Contoso; passen Sie Namen, Zeiträume und Dateien an Ihre eigene Aufgabe an.

## Use Case 1: Vertretung übernehmen mit persönlichem Copilot

### Schritt 1: Copilot meinen Schreibstil beibringen

Wo: Copilot Chat (https://copilot.cloud.microsoft/), oben "Arbeit"

```text
Analysiere die E-Mails, die ich in den letzten drei Monaten gesendet habe. Beschreibe meinen Schreibstil: Anrede, Grußformel, Länge, Aufbau, Tonalität, typische Formulierungen und wann ich Deutsch oder Englisch schreibe. Formuliere daraus eine Anweisung an Copilot für das Verfassen meiner E-Mails, in der Du-Form, höchstens 1.000 Zeichen, die ich direkt in Outlook einfügen kann. Übernimm keine Namen, Zahlen oder Inhalte aus den E-Mails.
```

Danach: Outlook, Pfeil neben dem Copilot-Symbol, Einstellungen, Entwurfsanweisungen. Schalter aktivieren, Text einfügen, speichern.

### Schritt 2: Meeting nachholen

Wo: Teams, Meeting im Chat öffnen, Registerkarte "Zusammenfassung", Copilot

```text
Ich übernehme diese Vertragsverlängerung als Vertretung. Was wurde in dieser Besprechung entschieden, was ist noch offen, und wer hat welche Aufgabe bis wann? Stelle die Aufgaben als Tabelle mit verantwortlicher Person und Termin dar. Wenn kein Termin genannt wurde, schreibe „kein Termin genannt“.
```

```text
Was spricht laut dieser Besprechung für und gegen einen Wechsel zu Summit Metrology? Nenne jeweils, wer es gesagt hat, mit Zeitpunkt im Meeting.
```

### Schritt 3: Mail beantworten

Wo: Outlook, Mail öffnen, "Antworten", "Mit Copilot entwerfen"

```text
Antworte auf Englisch, weil Brightline auf Englisch schreibt. Ich vertrete Corey Gray. Bedanke dich für das überarbeitete Angebot und bitte um Klärung bis 27. November: 1) Bearbeitungszeit von fünf Arbeitstagen ohne Aufpreis, wie in der E-Mail genannt, 2) Haftungsgrenze von 1 Mio. Euro wie im aktuellen Vertrag, 3) Nachweis der verlängerten Akkreditierung vor Vertragsabschluss. Freundlich, aber bestimmt.
```

## Use Case 2: Leasing-Angebote in Excel auswerten und ergänzen

### Schritt 1: Daten analysieren

Wo: Excel, Datei öffnen, "Start", "Copilot", Modus "Chat"

```text
Ich muss bis Freitag eine Empfehlung für die neue Dienstwagenflotte abgeben. Analysiere die drei Leasing-Angebote in dieser Tabelle: Welches Angebot ist bei den Gesamtkosten pro Fahrzeug über 36 Monate inklusive Monatsrate, Energie und Wartung am günstigsten, wie unterscheiden sich CO2 und Lieferzeit, und welche Auffälligkeiten oder fehlenden Angaben siehst du? Antworte in Stichpunkten und nenne die Zahlen.
```

### Schritt 2: Inhalt einfügen mit "Mit Copilot bearbeiten"

Wo: Excel, Copilot, Modus "Bearbeiten"

```text
Füge ein neues Blatt „Vergleich“ hinzu. Berechne dort für jedes Angebot und Modell die Gesamtkosten pro Fahrzeug über 36 Monate aus Monatsrate, Energie und Wartung als Formeln, stelle CO2 pro Fahrzeug und Lieferzeit daneben und vergib eine Bewertung mit der Gewichtung Kosten 50 %, CO2 30 %, Lieferzeit 20 %. Sortiere nach der Bewertung, hebe das beste Angebot farbig hervor und füge ein Balkendiagramm der Gesamtkosten hinzu.
```

### Schritt 3 (optional): Präsentation erstellen

Wo: PowerPoint, neue Präsentation, Copilot, Datei mit / auswählen

```text
Erstelle aus /FLT-2026-031_Lease_Offers.xlsx eine Präsentation mit vier Folien für die Geschäftsleitung: 1) Ausgangslage, 2) Vergleich der drei Angebote nach Gesamtkosten, CO2 und Lieferzeit, 3) Empfehlung, 4) nächste Schritte. Kurze Stichpunkte, höchstens fünf pro Folie.
```

## Nachmittag: Copilot-Werkstatt mit dem Reise-Assistenten

In der Vorführung bauen wir einen eigenen Assistenten, der Fragen zu Dienstreisen ausschließlich auf Basis der (fiktiven) Contoso Reiserichtlinie 2026 beantwortet. Danach bauen Sie nach demselben Muster Ihren eigenen Assistenten.

### Schritt 1: Assistenten beschreiben

Wo: Copilot Chat, links "Agents", dann "Agent erstellen"

```text
Erstelle einen Assistenten namens Reise-Assistent, der Fragen von Mitarbeitenden zu Dienstreisen, Dienstwagen und Reisekosten ausschließlich auf Basis der Contoso Reiserichtlinie 2026 beantwortet. Antworte in der Sprache der Frage, halte die Antworten kurz, nenne immer den Abschnitt der Richtlinie, und wenn die Richtlinie eine Frage nicht abdeckt, sage das und verweise an die Reisestelle.
```

### Schritt 2: Wissen hinzufügen

Wo: im Agent Builder unter "Wissen" die SharePoint-Seite oder die Datei Contoso_Reiserichtlinie_2026.docx auswählen. Optional die Websuche deaktivieren, damit der Assistent nur aus der Richtlinie antwortet.

### Schritt 3: Startprompts ergänzen und testen

Diese Fragen als Startprompts eintragen und im Testbereich rechts ausprobieren:

```text
Darf ich für eine zweitägige Reise nach München einen Mietwagen statt eines E-Fahrzeugs aus dem Pool buchen?
```

```text
Ich musste mit dem Poolfahrzeug unterwegs privat laden. Was bekomme ich erstattet?
```

```text
Welche Hotelobergrenze gilt in München?
```

Und einmal eine Frage, die die Richtlinie nicht regelt. Der Assistent sollte das sagen und an die Reisestelle verweisen:

```text
Darf ich nach der Dienstreise noch zwei Urlaubstage am Zielort anhängen?
```

### Ihr eigener Assistent: Vorlage zum Anpassen

Ersetzen Sie die Angaben in eckigen Klammern:

```text
Erstelle einen Assistenten namens [Name], der [Zielgruppe] bei [Aufgabe] unterstützt. Nutze ausschließlich [Wissensquelle, z. B. Richtlinie, Handbuch, Vorlage]. Antworte [Sprache, Länge, Ton], nenne immer die Quelle, und wenn du etwas nicht weißt, sage das und verweise an [Ansprechpartner].
```

Tipps: Nur freigegebene, unkritische Dokumente als Wissen verwenden. Den Assistenten nur mit Personen teilen, die auch Zugriff auf die Wissensquelle haben.

## Gute Prompts in vier Teilen

Ziel (was soll entstehen), Kontext (wer bin ich, worum geht es), Quelle (welche Datei, Mail, welches Meeting) und Erwartung (Format, Länge, Ton). Danach mit kurzen Folgeprompts nachschärfen: "kürzer", "als Tabelle", "für die Geschäftsleitung".
