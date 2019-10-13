---
title: Zufallsmuster
pre: "<b>7. </b>"
weight: 7
---

### Aufgabe 1: Grundsätzliche Überlegungen

Das folgende Programm erstellt eine Form:

```python
import turtle

def shape():
  for i in range(4):
    turtle.forward(50)
    turtle.right(90)
 
shape()
```

Beantworte folgende Fragen, passe das Programm dafür an:

  * Wie müsste man das Programm verändern, wenn man eine dreiseitige Figur erstellen möchte?

  * Wie müsste man das Programm verändern, wenn man eine fünfseitige Figur erstellen möchte?

  * Was ist die Beziehung zwischen Seitenanzahl und Winkel, den die Turtle zeichnen muss.

  * Was benötigst du noch, wenn du eine zufällige Figur zwischen 3 und 6 Ecken zeichnen möchtest?

### Aufgabe 2: Parameter

Damit das Unterprogramm beliebige Formen zeichnen kann, musst das Unterprogramm wissen, wie viele Seiten die Figur haben soll. Du kannst dies mit Hilfe von Parametern realisieren.

Betrachte dazu folgendes Programm

def shape(anzahl):
    print(anzahl)
    
anzahl = 3
shape(anzahl)


Probiere aus, was passiert, wenn du den Wert für Anzahl in Zeile 3 durch 4,5 oder 6 ersetzt.

Hinweis: In repl.it siehst du die Ausgabe mit Klick auf **Console**

### Aufgabe 3: Parameter verwenden 

Du kannst den Namen Anzahl in deiner Funktion wie eine Zahl verwenden.

```python
def shape(anzahl):
  for i in range(anzahl):
    turtle.forward(100)
    turtle.right(...)
 
shape()
```

Finde den richtigen Ausdruck für ... heraus, so dass die Figur mit der richtigen Anzahl an Seiten gezeichnet wird. Du kannst in die Klammern aus Rechenausdrücke einsetzen, wie z.B. anzahl*10,  anzahl / 10, .... 

### Aufgabe 4: Parameter verwenden

Erweitere deine Programme aus den vorherigen Übungen so, dass zufällige Figuren gezeichnet werden.