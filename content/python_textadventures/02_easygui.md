---
title: Easygui
pre: "<b>2. </b>"
weight: 2
---

## Eine grafische Benutzeroberfläche

### Installation

#### Thonny:
Installiere zunächst das Package Easy-Gui

  * Wähle dazu in Thonny das Menü: **"Tools" -> "Manage Packages"**

  * Suche nach EasyGui und klicke auf install.

#### repl.it

In repl.it werden Pakete automatisch installiert, wenn du sie mit der import-Anweisung importierst.


### Erste Schritte
Jetzt kannst du folgendermaßen EasyGui Dialoge einbinden.

```python
import easygui
zustand = "Eingang"
while zustand != "Ende":
  easygui.msgbox("Du stehst an folgendem Ort: " + zustand, "Mein Textadventure")
  entscheidung = easygui.buttonbox("Wohin gehst du", "Mein Textadventure", ["links", "rechts"])
  if zustand == "Eingang":
    if entscheidung == "links":
      zustand = "Seiteneingang links"
    elif entscheidung == "rechts":
      zustand = "Seiteneingang rechts"
    elif entscheidung == "ende":
      zustand = "Ende"
```

In den Zeilen 4 und 5 wurden jeweils die Dialoge durch Gui Elemente ersetzt.