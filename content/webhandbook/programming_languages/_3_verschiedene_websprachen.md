---
title: 3 Verschiedene Web-Programmiersprachen
description : "Verschiedene Web-Programmiersprachen"
tags: ["javascript", "typescript", "python", "php", "ruby"]
---

#### 3.1 Web-Programmiersprachen

Mittlerweile gibt es eine große Menge an verschiedenen Programmiersprachen. Jede Programmiersprache hat ihre Vorteile und Nachteile gegenüber einer anderen. Doch welche Programmiersprachen eignen sich für die Webentwicklung am besten? Gibt es überhaupt die eine Web-Programmiersprache? 

Mit Web-Programmiersprachen können komplexe logische Anweisungen und Prozesse definiert werden. Jede Programmiersprache hat wie die verschiedenen Sprachfamilien auch ihre Eigenarten. In den folgenden Kapiteln werden die bekanntesten Vertreter der Web-Programmiersprachen kompakt vorgestellt. 

#### 3.1.1 JavaScript

Bekannt ist JavaScript als prototypbasierte Skriptsprache für Webseiten. Jedoch wird diese _lightweight_ Sprache auch in anderen Umgebungen eingesetzt, wie beispielsweise Node.js oder _Apache_. Was bedeutet lightweight im Zusammenhang mit einer Programmiersprache? Lightweight Sprachen sind so designt, dass sie einen kleinen _Memory-Footprint_ besitzen, einfach in verschiedenen Systemen zu implementieren sind und sie eine minimalistische Syntax aufweisen.

JavaScript trägt zwar den Namen der objektorientierten Programmiersprache Java, doch wurden beide Sprachen in den frühen 90er-Jahren unabhängig voneinander entwickelt mit völlig unterschiedlichen Grundkonzepten.

Je nach Bedarf lässt sich in JavaScript objektorientiert, prozedural oder funktional programmieren. Dies ist möglich durch den standardisierten Sprachkern _ECMAScript_. Dieser beschreibt eine dynamisch typisierte, objektorientierte, aber klassenlose Sprache.

__Objektorientierte Programmierung__

Obwohl JavaScript dank seines Sprachkerns objektorientierte Programmierparadigmen beinhaltet, kann es nicht als objektorientierte Programmiersprache angesehen werden. JavaScript unterstützt Grundelemente der Objektorientierung wie beispielsweise Datenkapselung, Polymorphie und Vererbung. Doch das wesentlichste Konzept __Klassen__ bietet sie nicht. Mit ECMAScript 6 (kurz ES6) wurde jedoch das Schlüsselwort _class_ eingeführt, mit dem es möglich ist, nun pseudo Klassen zu definieren. Doch sind diese nichts weiter als Funktionen - anstatt _function_ ist es nun möglich, class zu verwenden.

__Prototyp__

Jedes Objekt in JavaScript verfügt über die Eigenschaft _prototype_. Mit diesem Muster beziehungsweise Bauplan werden Objekte erzeugt. Anders als in objektorientierten und klassenbasierten Sprachen, wo Klassen das Muster für Objekte sind.

Prototypen unterscheiden sich von Klassen dahingehend, dass auf Objekten eines Prototyps beliebige Operationen ausgeführt werden können. Das geht bei Klassen nicht. Ein weiterer Unterschied ist, wenn aus einer Klasse ein Objekt gebildet wird, entsteht eine Instanz. Bei Objekten eines Prototypen referenziert das erzeugte Objekt auf den Prototypen. Auch ist es möglich, das Objekte eines Prototyps nachträglich mit Eigenschaften und Methoden ergänzt werden können. Das geht bei Klassen auch nicht.

__Typisierung__

JavaScript ist ein Vertreter der dynamischen Typisierung. Das bedeutet, dass die Typprüfung erst zur Laufzeit passiert - beispielsweise die Prüfung des Datentyps einer Variable.

__Typsicherheit__

In Sachen Typsicherheit nimmt es JavaScript nicht allzu ernst. In großen Projekten ist JavaScript bezüglich der dynamischen Typsicherheit nicht einfach zu handhaben, da Typen schlichtweg nicht angegeben werden müssen.

__Frontend__

JavaScript zählt wohl mit zu den beliebtesten Programmiersprachen überhaupt und die Sprache unterstützt wohl die meisten Frameworks und Bibliotheken, die es für den Frontend-Bereich gibt. JavaScript ist überaus beliebt und dynamisch und unterstützt unter anderem folgende Frontend-Frameworks und Bibliotheken: Angular, React, _Vue.js_, _Ember.js_, _Aurelia_, und noch viele mehr!

__Backend__

