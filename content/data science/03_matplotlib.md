---
title: Matplotlib
pre: "<b>3. </b>"
weight: 3
---

Installiere in Thonny die Bibliothek matplotlib und importiere diese:

```
import matplotlib as mlp
import matplotlib.pyplot as plt
```

(Das Alias as im Import sagt, dass du die Bibliothek in Zukunft mit mpl aufrufen kannst - So sparst du dir Schreibarbeit)

Jetzt kannst du deinen ersten Plot anzeigen:

```
plt.plot([1,2,3,4], [1,4,9,16], 'bo')
plt.show()
```

  * Das erste Argument der Funktion ist eine Liste mit x-Werten
  
  * Das zweite Argument der Funktion ist eine Liste mit y-Werten

  * Das dritte Argument ist ein Format-String, der dir es leicht erlaubt, das Aussehen des Plots zu verwenden. Dieser besteht aus mehreren Teilen.

#### Farbe

^ Buchstabe  ^ Farbe    ^
| 'b'        | blue     |
| 'g'        | green    |
| 'r'        | red      |
| 'c'        | cyan     |
| 'm'        | magenta  |
| 'y'        | yellow   |
| 'k'        | black    |
| 'w'        | white    |
|            |          |

#### Markierung 

^ Buchstabe  ^ Markierung             ^
| '.'        | point marker           |
| ','        | pixel marker           |
| 'o'        | circle marker          |
| 'v'        | triangle_down marker   |
| '%%^%%'        | triangle_up marker     |
| '%%<%%'        | triangle_left marker   |
| '%%>%%'        | triangle_right marker  |
| '1'        | tri_down marker        |
| '2'        | tri_up marker          |
| '3'        | tri_left marker        |
| '4'        | tri_right marker       |
| 's'        | square marker          |
| 'p'        | pentagon marker        |
| '*'        | star marker            |
| 'h'        | hexagon1 marker        |
| 'H'        | hexagon2 marker        |
| '+'        | plus marker            |
| 'x'        | x marker               |
| 'D'        | diamond marker         |
| 'd'        | thin_diamond marker    |
| '%%|%%'        | vline marker           |
| '_'        | hline marker           |

#### Linien

^ Buchstabe  ^ Linie                ^
| '-'        | solid line style     |
| '--'       | dashed line style    |
| '-.'       | dash-dot line style  |
| ':'        | dotted line style    |
