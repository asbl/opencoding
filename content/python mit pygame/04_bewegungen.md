---
title: Bewegungen
pre: "<b>4. </b>"
weight: 4
---


Bewegungen kannst du hinzufügen, wenn du die festen Koordinaten, an die du ein Bild geblittet hast, variabel machst:

```python
x = 10
y = 10
stepx = 1
stepy = 1
while running:
    screen.blit(image, (x, y))
    x = x+stepx
``` 

Wie du siehst entstehen zwei Probleme:

1. Dein Bild hinterlässt eine Spur
2. Dein Bild verschwindet aus dem Bildschirm.

Problem 1. lässt sich lösen, indem man zu Beginn der Mainloop immer erstmal den kompletten Bildschirm löscht:

```python
while running:
    screen.fill((20, 20, 20))
    screen.blit(image, (x, y))
    ...
```
Problem 2 lässt sich lösen, in dem man testet, ob das Bild außerhalb des Sichtbereiches ist.

```
    if x> screen.get_width() or x<0:
        stepx = stepx * (-1)
    x = x+ stepx
```

