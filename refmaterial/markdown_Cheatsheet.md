# Markdown Cheat-Sheet

Kurzreferenz für wichtige Auszeichungsmöglichkeiten in Markdown. 

##### Inhaltsverzeichnis  
[Überschriften](#headers)  
[Hervorhebung](#emphasis)  
[Zeilenumbrüche](#lines)  
[Listen](#lists)  
[Links](#links)  
[Bilder](#images)  
[Code-Beispiele](#code)  
[Tabellen](#tables)  
[HTML-Elemente](#html)  
[Linien](#hr)  

<a name="headers"/>

## Überschriften

```no-highlight
# H1
## H2
### H3
#### H4
##### H5
###### H6
```

# H1
## H2
### H3
#### H4
##### H5
###### H6
------

<a name="emphasis"/>

## Hervorhebungen

```no-highlight
*Dieser Text erscheint kursiv.*
_Dieser auch._

**Dieser Satz ist voll fett**.
__Aber dieser auch__.

**Man kann auch _kombinieren_**.

```
Ergebnis: 

*Dieser Text erscheint kursiv.*
_Dieser auch._

**Dieser Satz ist voll fett**.
__Aber dieser auch__.

**Man kann auch _kombinieren_**.


<a name="lines"/>

## Zeilenumbrüche

Zeilenumbrüche sind eigentlich ganz einfach, aber manchmal braucht man eine Leerzeile mehr, als man denkt. Im Zweifelsfall einfach ausprobieren.


```
Fangen wir mit einer einfachen Zeile an.

Um einen neuen Absatz zu erzeugen, fügen Sie zwischen den Sätzen eine leere Zeile ein.

Anders in diesem Beispiel.
Dieser Satz beginnt im selben Absatz wie sein Vorgänger.
```
Ergebnis:

Fangen wir mit einer einfachen Zeile an.

Um einen neuen Absatz zu erzeugen, fügen Sie zwischen den Sätzen eine leere Zeile ein.

Anders in diesem Beispiel.
Dieser Satz beginnt im selben Absatz wie sein Vorgänger.

<a name="lists"/>

## Listen

### Ungeordnete Liste
Einrückungen werden durch Leerzeichen erzeugt:

```
* Eintrag 1
* Eintrag 2
  * Eingerückt 2a
  * Eingerückt 2b
    * Eingerückt 2aa
```
Ergebnis:
* Eintrag 1
* Eintrag 2
  * Eingerückt 2a
  * Eingerückt 2b
    * Eingerückt 2aa
  
  Hinweis: Es müssen immer so viele Leerzeichen sein, bis das Aufzählungszeichen unter dem ersten Wort der Ebene darüber steht. 

Anstelle von Sternchen geht auch was anderes: 

```
* Sternchen
- Minuszeichen
+ Pluszeichen
```

Ergebnis: 
* Sternchen

- Minuszeichen

+ Pluszeichen

### Geordnete Listen

Die Zahl als solche spielt keine Rolle, sofern es sich um eine Zahl handelt:
```
2. Eintrag 1
0. Eintrag 2
   1. Eingerückt 2a
   7. Eingerückt 2b
```
Ergebnis:

2. Eintrag 1
0. Eintrag 2
   1. Eingerückt 2a
   7. Eingerückt 2b

### Kombiniert geht natürlich auch
```
1. Erster Aufzählungspunkt. 
   * Ungeordnete eingerückte Liste.
   * Zweiter Listeneintrag.
     1. Und noch ne Ebene.
     1. Reicht langsam.
```
Ergebnis:

1. Erster Aufzählungspunkt. 
   * Ungeordnete eingerückte Liste.
   * Zweiter Listeneintrag.
     1. Und noch ne Ebene.
     1. Reicht langsam.



<a name="links"/>

## Links

Für das Erzeugen von Links gibt es viele Möglichkeiten, hier die einfachsten.

```no-highlight
[Link zu Tagungsseite](http://tagungen.tekom.de/h17/tekom-jahrestagung-2017/)
```
ACHTUNG: im Link nicht das http:// vergessen.

```
URLs ohne alles werden automatisch zu Links: www.tagungen.tekom.de

[Link mit relativem Pfad zu anderer Datei: [Startseite](../index.md)
```

Ergebnis:

[Link zu Tagungsseite](http://tagungen.tekom.de/h17/tekom-jahrestagung-2017/)

URLs ohne alles werden automatisch zu Links: www.tagungen.tekom.de

Link mit relativem Pfad zu anderer Datei: [Startseite](../index.md)

<a name="images"/>

## Bilder

```no-highlight
![tekom Logo](http://tagungen.tekom.de/fileadmin/templates/doctima/images/tekom_deutschland.png)
```

Bilder funktionieren so ähnlich wie Links:

![tekom Logo](http://tagungen.tekom.de/fileadmin/templates/doctima/images/tekom_deutschland.png)


<a name="code"/>

## Codebeispiele

Dieses Cheat-Sheet verwendet viele Beispiele, die den Quelltext der Markdown-Datei zeigen. Damit diese Beispiele nicht formatiert darsgestellt werden, kann man sie mit \`Akzentzeichen\` umklammern. So sieht es dann aus: `Akzentzeichen`.

\`\`\`
    Für ganze Abschnitte benötigen Sie sogar 3 Akzentzeichen (davor und danach).
\`\`\`
 

```
        Das Ergebnis sieht dann so aus.
```


Außerdem können Sie `<code>`Tags verwenden`</code>`. 


<a name="tables"/>

## Tabellen

Markdown an sich unterstützt keine Tabellen, aber in vielen Markdown-Ausprägungen (Flavors) können Sie mit Pipe-Zeichen oder evtl. HTML-Tabellen arbeiten. Mit Doppelpunkten geben Sie ganz einfach die Spaltenausrichtung an.

```no-highlight

| Tabellen    | Sind           | Toll  |
| ------------- |:-------------:| -----:|
| Spalte 3 ist| rechts  | ausrichtet|
| Spalte 2 | dagegen |   zentriert |

```
Ergebnis:

| Tabellen    | Sind           | Toll  |
| ------------- |:-------------:| -----:|
| Spalte 3 ist| rechts  | ausrichtet|
| Spalte 2 | dagegen |   zentriert |




<a name="blockquotes"/>


## HTML-Elemente

An vielen Stellen funktionieren auch HTML-Elemente in Markdown. 

```no-highlight
<dl>
  <dt>Definition list</dt>
  <dd>Dieser Listentyp wird gern verwendet.</dd>

  <dt>Ist fast wie XML</dt>
  <dd>Aber dann können Sie ja auch gleich <em>XML</em> schreiben.</dd>
</dl>
```
Ergebnis:

<dl>
  <dt>Definition list</dt>
  <dd>Dieser Listentyp wird gern verwendet.</dd>

  <dt>Ist fast wie XML</dt>
  <dd>Aber dann können Sie ja auch gleich <em>XML</em> schreiben.</dd>
</dl>

<a name="hr"/>

## Linien

```
Drei oder mehr ist die magische Zahl für Linien...

---

Es geht mit Bindestrichen

***

...Sternchen

___

...oder Unterstrichen
```

Ergebnis:

---

Es geht mit Bindestrichen

***

...Sternchen

___

...oder Unterstrichen

<a name="lines"/>



---
Weiterführende Informationen:
- https://guides.github.com/features/mastering-markdown/
- http://github.github.com/github-flavored-markdown/
- https://help.github.com/articles/basic-writing-and-formatting-syntax/
