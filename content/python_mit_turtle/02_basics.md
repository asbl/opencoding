---
title: "Python Basics"
pre: "<b>2. </b>"
weight: 1
---


### Operationen 

| Befehl                    | Beschreibung                                             |
| ------------------------- | -------------------------------------------------------- |
| turtle.forward()          | Gehe vorwärts                                            |
| turtle.backward()         | Gehe rückwärts                                           |
| turtle.right(x)           | Drehe dich um x Grad nach rechts                         |
| turtle.left(x)            | Drehe dich um x Grad nach links                          |
| turtle.penup()            | Hebe den Stift an (Bewege dich weiter, ohne zu zeichnen) |
| turtle.pendown()          | Setzt den Stift wieder ab, so dass du weiterzeichnest    |
| turtle.fillcolor("brown") | Ändert die Füllfarbe auf Braun                           |
| turtle.pencolor("red")    | Ändert die Stiftfarbe auf rot                            |
| turtle.begin_fill()       | Beginnt die Figur zu füllen                              |
| turtle.end_fill()         | Beendet das Füllen                                       |



### Grundlagen


Ein erster Code kann folgendermaßen aussehen:

<iframe height="400px" width="100%" src="https://repl.it/@a_siebel/First-example?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>


### Aufgabe 1.2: Zeichne ein Quadrat mit roter Stiftfarbe 

Zeichne ein Quadrat mit roter Stiftfarbe wie im folgenden Beispiel:

![Beispiel 1](/python/1.jpg)

{{%expand "--> Lösung anzeigen" %}}

```python
import turtle
turtle.fillcolor(“Brown”)
turtle.begin_fill()
turtle.pencolor(“Red”)
turtle.forward (100)
turtle.right (90)
turtle.forward (100)
turtle.right (90)
turtle.forward (100)
turtle.right (90)
turtle.forward (100)
turtle.end_fill()
```
{{% /expand%}}



### Aufgabe 1.3: Zeichne ein Quadrat (2) 

Zeichne ein Quadrat mit den Seitenlängen 180 mit einer lila ("purple") Linie und blauer ("blue) Füllungimport turtle

![Beispiel 2](/python/2.jpg)


{{%expand "--> Lösung anzeigen" %}}
```python
import turtle
turtle.pencolor("purple")
turtle.fillcolor("blue")
turtle.begin_fill()
turtle.forward (180)
turtle.right (90)
turtle.forward (180)
turtle.right (90)
turtle.forward (180)
turtle.right (90)
turtle.forward (180)
turtle.end_fill()
```
{{% /expand%}}

### Aufgabe 1.4: Zeichne ein Rechteck 

Zeichne ein Rechteck:


![Beispiel 3](/python/3.jpg)


{{%expand "--> Lösung anzeigen" %}}
```python
import turtle
turtle.forward (150)
turtle.right (90)
turtle.forward (80)
turtle.right (90)
turtle.forward (150)
turtle.right (90)
turtle.forward (80)
```
{{% /expand%}}

###  Aufgabe 1.5: Zeichne zwei Rechtecke

Ergänze Aufgabe 4 um ein zweites Rechteck, dass angezeigt werden soll. Die Rechtecke sollen sich nicht berühren. 
Verwende dafür pen up & pen down.


![Beispiel 4](/python/4.jpg)


{{%expand "--> Lösung anzeigen" %}}
```python
import turtle
# Erstes Rechteck
turtle.forward (150)
turtle.right (90)
turtle.forward (80)
turtle.right (90)
turtle.forward (150)
turtle.right (90)
turtle.forward (80)

# Stift anheben und weiterbewegen
turtle.penup()
turtle.forward(20)
turtle.pendown()
# Zweites Rechteck
turtle.forward (80)
turtle.right (90)
turtle.forward (150)
turtle.right (90)
turtle.forward (80)
turtle.right (90)
turtle.forward (150)
```
{{% /expand%}}

### Aufgabe 1.6: Zeichne ein Dreieck

Zeichne ein Dreieck

![Beispiel 5](/python/5.jpg)


{{%expand "--> Lösung anzeigen" %}}
```python
import turtle
import turtle
turtle.forward (150)
turtle.right (120)
turtle.forward (150)
turtle.right (120)
turtle.forward (150)
turtle.right (120)
```
{{% /expand%}}

### Aufgabe 1.7: Zeichne Figuren

Zeichne mindestens zwei der folgenden Figuren:

  * Regelmäßiges Fünfeck
  * Regelmäßíges Sechseck
  * Regelmäßiges Achteck
  * Regelmäßiges Zwölfeck





