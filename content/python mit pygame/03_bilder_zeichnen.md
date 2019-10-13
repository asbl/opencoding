---
title: Bilder zeichnen
pre: "<b>3. </b>"
weight: 3
---

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

### Hintergründe 

Den Hintergrund des Bildschirms kannst du folgendermaßen setzen

```python
screen.fill((r,g,b))
```

r,g,b sind jeweils Zahlen zwischen 0 und 256 und die Anteile von red, green und blue in der Farbe. Hier findest du einen Farbwähler: https://www.rapidtables.com/web/color/RGB_Color.html

Du kannst auch ein Bild als Hintergrund wählen:

```python
screen.blit(bgd_image, (0,0))
```
