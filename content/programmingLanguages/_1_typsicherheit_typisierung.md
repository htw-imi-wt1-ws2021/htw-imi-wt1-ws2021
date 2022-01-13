---
title: 1 Typsicherheit und Typisierung
description : "Typsicherheit und Typisierung"
tags: ["chapter1", "typsicherheit", "typisierung"]
---

#### 1.1 Typsicherheit

Die Typsicherheit sorgt dafür, dass die Code-Qualität gewährleistet wird und sich somit die Zuverlässigkeit des entwickelten Programms erhöht. Es obliegt dem Interpreter beziehungsweise Compiler die Sicherheit durch Typprüfung herzustellen und Typverletzungen aufzufangen. Manche Compiler geben Meldungen aus und in manchen passiert eine automatisierte Typumwandlung, sollte es eine Typverletzung geben. Beispielsweise warnt ein Compiler davor, eine Gleitkommazahl (Float, Double) an eine Ganzzahl-Variable (Integer) zu übergeben. Dennoch müssen bei Zuweisungen die beteiligten Typen nicht notwendigerweise identisch sein, da beispielsweise Ganzzahlen unter Umständen an Gleitkommazahlen-Variablen zugewiesen werden können. Wichtig dabei ist, dass die Datentypen kompatibel zueinander sind.

#### 1.2 Typisierung

Das Ziel der Typisierung ist die Vermeidung von Laufzeitfehlern. Sie dient dazu, dass Objekte wie beispielsweise Variablen oder Funktionen korrekt verwendet werden beziehungsweise sie soll sicherstellen, dass keine Operation ausgeführt werden kann, die syntaktisch oder semantisch fehlerhaft ist. Programmiersprachen, die eine Typisierung aufweisen nennt man entweder _stark typisiert_ oder _schwach typisiert_. Stark typisierte Programmiersprachen sind beispielsweise _C++_ und _Java_, während schwach typisierte Sprachen beispielsweise PHP und JavaScript sind. Bei der Typisierung gibt es Typprüfungen, die entweder zur Kompilierzeit oder Laufzeit vorgenommen werden. Man spricht hier entweder von einer statischen Typprüfung oder dynamischen Typprüfung.

__Statische Typisierung__

Die statische Typisierung gilt als die stark typisierte Typisierung. Bei einer statischen Typprüfung werden beispielsweise Zuweisungsfehler noch vor der Laufzeit erkannt beziehungsweise wird eine Typprüfung bereits zum Zeitpunkt der Kompilierung durchgeführt. Der Nachteil einer statischen Typisierung ist, dass teilweise die Typen erst zur Laufzeit bekannt sind. Des Weiteren ist der Compiler komplexer, da hier ein gewisser Mehraufwand für die Analyse anfällt.  

__Dynamische Typisierung__

Diese Art der Typisierung zeichnet sich durch ein hohes Maß an Flexibilität aus und gilt als die schwach typisierte Typisierung. Doch kann die hohe Flexibilität als Schwachstelle gesehen werden. Denn manche Fehler können mit diesem Schema der Typisierung erst zur Laufzeit erkannt werden - das bedeutet unter Umständen eine erschwerte Fehlersuche. Des Weiteren ist die dynamische Typisierung anfällig für einen nachlässigen Umgang in der Entwicklung. Zusätzlich erlaubt die dynamische Typisierung die korrekte Verarbeitung von eigentlich inkompatiblen Typen.
