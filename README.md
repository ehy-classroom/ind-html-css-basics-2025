# HTML/CSS Grundlagen 2025
Für Kurse in der Weiterbildung und Umschulung  
<a href="https://ehy-classroom.github.io/ind-html-css-basics-2025/" target="_blank">https://ehy-classroom.github.io/ind-html-css-basics-2025/</a>



Version: 1.0.6

Autor: Enno Hyttrek, <a href="mailto:ehy.training@gmail.com" target="_blank">ehy.training@gmail.com</a>


## Was bedeutet HTML? 

HTML steht für "HyperText Markup Language". Es ist die Standardsprache, um Inhalte und Struktur von Webseiten zu beschreiben. Mit HTML werden Texte, Bilder, Links und viele weitere Elemente auf einer Webseite angeordnet.

## Warum ist HTML keine Programmiersprache?

HTML ist eine Auszeichnungssprache (Markup Language), keine Programmiersprache. Das bedeutet: Mit HTML kann man keine Befehle, Schleifen oder Bedingungen formulieren, sondern nur die Struktur und Bedeutung von Inhalten festlegen. Es gibt keine "Logik" oder "Berechnungen" in HTML.

## Syntax von HTML (Tags, Attribute, etc.)

HTML besteht aus sogenannten "Tags" (Elementen), die in spitzen Klammern stehen. Die meisten Tags haben ein öffnendes und ein schließendes Tag:

```html
<p>Dies ist ein Absatz.</p>
```

Tags können auch "Attribute" enthalten, die zusätzliche Informationen liefern:

```html
<a href="https://www.example.com">Ein Link</a>
```

Im Beispiel ist `href` ein Attribut, das das Ziel des Links angibt.

## Bedeutung der Datei index.html

Die Datei `index.html` ist die Startseite einer Webseite. Wenn man einen Ordner im Browser aufruft, wird automatisch die `index.html` angezeigt. Sie ist der Einstiegspunkt für Besucher.

## Beschreibung der Übungsdatei index.html (Version 1.0.6)

In der Übungsdatei `index.html` wurde eine HTML-Struktur mit semantischen Elementen und erweiterten CSS-Styling erstellt:

### Grundstruktur (seit Version 1.0.1)
- Die Datei beginnt mit der Deklaration `<!DOCTYPE html>` für HTML5
- Das `<html>`-Element legt die Sprache auf Deutsch fest (`lang="de"`)
- Meta-Tags für Zeichencodierung (`charset="UTF-8"`) und mobile Darstellung (`viewport`)
- Titel der Seite im `<head>`-Bereich

### Semantische HTML5-Elemente (seit Version 1.0.2)
HTML5 bietet semantische Elemente, die die Bedeutung und Struktur einer Webseite besser beschreiben:

- **`<header>`** - Kopfbereich der Seite (statt eines einfachen `<div>`)
- **`<main>`** - Der Hauptinhalt der Seite (sollte nur einmal pro Seite verwendet werden)
- **`<section>`** - Thematisch zusammengehörige Inhaltsabschnitte
- **`<aside>`** - Seiteninhalt oder zusätzliche Informationen
- **`<footer>`** - Fußbereich der Seite

### Bilder und Medien (seit Version 1.0.3)
```html
<figure>
    <img src="pfad/zum/bild.jpg" alt="Beschreibung des Bildes">
    <figcaption>Bildunterschrift</figcaption>
</figure>
```

### Links mit neuen Tab (seit Version 1.0.3)
```html
<a href="https://example.com" target="_blank">Link öffnet in neuem Tab</a>
```

### Strukturierte Navigation und Listen (seit Version 1.0.4)
```html
<nav class="main-nav">
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#section-01">Abschnitt 1</a></li>
        <li><a href="#section-02">Abschnitt 2</a></li>
        <li><a href="#main-footer">Footer</a></li>
    </ul>
</nav>
```
- Navigation mit ungeordneter Liste (`<ul>`) für gleichwertige Menüpunkte
- Zusätzlich geordnete Liste (`<ol>`) im `<aside>`-Bereich für nummerierte Aufzählungen

### CSS-Styling (seit Version 1.0.5)
```css
body {
    background: hsl(200, 10%, 20%);
    color: hsl(200, 10%, 100%);
}
```
- Externes CSS-Stylesheet (`style.css`) für das Styling hinzugefügt
- Dunkles Theme mit HSL-Farbwerten implementiert

