---
title: Zufall
pre: "<b>6. </b>"
weight: 6
---

###  Aufgabe 1: Zufällige Rechtecke

Erstelle ein neues Programm.

Damit wir zufällige Quadrate zeichnen können, benötigen wir die random() Funktion. Wir werden eine zufällige Zahl erstellen und dann dieser Zahl eine Farbe zuweisen.

Betrachte dazu folgendes Programm
(Hinweis: Zeilen, die mit # beginnen sind Kommentare, die vom Computer nicht gelesen werden, sondern dazu gedacht sind von Menschen gelesen zu werden):

<iframe height="400px" width="100%" src="https://repl.it/@a_siebel/Zufall?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

  * **if** bedeutet: Falls die Bedingung gegeben ist, führe den eingerückten Code aus.
  * **elif** bedeutet: Falls die If-Bedingung nicht zutrifft, führe den eingerückten Code aus.

#### Aufgabe

Führe das Programm aus und vollziehe nach, was passiert.

### Aufgabe 2 

Erweitere das Programm so, dass die Rechtecke in einer von 5 Farben deiner Wahl gezeichnet werden.

### Aufgabe 3: In Funktion auslagern 

Der Code zum Auswählen von Farben soll im Programm immer wieder verwendet werden. Daher lagern wir ihn in eine Funktion aus.

Die Funktion soll folgendes tun:

  * Hole dir eine beliebige Zufallszahl
  * Hole dir die Farbe, die zu dieser Zufallszahl passt.
  * Gebe diese Zahl an das Hauptprogramm zurück (dafür verwendet man die **return-Anweisung**

<details>
<summary>--> Lösung anzeigen</summary>

```python
import random
import turtle
def getcolour():
    colnum = random.randint(1, 2)
    if colnum == 1:
        colour = "Red"
    elif colnum == 2:
        colour = "Blue"
    return colour

pc = getcolour()
turtle.pencolor(pc)
for i in range(4):
    turtle.forward(50)
    turtle.right(90)
```

#### Aufgabe
Führe das Programm aus und schaue was passiert.

### Aufgabe 3:

Erweitere das Programm so, dass das Quadrat mit einer zufälligen Farbe gefüllt wird.
(Du benötigst dafür 4 Zeilen Code). 


### Aufgabe 4:

Füge die getcolour() Funktion zu deinem Programm hinzu, in dem du ein Netz aus Rechtecken gezeichnet hast (Verwende dazu Copy & paste, schreibe nicht das ganze Programm ab). Ändere das Programm nun so ab, dass:

  * Quadrate in zufälligen Farben gezeichnet werden.
  * Quadrate in zufälligen Farben gefüllt werden.


