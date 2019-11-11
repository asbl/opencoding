---
title: CSS
pre: "<b>8. </b>"
weight: 8
---

## Arbeitsauftrag

HTML-Code kann mit Hilfe von CSS (Cascading Style Sheets) gestaltet werden. 

## Eine CSS Datei erstellen

Erstelle eine neue Datei im gleichen Ordner wie deine HTML-Datei mit den Namen **style.css**.

Schreibe in die Datei folgenden Text:

```css
b {
  color: red;
}
```
Der Code gibt allen <b> Tags eine rote Farbe. Bevor du die Änderung sehen kannst, musst du die Datei in HTML einbinden.

## CSS-Datei im HTML-Code einbinden

Dafür muss innerhalb des **head**-Tags folgender Code eingefügt werden.

```html
<link rel="stylesheet" type="text/css" href="style.css"/>
```
 **style.css** ist der Dateiname deiner Datei. Wenn du diese anders nennst oder in einem anderen Ordner speicherst, musst du diese Stelle entsprechend abändern.

## Eigenschaften zuweisen.

Jetzt kannst du einige deiner HTML-Tags gestalten, indem du dem HTML-Tag Eigenschaften zuweist.

 ```css
a { 
    color: white;
    background-color: black;
}
b {
    color: red;
}
 ```

Interessante css-Eigenschaften sind z.B. **color**, **background-color**, **height**, **width**, **max-width**, **align**, …


## Aufbau einer CSS-Datei

![1571659829122](./aufbaucss.png)

## Referenz

Eine Liste von Eigenscharten und möglichen Werten findest du hier: http://www.html-seminar.de/css-definitionen-uebersicht.htm 

## Typische Fehlerquellen

* Verwende kein **=** bei Wertzuweisungen (color **:** red, **nicht** color = red)
* Setze immer ein Semikolon ; am Ende einer Zeile, ansonsten werden deine nächsten Definitionen in der Regel nicht angewendet.

## Mehr Infos über CSS

* Mehr Infos zur Syntax: https://wiki.selfhtml.org/wiki/CSS/Tutorials/Einstieg/Syntax 