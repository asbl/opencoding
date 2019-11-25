---
title: Flexbox
pre: "<b>13. </b>"
weight: 13
---

## Arbeitsauftrag:

Erstelle eine Webseite, bei der Elemente mit dem flexbox-Layout angeordnet werden.

## Theorie: Das Flex-Box-Modell

Das Flexbox-Modell ist eine Möglichkeit, wie du Inhalte anordnen kannst, z.B. in Spalten.

Flexbox kennt prinzipiell mit der display-Eigenschaft verwenden:

```css
.container {
  display: flex
}
```


![Inline und Block-Elemente](/html/flexbox.jpg)


So kannst du die Kindelemente in dem Container platzieren:

```css
.container {
  display: flex
}
```

```html
<div class="container">
<div class="child">Item 1</div>
<div class="child">Item 2</div>
<div class="child">Item 3</div>
</div>
```

Dies sieht (wenn du den Child-Elementen noch etwas Rahmen und Abstand gibst) folgendermaßen aus:


![Inline und Block-Elemente](/html/flexbox2.jpg)


Dies sind bereits die Grundlagen von Flexbox. In Kombination mit margin, padding und border kannst du jetzt vielfältige Layouts erstellen, die auch auf unterschiedlichen Endgeräten gut aussehen. 

Mit weiteren Attributen kannst du die Darstellung verfeinern.

###### Richtung:

```css
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

Dies gibt die Richtung an, in der die Spalten angeordnet werden.

```css
.child {
  order: <integer>; /* default is 0 */
}
```

Dies legt die Reihenfolge der Elemente fest. Je kleiner der Wert umso weiter vorne wird das Element angezeigt.

```css
.container{
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

Gibt an, ob Elemente in die nächste Zeile verschoben werden dürfen.

###### Inhalt anordnen
```css
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right 
}
```

Ordnet die Elemente horizontal an.

###### Inhalt vertikal anordnen

```css
.container {
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end 
}
```

Gibt die Vertikale Anordnung der Elemente an.

## Mehr Informationen:

Hier findest du alle Eigenschaften von Flexbox anschaulich dargestellt: 
https://css-tricks.com/snippets/css/a-guide-to-flexbox/