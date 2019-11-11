---
title: Links und Pseudoklassen
pre: "<b>12. </b>"
weight: 12
---

## Arbeitsauftrag

Erstelle einen Link und gestalte mit CSS den Link unterschiedlich je anchdem, ob dieser bereits besucht wurde oder noch nicht besucht wurde. Füge einen Hover-Effekt beim Überfahren mit der Maus hinzu.

## Theorie: Pseudoklassen

Beim gestalten von Links gibt es eine Besonderheit, die man beachten muss:

Links können verschiedene Zustände haben, je nachdem, ob diese bereits besucht wurden. Man kann diese folgendermaßen stylen: 


**a:link** bezeichnet einen noch nicht besuchten Link.
**a:visited** bezeichnet einen besuchten Link.

Man nennt dies auch **Pseudoklassen**. Weitere Pseudoklassen sind **a:hover** wenn die Maus gerade über einen Link fährt sowie **a:active** für einen ausgewählten Link. 

### Reihenfolge der Definitionen

a:hover muss dabei nach a:link und a:visited definiert werden, damit es einen Effekt hat.
Man kann mit hover auch andere Elemente stylen.

## Weitere Pseudoklassen

Es gibt noch weitere Pseudo-Klassen, mit denen man Elemente auswählen kann, z.B.
li:nth-child(even) um nur gerade Listenelemente auszuwählen. Siehe: https://wiki.selfhtml.org/wiki/CSS/Selektoren/Pseudoklasse/strukturelle_Pseudoklasse/nth-child 