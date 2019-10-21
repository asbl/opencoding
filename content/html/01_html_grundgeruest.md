---
title: HTML Grundgerüst
pre: "<b>1. </b>"
weight: 1
---

## Arbeitsauftrag

Lege eine Datei index.html mit folgendem Inhalt an:

```html
<!DOCTYPE html>
<html lang="de">

  <head>
      <title>Titel der Einzelseite</title>
      <link href="style.css" type="text/css" rel="stylesheet">
      <meta charset="UTF-8">
  </head>

  <body>
 
  </body>
</html>
```

### Hinweis für Windows-Benutzer

Wenn du die **Endung** .html der Datei nicht ändern kannst, musst du die Windows-Option „Bekannte Dateiendungen ausblenden“ deaktivieren.

![Dateiendungen](/html/dateiendungen.png)

## Mehr Infos über HTML

Ein HTML-Dokument ist folgendermaßen aufgebaut:

* **Tags**, enthalten Inhalte oder andere Tags. 
* Ein Tag wird mit spitzen Klammern beschrieben, z.B. `<head>, <html>, <body>`. Auf diese Weise beschreiben Tags die **Elemente** des HTML-Dokuments. 

Elemente werden üblicherweise geöffnet mit `<tagname>` und mit `</tagname>` geschlossen. Alles was dazwischen steht, befindet sich *innerhalb* des Elements. 

Von dieser Regel gibt es einige Ausnahmen. Wenn ein Tag keinen Inhalt hat, dann muss dies auch nicht geschlossen werden. Man kann dies trotzdem durch ein / am Ende des Tags kennzeichnen, z.B. in dem man schreibt: `<meta charset="UTF-8"/>`.  

Auf diese Weise ergibt sich die Struktur des Dokuments:

![1571578761505](/html/htmlstruktur.png)