Wie beim Frontend, zählt JavaScript auch beim Backend zu den beliebtesten Programmiersprachen überhaupt. JavaScript unterstützt auch im Bereich Backend eine vielzahl von verschiedenen Frameworks und Bibliotheken: Node.js, _Next.js_, _Express.js_, _Meteor_, und mehr.

#### 3.1.2 TypeScript

Einer der häufigsten auftretenden Fehler bei der Programmierung mit JavaScript sind Typfehler. Da Typen bei JavaScript nicht angegeben werden müssen, passiert es häufig, das ein anderer Typ übergeben wird, als erwartet und dadurch zahlreiche Fehler entstehen können. Das Ziel von TypeScript ist ein statischer _Type Checker_ für JavaScript Programme darzustellen. Bevor das Programm ausgeführt wird, wird überprüft, ob die Typen im Programm korrekt sind. Typescript bietet dabei alle JavaScript Funktionalitäten und zusätzlich dazu ein eigenes Typsystem. JavaScript bietet beispielsweise primitive Datentypen wie _string_ oder _number_, überprüft jedoch nicht, ob diese auch konsistent zugewiesen werden. TypeScript tut das.

__Objektorientierte Programmierung__

Die objektorientierte Programmierung mit TypeScript erfolgt nach den gleichen Prinzipien wie in JavaScript. TypeScript unterstützt auch dabei auch JavaScript-”Klassen”. Des Weiteren werden weitere typische Pattern wie die Implementierung von Interfaces, Vererbung und statische Methoden unterstützt.

__Typisierung__

TypeScript ist mit seinem statischen Typsystem ein Vertreter der statischen Typisierung. Die Verwendung dieses ist jedoch optional, weshalb auch das Schreiben von dynamisch typisierten Code möglich ist.

__Typsicherheit__

TypeScript verbessert die Typsicherheit von JavaScript-Programmen, beispielsweise dadurch, das nun Typen angegeben werden müssen. Allerdings ist auch die Typsicherheit von TypeScript noch ausbaufähig, weshalb im Jahr 2014 das Projekt: __Safer TypeScript__ von _Microsoft Research_ entwickelt und im Juli desselben Jahres veröffentlicht wurde. Hierbei soll die Typsicherheit durch eine Kombination von statischer und dynamischer Überprüfungen gewährleistet werden.

__Frontend__

TypeScript ist mittlerweile eine überaus beliebte Programmiersprache im Bereich Frontend-Entwicklung. Laut einem Bericht von __State of Frontend__ aus dem Jahr 2020, haben 94% der befragten Frontend-Entwickler angegeben, dass sie am liebsten mit TypeScript entwickeln. Weitere Ergebnisse des Berichts sind auf der entsprechenden Webseite nachzulesen: https://tsh.io/state-of-frontend/

__Backend__

Seit Node.js es ermöglicht auch mit JavaScript im Backend-Bereich zu entwickeln, gewinnt auch TypeScript an Beliebtheit bei der Backend-Entwicklung. Besonders dadurch, das TypeScript sowohl im Backend als auch im Frontend verwendet werden kann, sorgt dies für eine positive Entwicklererfahrung, da nun nicht mehr zwischen verschiedenen Programmiersprachen gewechselt werden muss.

#### 3.1.3 Python

Python ist eine zu interpretierende und interaktive Programmiersprache. Ein Ziel der Programmiersprache Python ist eine sehr einfache und übersichtliche Syntax. Wodurch auch Nicht-Programmierern der Einstieg in die Sprache leicht fallen soll. Python verfügt unter anderem über Module, Klassen, _Exceptions_ und _High-Level_ dynamische Datentypen.

__Objektorientierte Programmierung__

Python ist eine höhere und objektorientierte Programmiersprache. Mit dem Schlüsselwort class können Klassen definiert werden, welche Attribute und Methoden beinhalten.

__Typisierung__

Python ist Vertreter der dynamischen Typisierung.

__Typsicherheit__

Seit Version 3.6 sind Typangaben für Variablen bei Python möglich. Vorher erfuhr Python die Typen erst zur Laufzeit und Variablen mussten nicht einem speziellen Typen zugewiesen werden. Die sogenannten __Type Hints__ in Python 3.6 fügen Variablen oder anderen Programmobjekten Typinformationen hinzu. So kann nun auch der Rückgabewert einer Funktion vordefiniert werden. Durch die dynamische Typisierung und den Type Hints bietet Python eine hohe Typsicherheit.

__Frontend__

Es ist möglich, Python im Frontend zu nutzen. Dies wird jedoch nicht gängige Praxis, da meist JavaScript, sowie ihre Bibliotheken benötigt werden. Außerdem muss Python-Code vorher geparst und ausgeführt werden.

__Backend__

