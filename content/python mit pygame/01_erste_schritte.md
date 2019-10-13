---
title: Erste Schritte
pre: "<b>1. </b>"
weight: 1
---

### Installation 


#### Thonny

Installiere über **Tools -> Manage Packages** die Bibliothek pygame


### Erste Schritte 


Folgender Code erstellt ein Fenster, dass sofort wieder verschwindet:

```python
import pygame

pygame.init()
screen = pygame.display.set_mode((200,100))
```

#### Die Mainloop 

Nun brauchst du eine Mainloop.
Ergänze dazu folgenden Code:

```python
running = True
     
    while running:
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                running = False

```

### Bilder zeichnen 

Zeichne etwas auf den Bildschirm.

Dazu brauchst du 3 Zeilen Code:


```python
image = pygame.image.load("[Dateiname].png")
```

Diese Zeile lädt das Bild. Achtung: Das Bild muss im selben Verzeichnis wie dein Programm liegen und du musst den Dateinamen entsprechend setzen

```python
screen.blit(image, (50,50))
```

Diese Zeile blittet das Bild an die Position (50|50) (beachte, dass der Ursprung beim Bildschirm in der oberen Ecke sitzt)


```python
pygame.display.flip()
```

Diese Zeile sorgt dafür, dass das Display neu geladen wird. Gegebenfalls musst du dein Bild noch skalieren. Dies geht über folgenden Befehl:

```python
image = pygame.transform.scale(image, (20, 20))
```

So könnte dein Programm aussehen:

```python
import pygame

pygame.init()

screen = pygame.display.set_mode((200,100))

running = True
image = pygame.image.load("smiley.jpg")
image = pygame.transform.scale(image, (20, 20))
screen.blit(image, (50,50))
while running:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False
    pygame.display.flip()
```

### Transparente Farben

Manchmal möchte man, dass eine Farbe transparent gezeichnet wird. Dies geht mit:

```python
image.set_colorkey((255,255,255)) # Die Farbe weiß soll transparent sein.
```

===== Hintergründe =====

Den Hintergrund des Bildschirms kannst du folgendermaßen setzen

```python
screen.fill((r,g,b))
```

r,g,b sind jeweils Zahlen zwischen 0 und 256 und die Anteile von red, green und blue in der Farbe. Hier findest du einen Farbwähler: https://www.rapidtables.com/web/color/RGB_Color.html

Du kannst auch ein Bild als Hintergrund wählen:

```python
screen.blit(bgd_image, (0,0))
```

===== Bewegungen =====


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

Hier findest du ein umfangreicheres Tutorial: https://dr0id.bitbucket.io/legacy/pygame_tutorials.html