---
title: Funktionen
pre: "<b>3. </b>"
weight: 3
---

Je komplexer unser Programm wird, umso mehr macht es Sinn, Teile in Unterprogramme auszulagern. Dies geht mi    elif entscheidung == "ende":
      zustand = "Ende"t Hilfe von Funktionen.

An dieser Stelle wird eine Funktion Haupteingang geschrieben:

```python
def haupteingang():
    easygui.msgbox("Du stehst am Eingang")
    entscheidung = easygui.buttonbox("Wohin gehst du", "Mein Textadventure", ["links", "rechts", "ende"])
    if entscheidung == "links":
        neuer_zustand = "Seiteneingang links"
    elif entscheidung == "rechts":
        neuer_zustand = "Seiteneingang rechts"
    elif entscheidung == "ende":
        zustand = "Ende"
    return neuer_zustand
```

Das Unterprogramm trägt den Namen Haupteingang und hat den Parameter entscheidung. Abhängig von dem, was als Wert für entscheidung übergeben wird, gibt das Unterprogramm einen anderen Wert zurück.

Im Hauptprogramm können wir nun folgendermaßen auf das Unterprogramm zugreifen:

```python
import easygui

def haupteingang():
    easygui.msgbox("Du stehst am Eingang")
    entscheidung = easygui.buttonbox("Wohin gehst du", "Mein Textadventure", ["links", "rechts", "ende"])
    if entscheidung == "links":
        neuer_zustand = "Seiteneingang links"
    elif entscheidung == "rechts":
        neuer_zustand = "Seiteneingang rechts"
    elif entscheidung == "ende":
        zustand = "Ende"
    return neuer_zustand


zustand = "Eingang"
while zustand != "Ende":
    if zustand == "Eingang":
        zustand = haupteingang()

```


Auf diese Weise können wir weitere Unterprogramme hinzufügen:



Auf diese Weise wird dein Code besser lesbar, da du einzelne Teile in die entsprechenden Unterprogramme auslagern kannst.
