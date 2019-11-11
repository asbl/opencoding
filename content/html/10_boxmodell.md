---
title: Das Box-Modell
pre: "<b>10. </b>"
weight: 10
---

## Arbeitsauftrag

Erstelle mit dem Tag **\<div\>** einen Bereich mit Text, färbe den Hintergrund und lege Innen-und Außenabstände dieses Bereichs fest.

## Theorie: Das Boxmodell

Wenn die Hintergrundfarben, Rahmen und Abstände zeichnen willst, ist es wichtig das Box-Modell von HTML / CSS zu verstehen:

Jedes Tag wird entweder **inline** dargestellt oder als **Block**. 

![1573464658625](/html/inlineblock.png)

Du kannst die Eigenschaft umstellen mit dem Attribut **display** .

### Beispiel: 

Ein link wird normalerweise inline im Text dargestellt. Wenn dieser als Block modelliert werden soll (z.B. weil er wie ein Button aussehen soll, dann musst du folgendes schreiben:

```css
a {
    display: block;
}
```

Besser siehst du dies, wenn du dem Link einen Rahmen gibst:

```css
a {
    display: block;
    border: 1px solid black
}
```

Dies sieht so aus:

<a href="/" style="display: block; border: 2px solid black;">Ein Link</a>

Als Block nimmt 

### Blöcke und Abstände

Ein Block kann über Inhalt, Rahmen und Abstände definiert werden:![1573465342433](/html/boxmodell.png)

#### Margin

Legst die außenabstände fest. 

Beispiele:

  ```css
margin: 10 px;
margin-left: 5px;
  ```

#### Border

Legt den den Rahmen fest, z.B. für einen Rahmen der Dicke 1 px in schwarz:

```css
border: 1px solid black;
```

Es gibt ziemlich viele zusätzliche Attribute zum Gestalten von Rahmen: https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/%C3%A4u%C3%9Fere_Gestaltung/Rahmen

#### Padding

Legt die Innenabstände fest.

Beispiele:

  ```css
padding: 10 %;
padding-right: 5px;
  ```

Diese Eigenschaften funktionieren nur bei Elementen mit der Eigenschaft **display : block!**