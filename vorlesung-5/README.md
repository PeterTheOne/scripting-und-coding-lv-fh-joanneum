Vorlesung 5
===========

Zeitraum: 12. April, 14:00 - 16:15

Ort: FH Joanneum, G.AP152.108

Folien: [scripting-und-coding_5_folien.pdf](scripting-und-coding_5_folien.pdf)


Dokumente und verlinkte Seiten
------------------------------

 - [CodePen: Schleifen](https://codepen.io/PeterTheOne/pen/PRLmWa?editors=1010)
 - [CodePen: Objekte (Dictionary / JSON)](https://codepen.io/PeterTheOne/pen/zWbwjK?editors=1010)
 - [JSON](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON)
 - [https://petertheone.github.io/bpw16-vis/](https://petertheone.github.io/bpw16-vis/)
 - [https://neuwal.github.io/barometer/](https://neuwal.github.io/barometer/)
 - [http://feinstaub-graz.at/](http://feinstaub-graz.at/)
 - [CodePen: show, hide (jQuery)](https://codepen.io/PeterTheOne/pen/MVRobe?editors=1010)
 - [.hide() (jQuery)](https://api.jquery.com/hide)
 - [.show() (jQuery)](https://api.jquery.com/show/)
 - [CodePen: Add / remove Class (jQuery)](https://codepen.io/PeterTheOne/pen/PRgjJv)
 - [.addClass() (jQuery)](https://api.jquery.com/addClass/)
 - [.removeClass() (jQuery)](https://api.jquery.com/removeClass/)
 - [CodePen: on click (jQuery)](https://codepen.io/PeterTheOne/pen/bvJrwB?editors=1010)

Inhalt
------

### Schleifen

Wenn man in programmiersprachen etwas mehrfach ausführen will kann man entweder dieses 
etwas mehrfach hinschreiben oder man verwendet schleifen. Eine Schleife besteht 
Grundsätzlich aus zwei Teilen: Der erste Teil `(...)` bestimmt wie lange bzw. wie oft 
die Schleife ausgeführt wird, der zweite Teil `{...}` beinhaltet was bei jedem 
ausführen passieren soll.

Der erste Teil der for-Schleife `for (...)` besteht selbst wieder aus drei Bereichen 
die durch einen Strichpunkt `;` getrennt sind: 1. Wird nur ein Mal am Beginn 
ausgeführt, 2. Wird jedes Mal überprüft (wenn `true` wird die Schleife weiter ausgeführt, 
wenn `false` wird die Schleife abgebrochen), 3. Wird jedes Mal am Ende ausgeführt
`for(einMalAmBeginn; jedesMalÜberprüft; jedesMalAmEnde)`.

```
var books = ["Animal", "The Little Prince", "Fahrenheit 451"];

for (var i = 0; i < books.length; i = i + 1) {
  $("#list").append("<li>" + books[i] + "</li>");
}

```

### Objekte (Dictionary / JSON)

(siehe Slides)


### show, hide (jQuery)

 - [.hide() (jQuery)](https://api.jquery.com/hide)
 - [.show() (jQuery)](https://api.jquery.com/show/)

```
$('#navy').hide();
$('.round').hide();
$('.fontsizes').show();
```

### Add / remove Class (jQuery)

(siehe Slides)



### on click (jQuery)

Mit javascript kann auf sogenannte Events (Ereignisse) gehört und reagiert werden. Es gibt verschiedenste Events: Wenn etwas geklickt wird `click`, wenn sich die Maus bewegt, wenn sich ein inputfeld verändert, etc. Um interaktive Webseiten zu erstellen reagiert man auf diese Events.

Events sind an HTML Element gebunden, deshalb muss man erstmal ein Element selektieren `$('#clickme')`. Mit `.on()` hört und reagiert man auf Events. `.on()` besteht aus zwei Teilen: 1. Muss man angeben auf welches Event man hören möchte, 2. Muss man schreiben wass passieren soll wenn das Event eintritt `.on(event, function() { /* do something*/ })`.


Beispiel:

```
$('#clickme').on('click', function() {
  $('#welcome').text("Welcome!");
});
```

https://api.jquery.com/on/













