---
title: Hyperlinks
pre: "<b>4. </b>"
weight: 4
---

## Arbeitsauftrag

Erstelle in deinem Dokument einen Hyperlink zu ...
  
  * Einer fremden Webseite
  * Einer anderen HTML-Datei im selben Ordner, die du selbst angelegt hast.
  * Einer Datei in einem Unterordner deiner HTML-Datei

## Syntax

Ein **Hyperlink** wird folgender Syntax erstellt:

```html 
<a href=“[Url]“>Name des Links</a>
```

Die [URL] kann dabei sowohl auf eine **andere Webseite** verweisen als auch auf eine Datei **relativ** zum eigenen Pfad. 

**Beispiele:**

```html
<a href=“http://www.cws-usingen.de“>CWS Usingen</a>
<a href=“impressum.html“>Impressum</a>
<a href=“unterordner/impressum.html“>Impressum</a>
```

## Theorie Hyperlinks

Angenommen du hast eine Datei c:\mein-ordner\index.html. Du kannst die html-Datei bearbeiten, indem du einen Link erstellst in der Form: 

```html
<a href=“c:\mein-ordner\index.html“>Mein Link</a> 
```

Das Problem dabei ist folgendes: Wenn du die Datei auf den Server kopierst, liegt sie dort in einem anderen Pfad und der Link funktioniert dort nicht mehr. 

Daher verwendet man bei der HTML-Programmierung fast immer Pfade, die **relativ zur aktuellen Position** liegen.

![orderstruktur](/html/ordnerstruktur.png)

•Mit **unterordner**/datei.html kannst du auf Dateien in Unterordnern zugreifen.

•Mit **../**datei.html kannst du auf Dateien in übergeordneten Ordnern zugreifen

•Mit **../nachbar/datei.html** kannst du auf Dateien zugreifen, die auf einem Ordner auf gleicher Ebene liegen.


### Interne Links in repl.it

In repl.it kannst du Dateien mit **Drag & Drop** hinzufügen. Ziehe dazu eine Datei von deinem Desktop in den linken Bereich deines repls, bis sich der Mauszeiger verändert.

Anschließend kannst du auf die Datei verlinken.