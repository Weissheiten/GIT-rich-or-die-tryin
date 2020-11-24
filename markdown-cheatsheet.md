

# Markdown Cheatsheet

> Team Bluecode

Markdown ist ein Superset von HTML, das heißt jeder HTML-Tag kann auch in Markdown verwendet werden. Markdown Syntax erleichtert aber lesbare Textdateien zu schreiben (z.B. `Readme` oder `Changelog` Dateien). 

Eine Markdown-Datei erstellen: 

```
datei.md
```



### Header

```html
# <h1> Header
## <h2> Header
### <h3> Header
#### <h4> Header
##### <h5> Header
###### <h6> Header
```

Alternativ: 

```html
<h1> Header
===========

<h2> Header
-----------
```

---

### Text styles

```
*kursiver Text*
_auch kursiver Text_

**fetter Text**
__auch fetter Text__

***kursiver und fetter Text***
**_auch kursiver und fetter Text_**
*__sogar das ist kursiver und fetter Text__*
```

Außerdem in Github Flavoured Markdown:

```
~~durchgestrichener Text~~
```

##### Escapen von Formattierungszeichen:

```
*Dieser Text wäre kursiv*
\*Dieser Text wäre aber mit Sternchen\*
```



### Paragraphen

#### Absätze

Paragraphen enden mit einer oder mehreren Leerzeilen. 

```
Das ist ein Paragraph. Hier geht der Paragraph weiter. 
Dieser Teil gehört auch noch zum Paragraph. 

Hier beginnt ein neuer Paragraph, gleich nach einer Leerzeile. 



Das ist der dritte Paragraph. 
```

Alternativ können auch `<br>` Tags verwendet werden. 

```html
Erster Paragraph. <br>Zweiter Paragraph.
```

#### Blockquotes

```
> Dies ist ein Zitat. 
> Hier geht das Zitat weiter. 

>> Das ist ein doppelt eingerücktes Zitat. 
```



### Listen

#### Unordered Lists

```
* Eintrag 1
* Eintrag 2
* Eintrag 3

+ Eintrag 1
+ Eintrag 2
+ Eintrag 3

- Eintrag 1
- Eintrag 2
- Eintrag 3
```

Ergeben folgende Form: 

* Eintrag 1
* Eintrag 2
* Eintrag 3

#### Ordered Lists

```
1. Eintrag 1
2. Eintrag 2
3. Eintrag 3
```

und 

```
1. Eintrag 1
1. Eintrag 2
1. Eintrag 3
```

Diese numerieren die Einträge nach ihrer ***Reihenfolge***: 

1. Eintrag 1
2. Eintrag 2
3. Eintrag 3

#### Sublisten

```
1. Eintrag 1
2. Eintrag 2
	- Untereintrag 1
	- Untereintrag 2
3. Eintrag 3
```

Ergibt folgendes:

1. Eintrag 1
2. Eintrag 2
	- Untereintrag 1
	- Untereintrag 2
3. Eintrag 3

#### Checkboxen

```
- [ ] Erster Task
- [ ] Zweiter Task
- [x] Fertiger Task
```

Ergibt HTML-Checkboxen:

- [ ] Erster Task
- [ ] Zweiter Task
- [x] Fertiger Task



### Codeblöcke

Inline Code-Teile: 

```
Das ist eine Zeile und hier wird eine Variable definiert: `let a = "indeed";`
```

Codeblöcke werden mit Einrückungen erstellt: 

```
Das ist normaler Text in einer Zeile.

	// Das ist ein Codeblock
	const numbers = [1, 2, 3];
	numbers.forEach(e => console.log(e));

Hier geht der normale Text weiter.
```

Alternativ in Github Flavoured Markdown (mit Syntax-Highlighting!): 


    Das ist normaler Text in einer Zeile.
    ```javascript
    // Das ist ein Codeblock
    const numbers = [1, 2, 3];
    numbers.forEach(e => console.log(e));
    ```
    Hier geht der normale Text weiter.



### Abschnitte

Horizontal rulers: `<hr>` oder auch

```
***
---
_ _ _
*******************
```



### Links

Normaler Link:

```
[End of the Internet](http://hmpg.net/)
```

Mit Linktitel:

```
[End of the Internet](http://hmpg.net/ "Click here!")
```

Relative Links:

```
[About](/about/)
```

Autolink:

```
<http://hmpg.net/>
```

ist dasselbe wie `[http://hmpg.net/](http://hmpg.net/)`



### Bilder

```
![Alternativtext](http://placekitten.com/200/300 "Bildtitel")
```



### Tabellen

```
| Links         | Mittig     | Rechts          |
| :------------ | :--------: | --------------: |
| Ersters links | mittiges   | Ersters rechts  |
| Zweites links | noch eines | Zweites rechts  |
```