Als Backend-Programmiersprache ist Python im Vergleich zum Frontend wesentlich beliebter. Einer der Gründe dafür ist die einfache Lesbarkeit von Python. Des Weiteren unterstützen zahlreiche Web-Frameworks mittlerweile Python, dazu zählen beispielsweise Django oder Flask.

#### 3.1.4 PHP

Ist die Rede von Web-Programmiersprachen, so spielt die Skriptsprache PHP eine überaus große Rolle. PHP ist die mit Abstand am häufigsten serverseitig verwendete Programmiersprache zur Erstellung von Webseiten. Die Syntax von PHP ist angelehnt an den Programmiersprachen _C_ und _Perl_. Anders als beispielsweise bei JavaScript, ist PHP eine serverseitig interpretierte Skriptsprache, mit der es möglich ist, Webseiten dynamisch zu erzeugen, sowie Daten aus Benutzereingaben und Datenbanken zu verarbeiten.

Bei serverseitigem Code wird der Quelltext nicht direkt an den Webbrowser übermittelt, sondern an einen Interpreter auf dem Webserver. Der PHP-Interpreter schickt die Ausgabe an den Browser - ein HTML-Dokument.

__Warum PHP und nicht rein HTML?__

HTML oder HTML-Dateien sind rein statisch. Zum Beispiel: Bei der Erstellung einer Tabelle mit einer bestimmten Anzahl an Einträgen kann nur diese bestimmte Anzahl angezeigt werden. Mit PHP ist das flexibel beziehungsweise dynamisch möglich. Theoretisch alles, was auf einer Webseite dynamisch angezeigt werden soll, ist mit PHP möglich - beispielsweise ein Besuchercounter oder Einträge in einem Gästebuch.

__Objektorientierte Programmierung__

In PHP ist die objektorientierte Programmierung möglich. Dadurch wird PHP-Code leichter wartbar und ist einfacher wiederverwendbar. 

__Typisierung__

Wie bei vielen anderen Skriptsprachen auch, ist PHP ein Vertreter der dynamischen Typisierung beziehungsweise PHP ist schwach typisiert. Das bedeutet, dass die Typprüfung erst zur Laufzeit passiert - beispielsweise die Prüfung des Datentyps einer Variable.

__Typsicherheit__

PHP ist eine schwach typisierte Programmiersprache und somit ist es nicht möglich, typsicher zu deklarieren. Jedoch gibt es bei PHP das __Type Hinting__ mit dem es Funktionen ermöglicht, spezifische Parameter zu erzwingen.

Frontend und Backend
PHP unterstützt unter anderem folgende Frameworks: Symfony, _Laravel_, _CodeIgniter_, _CakePHP_ oder _Phalcon_.

#### 3.1.5 Ruby

Ruby ist eine dynamische Programmiersprache, sie sich produktiv einsetzen lässt. Sie zeichnet sich aus durch eine elegante und leicht zu lesende und schreibende Syntax. Ruby ist eine objektorientierte Programmiersprache, unterstützt aber weitere Programmierparadigmen, wie prozedurale und funktionale Programmierung. Die wohl größte Verbreitung findet Ruby im Einsatz als Webserver-Skriptsprache. 

__Objektorientierte Programmierung__

Ruby ist von Grund auf objektorientiert, was bedeutet, dass in Ruby ausnahmslos jeder Wert ein Objekt und jede Funktion eine Methode ist. Selbst Klassen sind Objekte. Die Objekte in Ruby sind dynamisch, was bedeutet, dass es auch möglich ist, prototypenbasiert zu programmieren. Damit können Objekte eigene Methoden haben.

__Typisierung__

Ruby ist Vertreter der dynamischen Typisierung und ist somit schwach typisiert.

__Typsicherheit__

Wie bei anderen Vertretern der dynamischen Typisierung auch ist es bei Ruby nicht möglich, typsicher zu deklarieren.

__Frontend__

Ruby wird teilweise auch für den Frontend-Bereich eingesetzt. Dennoch wird Ruby mehr als Backend-Programmiersprache gesehen als Frontend. Um Ruby im Frontend einzusetzen, muss Ruby-Quellcode in JavaScript-Code umgewandelt werden. Mit _Ruby2JS_, einer Ruby Erweiterung können Entwickler in Ruby-Code schreiben und den Code dann in JavaScript-Code umwandeln lassen. 

__Backend__

Ruby ist eine überaus beliebte Programmiersprache für den Backend-Bereich. Das wohl bekannteste Backend-Framework für Ruby ist Ruby on Rails. Das beliebteste Feature von _Ruby on Rails_ ist die Model-View-Controller-Architektur (kurz _MVC_). Dadurch ermöglicht das Framework, alle Code-Vorgänge separat durchzuführen. Neben Ruby on Rails gibt es noch weitere Backend-Frameworks wie: _Sinatra_, _Roda_ oder auch _Camping_.