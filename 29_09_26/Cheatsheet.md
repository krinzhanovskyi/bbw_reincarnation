# Cheatsheet Webauftritt

Autor: Oleksandr Krizhanovskyi<br/>
Version: 29.09.2026

## Begriffe zum Webauftritt

- **Webauftritt**:<br/> Ein Webauftritt ist die Gesamtheit aller digitalen Inhalte und Funktionen, die eine Person oder Organisation im Internet präsentiert, z. B. eine Website mit mehreren Seiten, Informationen und Angeboten.
- **Webseite**:<br/> Eine Webseite ist eine HTML-Seite, die im Browser angezeigt wird und bestimmte Inhalte oder Funktionen enthält.
- **Webpage**:<br/> Ein Webpage ist ein weiterer Begriff für eine Webseite; meist wird der Begriff in der englischen Fachsprache verwendet.
- **HTML**:<br/> HTML bedeutet HyperText Markup Language. HTML ist die Grundsprache zur Strukturierung von Inhalten im Web. Damit werden Texte, Überschriften, Bilder, Listen und Verknüpfungen definiert.
- **CSS**:<br/> CSS bedeutet Cascading Style Sheets. CSS beschreibt das Aussehen und das Layout.

## Request / Response & Netzwerk

- **IP-Adresse**:<br/> Eine IP-Adresse ist die eindeutige Nummer, mit der Geräte im Netzwerk (zBsp. im Internet) identifiziert werden. Sie funktioniert wie eine Telefonnummer: jeder Rechner braucht sie, um erreichbar zu sein.
  - **IPv4**: vier Zahlenblöcke (0–255), zBsp `192.168.0.1`
  - **IPv6**: längere, hexadezimale Schreibweise, weil es viel mehr Adressen gibt, zBsp `2001:0db8:85a3:0000:0000:8a2e:0370:7334`

- **Request**:<br/> Anfragen von Clients (zBsp Browsern) an den Server.
- **Response**:<br/> Antwort des Servers. Der Server schickt die passende Antwort zurück. Diese enthält den Status (zBsp Erfolg oder Fehler) und die Daten (zBsp HTML-Seite, JSON, Bilddatei).

- **URL (Uniform Resource Locator)**:<br/> Ist die Adresse einer Ressource im Internet. Sie zeigt dem Browser, wo etwas liegt und wie es abgerufen wird.
  - _Beispiel_: `https://www.beispiel.ch:443/pfad/datei.html?suche=test#anker`
  - `https` → Protokoll
  - `www.beispiel.ch` → Domain/Server
  - `:443` → Port (optional)
  - `/pfad/datei.html` → Dateipfad
  - `?suche=test` → Parameter
  - `#anker` → Sprungmarke auf der Seite

## HTML, Tags

### Heading/Überschrift:

- h1 ... h6

### Grundgerüst

- `<!DOCTYPE html>`: Definiert das Dokument als HTML5.
- `<html>`: Das Wurzelelement (Root) der Webseite.
- `<head>`: Enthält Metadaten, den Titel und Links zu CSS-Dateien (für den Benutzer nicht sichtbar).
- `<body>`: Enthält den sichtbaren Inhalt der Webseite.

### Text & Überschriften

- `<h1>` bis `<h6>`: Überschriften (Headings). `<h1>` ist die wichtigste (meist nur einmal pro Seite), `<h6>` die kleinste.
- `<p>`: Ein Textabsatz (Paragraph).
- `<br>`: Ein Zeilenumbruch (Line break). Ein "leerer" Tag ohne schliessenden Tag.
- `<strong>`: Wichtiger Text, wird meist fett gedruckt.
- `<em>`: Betonter Text (emphasized), wird meist kursiv gedruckt.

### Links & Bilder

- `<a>`: Ein Hyperlink (Anchor). Das Attribut `href` definiert das Ziel.
- `<img>`: Ein Bild. Benötigt die Attribute `src` (Bildquelle/Pfad) und `alt` (Alternativtext für Screenreader oder falls das Bild nicht lädt).

```html
<a href="[https://ethz.ch](https://ethz.ch)">Zur ETH Zürich</a>
<img src="logo.png" alt="Firmenlogo" />
```
