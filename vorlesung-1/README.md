Vorlesung 1
===========

Zeitraum: 21. März, 13:00 - 15:15

Ort: FH Joanneum, G.AP152.108

Folien: [scripting-und-coding_1_folien.pdf](scripting-und-coding_1_folien.pdf)


Dokumente und verlinkte Seiten
------------------------------

 - [drawingdata.net](https://drawingdata.net/) von [@drawingdata](https://twitter.com/drawingdata) ([GitHub](https://www.github.com/ginseng666))
 - BPW16-vis: [ORF Artikel](http://steiermark.orf.at/news/stories/2813211), [Visualisierungen](https://petertheone.github.io/bpw16-vis/) und [Code](https://github.com/PeterTheOne/bpw16-vis)
 - Neuwal Barometer: [Aktuelle Version](https://neuwal.com/barometer/profile.php?b=11&p=1), [Alte Version](https://neuwal.github.io/barometer/) mit [Code](https://github.com/neuwal/barometer)
 - [Feinstaub-Graz](http://feinstaub-graz.at/): [Code](https://github.com/PPOE/feinstaub-meter).
 - [Mehrheiten-Rechner](http://mehrheiten-rechner.at/): [Code](https://github.com/PeterTheOne/mehrheiten-rechner)
 - [CodePen: HTML Elemente](https://codepen.io/PeterTheOne/pen/oqZbPg)
 - [CodePen: CSS Deklarationen](https://codepen.io/PeterTheOne/pen/xWqYog)
 - [CodePen: CSS Selektoren](https://codepen.io/PeterTheOne/pen/ZxeOzQ)
 - [CodePen: CSS Selektoren 2](https://codepen.io/PeterTheOne/pen/JLWXJX)
 - [https://developer.mozilla.org](https://developer.mozilla.org)
 - [WS15/16 - MTD114 Hypermedia 1 - Teil 2: HTML-Grundlagen](https://www.youtube.com/watch?v=m9VmKANwHO8)
 - [http://www.htmlandcssbook.com/](http://www.htmlandcssbook.com/)
 - [Tastaturkürzel](Tastaturkuerzel.md)


Inhalt
------

### HTML

HTML Elemente beschreiben/notieren den Inhalt einer HTML Seite von der Bedeutung her (Semantisch). Nicht von der 
darstellung her, dafür verwendet man CSS.

#### HTML Elemente

Die Elemente bestehen aus den Klammern `<` und `>` und der Elementbezeichnung. Es gibt Elemente die sich öffen und 
schließen `<p></p>` und andere die sich selbst schließen `<br />`. Der Schrägstrich `/` zeigt den schluss eines Elements.

Zwischen einem öffnenden und schließenden Element kann Text stehen oder weitere HTML Elemente. Durch verschachteln von 
Elementen ergibt sich eine Baumstruktur auch [DOM](https://de.wikipedia.org/wiki/Document_Object_Model) genannt. 
Übergeordnete Element werden parent bzw. Eltern genannt und untergeordnete Elemente child bzw. Kind. (Nicht jedes
Element darf jedes andere Element enthalten.)

Beispiele: https://codepen.io/PeterTheOne/pen/oqZbPg

Elemente die wir uns angeschaut haben:

 - [`<p>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/p): Paragraph
 - [`<h1>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/h1) bis `<h6>`: Überschriften
 - [`<div>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/div): Division Element bzw. generischer Container
 - [`<br />`](https://developer.mozilla.org/de/docs/Web/HTML/Element/br): Zeilenumbruch
 - [`<header>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/header): repräsentiert eine Gruppe von Einführungs- oder Navigationshilfen
 - [`<footer>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/footer): Fußzeile
 - [`<img />`](https://developer.mozilla.org/de/docs/Web/HTML/Element/img): Bild Attribute: `src=""`, `alt=""`, etc.
 - [`<blockquote>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/blockquote): Zitateblock
 - [`<ul>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/ul): Ungeordnete Liste
 - [`<ol>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/ol): Geordnete Liste
 - [`<li>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/li): Listenelement als Kind (child) von `<ul>` oder `<ol>`
 - [`<a>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/a): Anchor element bzw. Link. Attribute: `href=""`, etc.
 - [`<em>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/em): Emphasis bzw. Betonung. ()Meist kursiv dargestellt.)
 - [`<strong>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/strong): Strong Importance bzw. starke Betonung. (Meist fett dargestellt.)
 - [`<table>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/table): Tabelle
 - [`<tr>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/tr): Tabellenzeile
 - [`<th>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/th): Tabellenkopf Element
 - [`<td>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/td): Tabellendaten Element
 - [`<form>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/form): Formular
 - [`<input>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/input): Eingeabe Feld
 - [`<button>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/button): klickbarer Knopf
 
Viele weitere Elemente:

https://developer.mozilla.org/en-US/docs/Web/HTML/Element
https://developer.mozilla.org/de/docs/Web/HTML/Element


#### HTML Attribute

HTML Elemente können Attribute enthalten, Werte die diese Elemente konfigurieren oder ihr Verhalten anpassen.

Attribute werden innerhalb der Klammern `<>` und nach der Elementbezeichnung des öffnenden Elements geschrieben `<a href=""> ... </a>`. 
Das Attribut besteht aus der Attributbezeichnung, gefolgt von einem Istgleich `=` und Anführungszeichen `""`, zwischen 
den Anführungszeichen steht der AttributWert (value) `href="https://www.fh-joanneum.at"`.

Globale Attribute können mit jedem HTML Element verwendet werden, andere Attribute nur mit spezifischen Elementen.

Attribute die wir uns angeschaut haben:

 - [`title=""`](https://developer.mozilla.org/de/docs/Web/HTML/Globale_Attribute/title) (Global): Text über das Element. Wird meist als Tooltip angezeigt.
 - [`id=""`](https://developer.mozilla.org/de/docs/Web/HTML/Globale_Attribute/id) (Global): Eindeutige Bezeichnung. Gleiche bezeichnung darf es nur ein Mal geben.
 - [`class=""`](https://developer.mozilla.org/de/docs/Web/HTML/Globale_Attribute/class) (Global): Ein oder mehrere Klassen, erlaubt das selektieren über CSS.
 - [`href=""`](https://developer.mozilla.org/de/docs/Web/HTML/Element/a#attr-href) (`<a>`, etc.): URL einer verlinkten ressource.
 - [`src=""`](https://developer.mozilla.org/de/docs/Web/HTML/Element/img#attr-src) (`<img>`, etc.): URL von einem eingebetteten Inhalt.
 - [`alt=""`](https://developer.mozilla.org/de/docs/Web/HTML/Element/img#attr-alt) (`<img>`, etc.): Alternativer Text falls ein Bild nicht angezeigt werden kann.

Weitere Attribute:

https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes
https://developer.mozilla.org/de/docs/Web/HTML/Attributes


#### HTML Grundgerüst

Dateiendung `.html`.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>SuC: HTML Wiederholung</title>
  </head>
  <body>
    <h1>HTML Wiederholung</h1>
    
  </body>
</html>
```

 - [`<!DOCTYPE html>`](https://developer.mozilla.org/en-US/docs/Glossary/Doctype): Gibt an dass es ein HTML document ist.
 - [`<html>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/html): Ist das erste Element
 - [`<head>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/head): HTML Dokument Kopf, enthält Dokumenttitel und Metainformationen.
 - [`<body>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/body): Inhalt des HTML Dokuments.
 - [`<meta charset="utf-8">`](https://developer.mozilla.org/de/docs/Web/HTML/Element/meta#attr-charset): setzt den Zeichensatz auf utf-8
 - [`<title>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/title): Dokumenttitel: Ist der Seitentitel der oben im Browserfenstern und Browsertab steht.


### CSS

CSS ist, im gegensatz zu HTML, für das aussehen von einem HTML Dokument zuständig.

CSS besteht aus Regelsätzen (auch Regeln). Die Grundbausteine von diesen Regeln sind Selektoren und Deklarationen. Eine 
Regeln beginnt mit einem Selektor, gefolgt von Klammern `{}` in denen eine oder mehrere Deklarationen stehen können.

```
  h1 {
    color: blue;
  }
```


#### CSS Deklarationen

Eine CSS Deklaration setzt den Wert einer CSS Style Eigenschaft. Zuerst steht die Bezeichnung der CSS Style Eigenschaft, 
gefolgt von einem Doppelpunkt `:` und dem Wert der Eigenschaft. Zum Beispiel `color: red;` setzt die Schriftfarbe Rot.

Deklarationen die wir uns angeschaut haben:

 - `background-color`: Hintergrundfarbe
 - `color`: Schriftfarbe
 - [`font-family`](https://developer.mozilla.org/de/docs/Web/CSS/font-family): Schriftfamilie
 - `font-size`: Schriftgröße
 - `margin`: Außenabstand aller vier Seiten eines Elements
 - `padding`: Innenabstand aller vier Seiten eines Elements.

Weitere:

https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Properties_Reference


#### CSS Selektoren

CSS Deklarationen können auf HTML Elemente angewandt werden. Mit einem Selektor wird festgelegt welche HTML Elemente 
eine Deklaration betreffen soll.

Arten nach denen Selektiert werden kann:

 - nach HTML Element: `h1 { ... }`, `p { ... }`, etc.
 - mit `#` nach id: `#hierStehtEineId { ... }`, `#element-1 { ... }`, etc.
 - mit `.` nach class: `.hierStehtEineClass { ... }`, `.roundCorner { ... }`, etc.
 - mit `:` nach pseudo-class: `:pseudoClass { ... }`, `:last-child { ... }`, etc.

Weiters lassen sich auch mehrere Selektoren mit `,` an einander reihen und Selektoren mit einem Leerzeichen ` ` 
verschachteln um Kindelemente von Elementen zu selektieren.

https://codepen.io/PeterTheOne/pen/ZxeOzQ
















