---
title: Tabellen
pre: "<b>6. </b>"
weight: 6
---

## Arbeitsauftrag

Füge eine Tabelle in deinem Dokument hinzu.

## Syntax

Tabellen können in html mit folgender Syntax erstellt werden:

```html
<table>
    <tr>
        <td>Zeile 1 – Spalte 1 </td>
        <td>Zeile 1 – Spalte 2</td>        
        <td>Zeile 1 – Spalte 3</td>    
    </tr>    
    <tr>
        <td>Zeile 2– Spalte 1</td>
        <td>Zeile 2 – Spalte 2</td>
        <td>Zeile 2 – Spalte 3</td>
    </tr>
</table>
```

Der Code erzeugt folgende Tabelle:

<table>
    <tr>
        <td>Zeile 1 – Spalte 1 </td>
        <td>Zeile 1 – Spalte 2</td>        
        <td>Zeile 1 – Spalte 3</td>    
    </tr>    
    <tr>
        <td>Zeile 2– Spalte 1</td>
        <td>Zeile 2 – Spalte 2</td>
        <td>Zeile 2 – Spalte 3</td>
    </tr>
</table>

### Tags

* `<table>` : Das Table-Element umschließt die ganze Tabelle

* `<tr>`: (Table row): Beschreibt eine neue Zeile

* `<td>`: (Table data): Beschreibt eine Zelle in einer Tabellenzeile. 

### Formatierung

Damit das HTML-Dokumt gut lesbar ist, rückt man die eine Ebene tiefer liegenden HTML-Tags ein. Man verwendet dazu normalerweise nicht die Leertaste sondern die Tab-Taste, da es einfacher ist so gleichmäßig einzurücken.

### Weitere Tags

* `<th>`: Ersetzt **tr** für die Kopfzeile der Tabelle

* `<caption>`: Direkt hinter dem <table>-Tag: Fügt eine Tabellenbeschriftung hinzu.

### Die Attribute Rowspan und Colspan

* `<td colspan=3>…</td>`: Die Zelle umfasst mehrere Spalten

* `<tr rowspan=3>…</tr>`: Die Zelle umfasst mehrere Zeilen.

Mehr Infos: https://wiki.selfhtml.org/wiki/HTML/Tabellen/Zellen_verbinden 

## Mehr Infos über Tabellen

Hier findest du mehr Informationen zu Tabellen: https://wiki.selfhtml.org/wiki/HTML/Tabellen 
