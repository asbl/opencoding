---
title: Schleifen
pre: "<b>3. </b>"
weight: 3
---

## Lektion 2: Schleifen

### Aufgabe 2.1: Schleifen

Meist ist es nicht sehr effizient die selben Anweisungen mehrfach zu schreiben. 
Im folgenden Programm siehst du, wie du etwas wiederholen kannst. Die Zeilen 3 und 4 sind eingerückt - dies ist wichtig- um dem Programm mitzuteilen, dass diese Zeilen innerhalb der Schleife wiederholt werden:


import turtle
for i in range(4):
    turtle.forward(100)
    turtle.right(90)

### Aufgabe 2.2: Code analysieren

Schau dir folgendes Programm an und überlege was es tut. Zeichne das Ergebnis auf ein Blatt Papier

Folgende Fragen helfen dir bei der Analyse.

  * Wann zeichnet die Turtle, wann zeichnet sie nicht?
  
  * Welche Zeilen werden wiederholt, welche Zeilen werden nicht wiederholt?

Führe **nach deiner Analyse** den Code aus, um dich selbst zu überprüfen.

<details>
<summary>--> Lösung anzeigen</summary>

```python
import turtle
import turtle
turtle.penup()
turtle.backward(300)
turtle.pendown()
for i in range(4):
   turtle.forward(100)
   turtle.right(90)
turtle.penup()
turtle.forward(150)
turtle.pendown()
for i in range(4):
   turtle.forward(100)
   turtle.right(90)
```
</details>



### Aufgabe 2.3: Quadrate

Zeichne das folgende Muster. Verwende für das Muster (So wie für alle folgenden Muster) Schleifen um möglichst wenige Befehle zu verwenden.

![Quadrate](/python/quadrate.jpg)

### Aufgabe 2.4: Pentragramm 

Zeichne folgendes Muster

![Fünfzackiger Stern(/python/fuenfzackiger_stern.jpg)


### Aufgabe 2.5: Pentragramme 

Zeichne folgendes Muster

![Fünfzackige Sterne](/python/fuenfzackige_sterne.jpg)

### Aufgabe 2.6: Stern

Zeichne folgendes Muster

![Stern](/python/viele_zacken.jpg)

### Aufgabe 2.7: Größer werdende Rechtecke

Zeichne folgendes Muster

![Beispiel 1](/python/rechtecke.jpg)

