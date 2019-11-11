---
title: Klassen
pre: "<b>11. </b>"
weight: 11
---

## Arbeitsauftrag

Erstelle mehrere Tags gleicher Art. Gestalte mit Hilfe von Klassen nur einzelne Objekte dieses Tags.

Du kannst z.B. mehrere Links erstellen und einige Links als button gestalten.

## Theorie: Klassen

Klassen sind im Baupläne oder Schablonen. Die Idee ist es, CSS Code wiederzuverwenden, denn mit Hilfe von Klassen must du nicht jeden einzelnen Link einzeln formatieren.

### Beispiel: Buttons

Sollen bestimmte Links als Buttons gezeigt werden, so weist man all diesen Links die Klasse **button** zu. Sollen die selben Links in **rot** formatiert werden, so weist man ihnen zusätzlich die Klasse **red** zu.

In deinem HTML-Code können Klassen mit Hilfe des Attributes **class** zugewiesen werden:

```html
<a href="impressum.html" class="button red">Impressum</a> 
```

Dies weist dem Link die Klassen button und red zu. 

In der CSS-Datei können diese Klassen nun folgendermaßen formattiert werden:

```css
button {
  border: 1px solid black;
  padding: 5px;
}

.red {
  background-color: red;
}
```

Im CSS Code wird vor die Klasse ein **Punkt** geschrieben, um sie von Tags zu unterscheiden.

