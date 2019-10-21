---
title: Erste Schritte (Entscheidungen if-then-else)
pre: "<b>1. </b>"
weight: 1
---

### 1. Die Mainloop

Schreibe folgenden Code:

```python
zustand = "Eingang"

while zustand!= "Ende":
  pass
```

Damit hast du eine Endlosschleife und das Grundgerüst für dein späteres Textadventure. Innerhalb dieser Endlosschleife kannst du jetzt Aktionen abfragen. 

Du kannst dein Programm in Thonny mit dem Stop-Icon beenden, sonst läuft es ewig weiter:

![How to stop Thonny](/python/thonnystop.png)

### 2. Entscheidungen 

Jetzt wird eine Entscheidung ergänzt:

```python
1 while zustand != "Ende":
2  print("Du stehst an folgendem Ort: " + zustand)
3  entscheidung = input("In welche Richtung gehst du?")
4  if zustand == "Eingang":
5    if entscheidung == "links":
6      zustand = "Seiteneingang links"
7    elif entscheidung == "rechts":
8      zustand = "Seiteneingang rechts"
9  if zustand == ...
```

### Verschachtelung:

Beachte, dass in Python die Verschachtelung von Entscheidungen eine besondere Rolle spielt. Die if-verzweigung **if entscheidung == "links"** wird nur unter der Bedingung ausgeführt, dass der Zustand = "Eingang" ist.


{{<mermaid align="left">}}
graph LR;
    A["zustand == 'Eingang'?"] -->|Ja| B(entscheidung == 'links'?)
    A -->|Nein| F("...Überprüfung des nächsten Zustands...")
    B -->|Ja| C("zustand <-- 'Seiteneingang links'")
    B -->|Nein| D("entscheidung == 'rechts'?")
    C --> F
    D -->|Ja| E("zustand <-- 'Seiteneingang rechts'")
    D -->|Nein| F
    E --> F
    F
{{< /mermaid >}}



### 3. Das Programm beenden

Spätestens jetzt macht es auch Sinn, dem Benutzer eine Möglichkeit zu geben, das Programm zu beenden:

```python
zustand = "Eingang"
while zustand != "Ende":
  print("Du stehst an folgendem Ort: " + zustand)
  entscheidung = input("In welche Richtung gehst du?")
  if zustand == "Eingang":
    if entscheidung == "links":
      zustand = "Seiteneingang links"
    elif entscheidung == "rechts":
      zustand = "Seiteneingang rechts"
    elif entscheidung == "ende":
      zustand = "Ende"
```

Geändert wurde folgender Teil: 
```python
    elif entscheidung == "ende":
      zustand = "Ende"
```
Der Benutzer kann jetzt auch immer die Option ende eingeben. Am Ende wird in den letzten Zeilen überprüft, ob die Entscheidung des Benutzers "ende" war. Wenn ja, wird das Programm beendet.

Beachte, dass du die Funktion zum Beenden an jedem möglichen Ort an dem sich der Spieler aufhalten kann, hinzufügen musst.




