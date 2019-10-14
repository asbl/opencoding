---
title: Funktionen 
pre: "<b>5. </b>"
weight: 5
---

### Aufgabe 1 

Wenn du größere Programme schreibst, ist es am einfachsten, wenn du diese in **Teilprogramme** zerlegen kannst.

In Python funktioniert dies mit Funktionen (oder auch Subroutinen). Das folgende Programm erstellt eine Funktion, um ein kleines Quadrat zu zeichnen. Anschließend wird die Funktion einmal aufgerufen:

```python
import turtle
def square():
  for i in range(4):
    turtle.forward(30)
    turtle.right(90)
square()
```

  * Das Schlüsselworts **def** steht für define. Mit diesem Schlüsselwort wird signalisiert, dass im folgenden eine Funktion definiert wird.
  
  * Anschließend folgt der Name der Funktion. Diese Funktion heißt square, denn es soll ein Quadrat gezeichnet werden. Nach dem Funktionsnamen folgen zwei Klammern und ein Doppelpunkt.

  * Der Inhalt der Funktion ist eingerückt. Hier wird beschrieben, was bei Aufruf der Funktion passieren soll.

Um die Funktion aufzurufen schreibt man den Namen der Funktion gefolgt von den beiden Klammern im Programm auf.

**Aufgabe:**

Führe das oben beschriebene Programm aus und schaue was passiert.

### Aufgabe 2

Erstelle selbst eine eigene Funktion:

  * Nenne sie nextshape
  * Die Funktion soll folgendes tun:
    * Hebe den Stift an.
    * Bewege dich um 60 vorwärts.
    * Senke den Stift.

Schreibe ein Programm, dass mit Hilfe der Funktion 3 Quadrate zeichnet:

Hinweis: So funktionieren Funktionsaufrufe

```python
square()
nextshape()
square()
nextshape()
square()
```

<details>
<summary>--> Lösung anzeigen</summary>

```python
import turtle

def square():
    for i in range(4):
        turtle.forward(30)
        turtle.right(90)

def nextshape():
    turtle.penup()
    turtle.forward(60)
    turtle.pendown()
    
square()
nextshape()
square()
nextshape()
square()
```
</details>

#### Exkurs: Namen bekannt machen

In jeder Programmiersprache müssen Namen zuerst bekannt gemacht werden, bevor sie benutzt werden können. Dies gilt für Variablen aber auch für Funktionen.

Daher führt folgendes Programm zu einem Fehler
```python
square()

def square():
    for i in range(4):
        turtle.forward(30)
        turtle.right(90)
```

Python kann die Funktion in Zeile 1 noch nicht aufrufen, da an dieser Stelle der Name der Funktion noch nicht bekannt ist.

### Aufgabe 3: 10 Rechtecke
Ändere das Programm so ab, dass 10 Rechtecke gezeichnet werden. Verwende dafür eine for-Schleife.

### Aufgabe 4: nextrow

Erstelle eine Funktion **nextrow**, die folgendes macht.

  * Hebe den Stift an
  * Gehe 600 Schritte rückwärts
  * Bewege dich 60 Schritte nach unten
  * Drehe dich so, dass du nach rechts schaust.

Teste dein Programm, in dem du das Programm aus Aufgabe 3 so erweiterst, dass zwei Reihen mit 6 Rechtecken gezeichnet werden.

Hinweis: Mit folgender Anweisung kannst du die Turtle schneller bewegen:

```python
turtle.speed(10)
```

...oder noch schneller:

```python
turtle.speed(0)
```

<details>
<summary>--> Lösung anzeigen</summary>

```python
import turtle

def square():
    for i in range(4):
        turtle.forward(30)
        turtle.right(90)

def nextshape():
    turtle.penup()
    turtle.forward(60)
    turtle.pendown()

def nextrow():
    turtle.penup()
    turtle.backward(600)
    turtle.right(90)
    turtle.forward(60)
    turtle.left(90)
    turtle.pendown()

turtle.speed(10)

for i in range(10):
    square()
    nextshape()
nextrow()
for i in range(10):
    square()
    nextshape()
```
</details

### Aufgabe 5: Ein Netz aus Quadraten

Erweitere das Programm und erstelle ein 10x10 Netz an Rechtecken.

  * Erstelle eine Routine gotostart(), die die Turtle 300 nach links und 300 nach oben bewegt, damit das komplette Netz im sichtbaren Bereich gezeichnet wird.
  
  * Verwende eine Schleife um auf die gleiche Weise wie du die 10 Rechtecke gezeichnet hast auch 10 Reihen zu zeichnen. So kann ein Ansatz dafür aussehen:
  
```python
for i in range(10):
    for j in range(10):
        ...
```

<details>
<summary>--> Lösung anzeigen</summary>

```python
for i in range(10):
    for j in range(10):
        square()
        nextshape()
    nextrow()
```
</details>

====== Aufgabe 5: Mehrfarbiges Grid ======

Erstelle ein mehrfarbiges Grid. 

  * Suche dir dazu zusammen, was du benötigst. Hier findest du eine Übersicht über alle Turtle-Funktionen: https://docs.python.org/3.3/library/turtle.html?highlight=turtle