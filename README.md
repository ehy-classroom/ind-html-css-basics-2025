# HTML/CSS Basics 2025
Für Kurse bei indisoft


Version: 1.0.0

Autor: Enno Hyttrek, ehy.training@gmail.com


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

## Beschreibung der Übungsdatei index.html (Version 1.0.0)

In der Übungsdatei `index.html` wurde eine minimale HTML-Struktur erstellt:

- Die Datei beginnt mit der Deklaration `<!DOCTYPE html>` für HTML5.
- Das `<html>`-Element legt die Sprache auf Deutsch fest (`lang="de"`).
- Im `<head>`-Bereich steht der Titel der Seite.
- Im `<body>`-Bereich wird eine Überschrift angezeigt.

**Schritte dorthin:**
1. Neue Datei `index.html` anlegen
2. Grundstruktur mit `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>` schreiben
3. Titel und Überschrift ergänzen
4. Datei speichern und im Browser testen

**Version 1.0.0** steht für die erste, einfache Version der Datei.

## Kommentar zur kommentierten Version

Es gibt zusätzlich eine Datei `index-commented.html`, in der alle Elemente ausführlich kommentiert sind. Sie dient ausschließlich zur Erklärung des Codes und ist eine ganz normale HTML-Datei – sie kann nicht mehr als Startseite (index.html) funktionieren, weil es im Webverzeichnis immer nur eine Datei mit dem Namen `index.html` geben kann. Nur diese wird beim Aufruf des Verzeichnisses automatisch angezeigt. Varianten wie `index2.html` oder `index3.html`, die man manchmal sieht, sind grundsätzlich sinnlos, da sie keine besondere Bedeutung für den Webserver haben und nicht automatisch geladen werden.