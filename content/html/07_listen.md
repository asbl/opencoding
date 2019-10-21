---
title: Listen
pre: "<b>7. </b>"
weight: 7
---

## Arbeitsauftrag

Erstelle verschiedene Arten von Listen in deinem Dokument.

## Syntax

Listen können ähnlich wie Tabellen erstellt werden:

## Syntax

### Ungeordnete Listen:
```
<ul>
    <li>Unterpunkt 1</li>
    <li>Unterpunkt 2</li>
</ul>
```

... wird zu:

<ul>
    <li>Unterpunkt 1</li>
    <li>Unterpunkt 2</li>
</ul>

### Nummerierte Listen

```
<ol>
    <li>Unterpunkt 1</li>
    <li>Unterpunkt 2</li>
</ol>
```

... wird zu:

<ol>
    <li>Unterpunkt 1</li>
    <li>Unterpunkt 2</li>
</ol>

## Definitionslisten:

Weiterhin gibt es noch Definitionslisten z.B. für Listen von Abkürzungen oder Vokabeln:

Definitionslisten werden mit dem Tag `<dl>` umschlossen.
  
  * `<dt>` Bezeichnet den Term der Beschrieben werden soll
  
  * `<dd>` Bezeichnet die Beschreibung des Terms.

Beispiel:

```html
<dl>
  <dt>DNS</dt> <dd>Domain Name Service</dd> 
  <dt>IP</dt> <dd>Internet Protocoll</dd>
</dl>

```
