Vorlesung 3
===========

Zeitraum: 10. April,	15:30 - 17:45

Ort: FH Joanneum, G.AP152.108

Folien: [scripting-und-coding_3_folien.pdf](scripting-und-coding_3_folien.pdf)


Dokumente und verlinkte Seiten
------------------------------

 - [http://explorabl.es](http://explorabl.es/)
 - [Syrian Journey: Choose your own escape route](http://www.bbc.com/news/world-middle-east-32057601)
 - [Wikipedia: Algorithmus](https://de.wikipedia.org/wiki/Algorithmus)
 - [Wikipedia: Programmiersprache](https://de.wikipedia.org/wiki/Programmiersprache)
 - [Wikipedia: Programmierung](https://de.wikipedia.org/wiki/Programmierung)
 - [CrashCourse: Computer Science](https://www.youtube.com/playlist?list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo)
 - [Ada Lovelace](https://de.wikipedia.org/wiki/Ada_Lovelace)
 - [Hidden Figures](https://www.rottentomatoes.com/m/hidden_figures/)
 - [Wikipedia: Skriptsprache](https://de.wikipedia.org/wiki/Skriptsprache)
 - [joy.js von ncase](http://ncase.me/joy/demo/turtle/?drawing=blank)
 - [MDN: Javascript](https://developer.mozilla.org/bm/docs/Web/JavaScript)
 - [jQuery](https://jquery.com/)
 - [CodePen: Hallo Welt!](https://codepen.io/PeterTheOne/pen/eMxvMw?editors=1010)
 - [CodePen: Variablen (Zwischenspeichern)](https://codepen.io/PeterTheOne/pen/VXgpqb?editors=1010)
 - [CodePen: jQuery “CSS” Selektoren](https://codepen.io/PeterTheOne/pen/wmNdaQ?editors=1010)
 - [CodePen: Operationen (Rechnen)](https://codepen.io/PeterTheOne/pen/yKZPXo?editors=1010#0)
 - [CodePen: Body mass index](https://codepen.io/PeterTheOne/pen/JLxMrd?editors=1010#0)
 - [CodePen: Vergleiche](https://codepen.io/PeterTheOne/pen/MVLrqd?editors=1010)
 

Inhalt
------

...


### Hallo Welt

Es gibt drei verschiedene Möglichkeiten etwas auzugeben.

 - `alert('Hallo Welt!');`: Alert popupfenster
 - `console.log('Hallo Welt!');`: Nur sichtbar wenn man im Browser die Seite untersucht.
 - Text im HTML einfügen:
   - `document.getElementById('textField').innerText = 'Hallo Welt!';` oder
   - `$('#textField').text('Hallo Welt!');` (jQuery)


### Variablen (Zwischenspeichern)
    
Variablen sind Zwischenspeichern, ein Wert kann damit mit einem Namen/Label versehen werden auf dass dann später wieder zugegriffen werden kann. Beim ersten definieren (initialisieren) einer Variable verwendet man `var`. Danach kommt der Name der Variable den man selbst wählen kann. Der Wert der Variable wird mit einem "ist gleich" `=` der Variable zugewiesen. Hinter Gleichheitszeichen steht der Wert, abgeschlossen wird die zeile mit einem Strichpunkt `;`.

Es gibt verschiedene Typen von Werten: Texte bzw. Zeichenketten auch String genannt, Logische Werte als Boolean, Zahlen als Integer oder Float (Kommazahlen).

Der Wert einer Variable kann man nach der ersten zuweisung ändern in dem man der Variable erneut mit einem "ist gleich" `=` einen Wert zuweist. (Dabei braucht es nicht mehr das Wort `var`).

```
var welcomeText = 'Hallo Welt!';          // String
var raining = true;                       // Boolean
raining = false;
var personCount = 5;                      // Integer
var happiness = 0.9;                      // Float
```

### jQuery CSS Selektoren

(siehe Slides)

### Operationen (Rechnen)

(siehe Slides)
    
### Vergleiche

(siehe Slides)
