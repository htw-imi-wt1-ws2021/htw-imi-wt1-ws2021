---
title: MyStuff
weight: 2
tags: ["projekt1", "MyStuff"]
pre: "<b>1. </b>"
---

Das Projekt "MyStuff" ist eine Web-Applikation, gerichtet an Student:innen. Vorbei ist die Zeit wo man als Student verschiedene Programme im Blick haben musste, um sich selbst zu organisieren und um keine Frist(en) zu verpassen. MyStuff ist ein zentraler Platz für das Studium bzw. für die Module eines gewählten Studiengangs, wo wichtige Dokumente, Termine und Quellen eigenständig zusammengetragen werden.


#### 1.1 Teammitglieder

**Jördis Liermann - 0576959**

**Nguyen Xuan Bach Do - 0556341**

**Alain Ngoufack Nguefack - 0557214**

**Dominic Engel - 0576863**


#### 1.2 Technologien

Für die Entwicklungsphase hat sich das Team auf die folgenden Technologien geeinigt:
- Für das Backend wird die Node.JS Umgebung verwendet. Dazu wird das Framework Express.JS genutzt, um eine REST-API zu bauen.
- Für die Entwicklung des Frontends wird das Framework React.JS verwendet, da der Großteil des Teams bereits Erfahrung mit diesem Framework hat. Dadurch können zeitaufwendige Schritte bei der Einarbeitung eingespart werden.
- Das Team hat sich für eine No-SQL-Datenbank entschieden, um Daten für die Webanwendung zu speichern.

Neben den vier fundamentalen Operationen persistenter Datenbankanwendung, auch bekannt unter dem Akronym CRUD, wird unsere Web-Applikation eine Art Tag-Management bieten, unter dem es möglich sein wird, eigene Tags zu erstellen. 


#### 1.3 Ziele

Die Applikation ermöglicht es Student:innen Module hinzuzufügen und zu bearbeiten, um so das Studium selbst zu organisieren. Zum einen können innerhalb eines Moduls wichtige Vorlesungsfolien mit Informationen versehen, hochgeladen und wieder gelöscht werden. Auch ist es möglich, sich selbst ToDos zu erstellen. Diese können dann eigenständig mit Informationen versehen und terminiert werden. Ist ein Todo fertig bearbeitet oder der Termin abgelaufen, kann es auch wieder gelöscht werden. Wichtige Quellen oder Referenzen wie Links zu Webseiten können ebenfalls hinzugefügt und wieder gelöscht werden. Das Spannende hierbei ist, dass der Benutzer beim Hinzufügen von externen Quellen diese automatisch mit einem Tag versehen werden. Anschließend kann der Benutzer dann nach Tags filtern und bekommt eine Liste von Quellen zu einem bestimmten Tag. Die hochgeladenen Daten werden dabei global in einer Datenbank gespeichert und sind jederzeit abrufbar.


#### 1.4 Herausforderungen

In unserer Web-Applikation MyStuff wird es möglich sein, Links zu externen Webseiten zu speichern - ähnlich wie das Speichern von Lesezeichen bei Google Chrome oder Mozilla Firefox. Doch strebt das Team danach, diese externen Quellen mit Tags automatisch zu kategorisieren! Der Benutzer hat die Möglichkeit neue Tags zu erstellen. Unter einem Tag beschreibt der Benutzer weitere Schlagwörter, die diesen Tag definieren sollen. 

__Zum Beispiel:__

Unter __#programming__ könnten sich folgende Schlagwörter befinden:
- variables
- data types
- loop
- class
- interface

Das spannende daran ist, dass der Benutzer die selbst erstellten Tags nach Belieben definieren kann. Ein Benutzer mit weit mehr Erfahrungen in der Softwareentwicklung würde eventuell nach anderen Schlagwörtern filtern wollen als ein Anfänger. Speichert ein Benutzer nun einen Link zu einer Webseite, durchsucht ein Algorithmus
den HTML-Body der Webseite nach diesen Schlagwörtern. Werden diese gefunden und es werden bspw. (Schlagwörter > 15) gefunden, kategorisiert der Algorithmus den Link zu einem der definierten Tags.

Bei MyStuff kann der Benutzer dann nach Tags filtern und bekommt eine Liste der externen Quellen zu einem bestimmten Tag. Der Benutzer kann so bspw. bei einer Recherche zu verschiedenen Themen schnell Links speichern und abrufen.


#### 1.5 Link zum Projekt

Das Projekt sowie der Sourcecode sind unter folgendem Link zu finden:

[MyStuff Webapplikation](http://localhost:8080)


#### 1.6 Entwurf

Vor der Umsetzung des Projektes wird zunächst eine Liste mit den Features erstellt. Hierfür wurde bei MyStuff eine sogenannte User Story Map verwendet. Dabei werden zunächst verschiedene Aktivitäten (grüne Post-Its) festgelegt, welche eine Art Kategorie bilden. Anschließend werden dieser Aktivität weitere Teilschritte zugeordnet (gelbe Post-Its). Beispielsweise gehören zu der Aktivität: Module bearbeiten, die Unterpunkte Modul erstellen, Modul löschen, Module sortieren (z. B. nach Semester) und Module priorisieren.


![Unser Screenshot](/images/1_team_mystuff/hello.jpg?width=40pc)

#### 1.8 Link zum Sourcecode

[Code](http://localhost:8080)