### Erweiterte CSS-Architektur (seit Version 1.0.6)
```css
/*---------------------
RESET
---------------------*/
*::before, *::after, * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/*---------------------
LAYOUT
---------------------*/
.container {
    padding: 1rem 20px;
    max-width: 75rem;
    margin: 0 auto;
}
```
- **CSS Reset**: Normalisiert Browser-Unterschiede mit Universal-Selektor
- **Container-System**: Zentrierte, begrenzte Inhaltsbreite für bessere Lesbarkeit
- **Strukturierte CSS-Organisation**: Logische Gruppierung (Reset, Layout, Colors, etc.)
- **Flexbox-Navigation**: `display: flex` für horizontale Menüanordnung
- **HSL-Farbschema**: Konsistente Farbpalette mit verschiedenen Helligkeitsstufen
- **Responsive Design Vorbereitung**: Viewport-relative Einheiten (vh, vw)
- **Box-Model Optimierung**: `box-sizing: border-box` für einfachere Berechnungen

**Schritte zur Erstellung:**
1. Neue Datei `index.html` anlegen
2. Grundstruktur mit `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>` schreiben
3. Meta-Tags für Zeichencodierung und mobile Darstellung hinzufügen
4. Semantische Elemente statt einfacher `<div>`-Container verwenden
5. Bilder mit `<figure>` und `<figcaption>` strukturieren
6. Links mit passenden Attributen versehen
7. Datei speichern und im Browser testen
8. CSS-Stylesheet hinzufügen für Styling
9. CSS-Architektur mit Reset, Layout-System und strukturierter Organisation erweitern

**Version 1.0.6** steht für die aktuelle Version mit semantischen HTML5-Elementen, Bildern, strukturierter Navigation, professioneller CSS-Architektur mit Reset, Container-System, Flexbox-Layout und strukturierter Code-Organisation.

## CSS-Integration und die Cascade

### Die drei Arten, CSS einzubinden

CSS kann auf drei verschiedene Arten in HTML-Dokumente eingebunden werden. Dabei gilt eine klare Prioritätsreihenfolge (CSS-Cascade):

#### 1. Externes Stylesheet (niedrigste Priorität)
```html
<link rel="stylesheet" href="path/to/style.css">
```
- CSS-Regeln werden in einer separaten `.css`-Datei definiert
- Wird über das `<link>`-Element im `<head>` eingebunden
- Beste Praxis für größere Projekte und Wartbarkeit
- **In diesem Projekt:** `style.css`

#### 2. Internes Stylesheet (mittlere Priorität)
```html
<style>
    /* CSS-Regeln hier */
</style>
```
- CSS-Regeln werden direkt im `<head>` der HTML-Datei definiert
- Überschreibt Regeln aus externen Stylesheets
- **In diesem Projekt:** Leerer `<style>`-Container vorhanden, aber nicht verwendet

#### 3. Inline-Styles (höchste Priorität)
```html
<div style="color: red;">Roter Text</div>
```
- CSS-Regeln werden direkt am HTML-Element definiert
- Überschreibt alle anderen CSS-Regeln
- **In diesem Projekt:** Bewusst NICHT verwendet (schlechte Praxis)

### Warum die Cascade wichtig ist

Die CSS-Cascade bestimmt, welche Regel angewendet wird, wenn mehrere Regeln auf dasselbe Element wirken. Die Reihenfolge ist:
1. Inline-Styles (höchste Priorität)
2. Interne Stylesheets (`<style>`)
3. Externe Stylesheets (`<link>`)
4. Browser-Standard-Styles (niedrigste Priorität)

Zusätzlich spielen **Spezifität** und **Reihenfolge** eine Rolle bei der Regel-Auswahl.

## Kommentar zu den kommentierten Dateien

Es gibt zusätzlich kommentierte Versionen der Dateien zur Erklärung:

### `index-commented.html`
Diese Datei enthält alle HTML-Elemente mit ausführlichen Kommentaren. Sie dient ausschließlich zur Erklärung des Codes und ist eine ganz normale HTML-Datei – sie kann nicht mehr als Startseite (index.html) funktionieren, weil es im Webverzeichnis immer nur eine Datei mit dem Namen `index.html` geben kann. Nur diese wird beim Aufruf des Verzeichnisses automatisch angezeigt. Varianten wie `index2.html` oder `index3.html`, die man manchmal sieht, sind grundsätzlich sinnlos, da sie keine besondere Bedeutung für den Webserver haben und nicht automatisch geladen werden.

### `style-commented.css`
Diese CSS-Datei enthält dieselben Styling-Regeln wie `style.css`, aber mit ausführlichen Kommentaren zu jedem CSS-Konzept. Sie dient nur zur Veranschaulichung und wird nicht in der HTML-Datei eingebunden. Für das tatsächliche Styling der Website wird ausschließlich `style.css` verwendet.

---

**Anmerkung:** Diese README-Datei sowie Teile des Codes der Beispieldateien wurden mit KI-Unterstützung erstellt (GitHub Copilot, Modell Claude Sonnet 4).