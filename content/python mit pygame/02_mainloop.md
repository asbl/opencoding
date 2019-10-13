---
title: Die Mainloop
pre: "<b>2. </b>"
weight: 2
---

Nun brauchst du eine Mainloop, d.h. eine Schleife die ständig läuft, bis die Zustandsvariable **running** den Wert **False** annimmt (z.B. wenn der Benutzer auf das x-Symbol des Fensters klickt.)


Ergänze dazu folgenden Code:

```python
running = True
     
    while running:
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                running = False

```
