---
title: Konzept - Trennung von Inhalt, Struktur und Layout
---

### Warum sollte man überhaupt Inhalt, Struktur und Layout trennen?

Einer der Kernideen von HTMl+CSS ist es, Inhalt, Layout und Struktur zu trennen.

Dies hat folgende Vorteile:

  * Ein Text kann unabhängig vom Ausgabemedium erstellt werden. Eine Webseite soll z.B. anders aussehen, je nachdem ob sie auf einem PC, Handy oder Tablet dargestellt werden soll. 

  * Kollaboratives Arbeiten: Wenn du in Word-Dateien ohne Trennung von Layout/Inhalt/Struktur zusammenarbeitest, dann muss auch jeder Bearbeiter des Dokuments am Layout mitarbeiten, selbst wenn er z.B. nur ein Lektorat macht. Das gemeinsame Arbeiten sollte daher am besten nur auf dem Text basieren und das Layout unabhängig davon erstellt werden.

### Inhalt

Dies ist der eigentliche Inhalt.

### Struktur

Informationen darüber, wie der Inhalt strukturiert ist (Überschriften, Listen, ...)

### Layout

Informationen darüber, wie der Inhalt gestaltet ist.


### Wo findet man dieses Prinzip?

Dieses Prinzip trifft man an unterschiedlicher Stellen in der Informatik:

  - Bei graphischen Benutzeroberflächen (GUIS) sollte der Code für die Anzeige, das Datenmodell und die Steuerung getrennt werden (Pattern: Model View Controler)

  - In Word&co kannst du mit Hilfe von Formatvorlagen Inhalt und Layout trennen. Beim Bearbeiten legst du Formatvorlagen fest (Überschrift, Listen, ...) und kannst an anderer Stelle für eine komplette Formatvorlage das Layout ändern.

  - HTML dient als **Schnittstelle** zwischen Programmiern und Designern: Programmierer erstellen oft mit Hilfe von Frameworks HTML-Code. Die Designer können dann diesen HTML-Code mit Hilfe von CSS gestalten ohne Wissen darüber zu besitzen, wie dieser HTML-Code genau generiert wird.