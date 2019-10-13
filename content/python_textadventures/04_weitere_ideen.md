---
title: Weitere Ideen
pre: "<b>4. </b>"
weight: 4
---

### Zufall 

Oft sollen Dinge vom Zufall abhängen. Dies kannst du in Python folgendermaßen machen:

```python
import random

print("Würfle mit einem Würfel")
wuerfel = random.randint(1,6)
print(wuerfel)
```

Überlege dir, wie du mit Hilfe dieser Funktion Zufallszahlen in dein Programm einbauen kann

### Inventar - Für fortgeschrittene

Wenn es viele mögliche Gegenstände gibt, die ein Charakter mit sich führen kann, dann wird es schnell unübersichtlich, wenn du für jeden Gegenstand eine einzelne Variable hinzufügst. 

Dafür gibt es in Python Listen:

```
inventar = []
```

erstellt eine neue Liste

```python
inventar.append("Schlüssel")
```

fügt einen Schlüssel zum Inventar hinzu.

```python
inventar.remove("Schlüssel")
```

löscht den Schlüssel aus dem Inventar.

Mit folgender Anweisung
```python
if "Schluessel" in inventar:
 ...
```

kannst du überprüfen, ob ein Charakter den Gegenstand mit sich führt.


### Inventar an Funktionen übergeben

Die Inventar-Variablen muss irgendwo im Hauptprogramm definiert werden. Damit die Variable auch in den Unterprogrammen bekannt ist, muss sie als Parameter übergeben werden.

```python
inventar = []
zustand = "Anfang"

....

def tue_irgendetwas(inventar)
  if "Gegenstand" in inventar:
      inventar.append("neuer Gegenstand")
    
# Hier kommt das Hauptprogramm

while zustand != Ende
  tue_irgendetwas(inventar)
```