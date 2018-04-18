Vorlesung 2
===========

Zeitraum: 22. März, 14:00 - 16:15

Ort: FH Joanneum, G.AP152.108

Folien: [scripting-und-coding_2_folien.pdf](scripting-und-coding_2_folien.pdf)


Dokumente und verlinkte Seiten
------------------------------

 - [MDN: SVG](https://developer.mozilla.org/kab/docs/Web/SVG)
 - [W3C Recommendation: SVG](https://www.w3.org/TR/SVG11/)
 - [Working with SVG — A Primer](https://slides.com/sarasoueidan/working-with-svg-a-primer#/) Folien von [Sara Soueidan](https://www.sarasoueidan.com/) ([@SaraSoueidan](https://twitter.com/sarasoueidan))
 - [Understanding SVG Coordinate Systems and Transformations](https://www.sarasoueidan.com/blog/svg-coordinate-systems/)
 - [CodePen: SVG Elemente](https://codepen.io/PeterTheOne/pen/QmvBbo)
 - [CodePen: SVG Haus](https://codepen.io/PeterTheOne/pen/YaVjVe)
 - [CodePen: SVG Beispiel selbst](https://codepen.io/PeterTheOne/pen/XERBzj)
 

Inhalt
------

### Bildformate

#### Rastergrafiken vs. Vektorgrafiken

Rastergrafiken sind nach einem Bildraster in einer fixen größe aufgebaut, jeder Pixel wird einzeln festgelegt. Vor allem geeignet für Fotos (Abtastung durch einen Bildsensor).

Beispiele: JPEG, BMP, PNG, GIF, ICO, TIF, PSD

Vektorgrafiken bestehen aus grafischen Elementen wie Linien, Kreisen, Rechtecken etc. Und können deshalb skaliert (vergrößert/verkleinert) werden ohne verluste bei der Bildqualität. Vor allem geeignet für Logos und Grafiken die digital erstellt worden sind. Dabei ist die Dateigröße meist auch kleiner. Die genaue darstellung auf einem Bildschirm wird immer erst beim anzeigen einer vektorgrafik berechnet.

Beispiele: SVG, EPS, AI


### SVG

#### Grundaufbaue

```
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN" "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<svg version="1.1" baseProfile="full" xmlns="http://www.w3.org/2000/svg" 
    preserveAspectRatio="xMidYMid meet" viewBox="0 0 300 300">

  <title>Title goes here</title>

  <!-- SVG Elements go here -->
</svg>

```

#### Koordinatensystem

Die y-Achse (Vertical, von oben nach unten) ist gespielt, der nullpunkt ist oben und positive Werte gehen nach unten.


#### Elemente

- [`<title>`](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/title): Name der Grafik.
- [`<desc>`](https://developer.mozilla.org/en-US/docs/Web/SVG/Element/desc): Beschreibung der Grafik.
- [`<rect x="" y="" width="" height="">`](https://developer.mozilla.org/de/docs/Web/SVG/Element/rect): Rechteck
- [`<line x1="" y1="" x2="" y2="">`](https://developer.mozilla.org/de/docs/Web/SVG/Element/line): Linie
- [`<circle cx="" cy="" r="">`](https://developer.mozilla.org/de/docs/Web/SVG/Element/circle): Kreis
- [`<ellipse cx="" cy="" rx="" ry="">`](https://developer.mozilla.org/de/docs/Web/SVG/Element/ellipse): Ellipse 
- [`<text x="" y="">`](https://developer.mozilla.org/de/docs/Web/SVG/Element/text): Text
- [`<g>`](https://developer.mozilla.org/de/docs/Web/SVG/Element/g): Gruppierungselement
- [`<polygon points="">`](https://developer.mozilla.org/de/docs/Web/SVG/Element/polygon): Geschlossene Form aus Linien.
- [`<polyline points="">`](https://developer.mozilla.org/de/docs/Web/SVG/Element/polyline): Mehrere verbundene Linien.
- [`<path>`](https://developer.mozilla.org/de/docs/Web/SVG/Element/path): Generisches Element für Formen.

Weitere: https://developer.mozilla.org/en-US/docs/Web/SVG/Element

#### Zusätzliche Attribute

- [`fill=""`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/fill): Farbe mit der ein Element gefüllt wird.
- [`stroke=""`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/stroke): Farbe mit der die Linien von einem Element dargestellt werden.
- [`stroke-width=""`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/stroke-width): Breite der Linien.
- [`color=""`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/color): Textfarbe
- [`text-anchor=""`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/text-anchor): Text ausrichtung nach der x,y koordinate.
- [`font-size=""`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/font-size): Schriftgröße
- [`font-family=""`](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/font-family): Schriftfamilie

Weitere: https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute

