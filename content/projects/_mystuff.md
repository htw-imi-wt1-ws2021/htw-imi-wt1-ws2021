---
title: MyStuff
weight: 2
tags: ["projekt1", "MyStuff"]
pre: "<b>1. </b>"
---

#### 1 Abstract

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

Das Projekt ist unter folgendem Link zu finden:

[MyStuff Webapplikation](https://my-stuff-htw.herokuapp.com/)


#### 1.6 Entwurf

Vor der Umsetzung des Projektes wird zunächst eine Liste mit den Features erstellt. Hierfür wurde bei MyStuff eine sogenannte User Story Map verwendet. Dabei werden zunächst verschiedene Aktivitäten (grüne Post-Its) festgelegt, welche eine Art Kategorie bilden. Anschließend werden dieser Aktivität weitere Teilschritte zugeordnet (gelbe Post-Its). Beispielsweise gehören zu der Aktivität: Module bearbeiten, die Unterpunkte Modul erstellen, Modul löschen, Module sortieren (z. B. nach Semester) und Module priorisieren.

![User Story Map](/images/1_team_mystuff/user_story_map.jpg?width=40pc)

Anschließend werden die Aktivitäten nach Zeit sortiert, d.h. je weiter links eine Aktivität steht, desto früher soll diese bei der Entwicklung umgesetzt werden. Die einzelnen Teilschritte der Aktivität werden dabei auch nach ihrer Priorität sortiert - je weiter oben, desto wichtiger ist diese.
Als letzter Schritt wird eine rote Linie durch die User Story Map gezogen, also gelben Post-Its, welche sich oberhalb dieser Linie befinden, müssen in der fertigen Anwendungen vorhanden sein. Die verbleibenden Features werden erst implementiert, wenn alle Features oberhalb der roten Linie fertig sind und noch genügend Ressourcen für eine Weiterentwicklung vorhanden sind.

Nachdem alle Features der Anwendungen definiert wurden, wird als nächster Schritt ein erster Entwurf der Oberfläche der Web-App erstellt.
Für die Erstellung der MyStuff-Mockups wurde das Prototyping-Tool Figma verwendet.

(siehe auch https://www.figma.com/file/fRpANngWEGEqgV2Gkxv8xi/Bach-project?node-id=0%3A1)

Die Abbildung weiter unten zeigt die Startseite, welche der Nutzer angezeigt bekommt, nachdem sich dieser einloggt. Hier befindet sich auf der linken Seite eine Übersicht über alle Module. Daneben befinden sich alle Informationen über das momentan aktive Modul. Diese sind unterteilt in drei Reitern. Eine ToDo-Liste für das Modul, wo der Benutzer Abgaben sowie Termine für das Modul festhalten kann. Um eine Übersicht über die bereits erledigten und ausstehenden ToDos zu haben, können diese in drei verschiedenen Spalten unterteilt werden:

- ToDo - enthält Aufgaben die noch anstehen
- Doing - enthält Aufgaben, die gerade in Bearbeitung sind
- Done - enthält Aufgaben, welche erledigt sind

![Figma Prototyp Übersicht](/images/1_team_mystuff/figma_prototyp_uebersicht.jpg?width=40pc)

Zusätzlich zu der ToDo-Liste ist es bei MyStuff auch möglich, Daten zu jedem Modul hochzuladen, dazu zählen z. B. Vorlesungsfolien, Übungsaufgaben oder Mitschriften.

Neben den Daten zu dem Modul kann der Benutzer auch Links wie beispielsweise Beweise oder Literaturempfehlungen in der MyStuff-App speichern. Diese erhalten bei der Erstellung automatisch Tags (siehe auch 1.3. Herausforderung) passend zu dem Inhalt der Links. Der Benutzer kann Tags zu den Links auch manuell anpassen.
Die Links werden mit Tags versehen, damit der Benutzer diese mit einem Filter sortieren kann um so schneller den richtigen Link zu finden (siehe Abb. 3). 

![Figma Prototyp Links](/images/1_team_mystuff/figma_prototyp_links.jpg?width=40pc)

#### 1.7 Umsetzung
##### 1.7.1 Backend

Wie bereits in Abschnitt 1.2 erwähnt, wird das Backend in Node.JS-Entwicklungsumgebung mit Hilfe des Express.JS-Framework entwickelt. Die NoSql-Datenbank wurde mit Hilfe von MongoDB-Datenbank (https://www.mongodb.com/) auf der Cloud bereitgestellt.

Folgende Abbildung stellt eine Übersicht über die Verzeichnishierarchie des Backends dar:

![Struktur des Backends](/images/1_team_mystuff/struktur.jpg?width=15pc)

Das Backend wird wie folgt aufgeteilt:

- __backend__-Verzeichnis enthält alle Quellcodes des MyStuff-Project, die für die Ausführung des Projekts benötigt werden.
- __node_modules__ enthält Quellcodes der verwendeten Module bzw. Bibliotheken, die in package.js-Datei definiert werden.
- __package.json__ wird benutzt, um installierte Abhängigkeiten (Dependencies) zu überprüfen. Außerdem enthält diese Datei mehrere nützlichen Skripte, die z.B für Start, Build oder Test des Projekts verwendet werden.
- __models__-Verzeichnis enthält alle Datenschema-Schnittstelle der Datenbank. Mit dem Schema werden Felder, die in jedem Dokument sowie deren Validierungsanforderungen und Standardwerte definiert.
- __routes__-Verzeichnis enthält die Kontrolle Komponente des Backends. Alle REST-Anfragen werden hier entsprechend der Klasse gefiltert und verwaltet.
- __app.js__-Datei enthält die Start-Skripte des Backends. Hierzu werden die Express.JS-Framework  als auch mongoose-Modul, das für die Anbindung der MongoDB-Datenbank erforderlich ist, definiert und aufgerufen. Außerdem werden hier die Umleitungen der HTTP-Anfragen zu der entsprechenden Kontrolle-Datei in der routes-Verzeichnis definiert.

Nach der erforderlichen Konfiguration des Backends in der app.js-Datei werden Datenschema im models-Verzeichnis definiert. Insgesamt wurde drei Modellen für drei Instanzen im Projekt umgesetzt: __User__, __Todo__ und __Module__. Folgende Diagramm zeigt die Beziehungen zwischen den Modellen.

![UML Diagramm](/images/1_team_mystuff/uml.jpg?width=30pc)

Nach der Definition der Datenmodellen werden die Route umgesetzt. Im folgenden werden einen Überblick über die erforderlichen Routen, ihre Aufgaben und die HTTP-Methode, die für den Zugriff auf sie verwendet wird.

Services in der Users-Route:
![Services in der Users-Route](/images/1_team_mystuff/users.jpg?width=40pc)


Services in der Modules-Route:
![Services in der Modules-Route](/images/1_team_mystuff/modules.jpg?width=40pc)

Services in der Todos-Route:
![Services in der Todos-Route](/images/1_team_mystuff/todos.jpg?width=40pc)

Die Backend-Implementierung ist unter folgendem Link zu finden:
[Backend-Implementierung](https://github.com/Bachdz/MyStuffBackend)

##### 1.7.2 Frontend

Gemäß Abschnitt 1.2 wird für die Entwicklung der Benutzeroberfläche das Framework React.JS benötigt. Um eine Entwicklungsumgebung mit React zu erstellen, kommt das Tool Create React App in Einsatz. Dieses Tool wird mit NPM (Node Package Manager) von Node.js installiert. 
Als erstes wird wie die Umsetzung des Backends die Aufteilung der Komponente durchgeführt. Dadurch kann die Wiederverwendbarkeit des Codes möglichst maximieren und die Wartung des Projekts einfacher durchführen. 

Folgende Abbildung veranschaulicht die Verzeichnishierarchie des Frontends:

![Struktur des Frontends](/images/1_team_mystuff/frontend.jpg?width=15pc)

- __node_modules__ enthält den Quellcode des React-Frameworks und verwendeten Module bzw. Bibliothek, die in package.json definiert werden.
- __public__ enthält HTML-Dateien und Komponente wie Bilder, die  clientseitig gerendert werden sollen.
- __src__ ist der Ort, wo die Projektentwicklung stattfindet. Es enthält alle Komponente des Projekts, die in Javaskript geschrieben werden. Es beinhaltet Login-Komponente und Komponente vom Mainscreen wie Modules, Todos, Links. Darüber hinaus liegen unter dem css-Verzeichnis die zu den Komponente zugehörigen CSS-Dateien. 
- Die __index.js__-Datei ist der Startpunkt beim Kompilieren der Anwendung, bei dem die App.js-Komponente aufgerufen wird.
- __package.json__ wird für die Definition der installierten Abhängigkeiten verwendet.
- __package-lock.json__ wird anhand der Informationen in package.son automatisch generiert.

Die Art und Weise, wie Komponenten in React miteinander anhängig sind, sind state (Zustand)  und props (Eigenschaft).  Eine Komponente besitzt ihr eigenes Zustand bzw. Instance-Daten. z.B. User-Komponente besitzt Zustand wie username: String. 
Information zwischen Komponenten können mittels props transportiert werden. z.B. Die Mainscreen-Komponente muss z.B. in der Lage sein, die geloggte Information der User-Komponente anzuzeigen. Daher kann die User-Komponente diese Information an die Mainscreen-Komponente weitergeben, die dann in der Mainscreen-Komponente mit Hilfe von  props. zugänglich sein wird.
In der folgenden Abbildung ist eine Übersicht über die Komponente von der Main-Seite und ihre Beziehungen gegeben. Die wichtigen Daten im Zustand jeder Komponente und die props, die von einer Komponente zur anderen übertragen werden, sind ebenfalls abgebildet.

Komponenten des Main-Screens und ihre Beziehungen:
![Komponenten des Main-Screens und ihre Beziehungen](/images/1_team_mystuff/komponente.jpg?width=50pc)

Die komplette Implementation des Frontends ist auf Github zu finden:
[Frontend-Implementierung](https://github.com/Bachdz/MyStuffFrontend)

Im Folgenden sind Bilder von Seiten sehen, die für das Frontend implementiert wurden:

Welcome-Seite:
![Welcome-Seite](/images/1_team_mystuff/welcome.jpg?width=50pc)

Login-Seite:
![Login-Seite](/images/1_team_mystuff/login.jpg?width=50pc)

Main-Seite in Todos-Tab:
![Main-Seite in Todos-Tab](/images/1_team_mystuff/main_todos.jpg?width=50pc)

Main-Seite in Links-Tab:
![Main-Seite in Links-Tab](/images/1_team_mystuff/main_links.jpg?width=50pc)

##### 1.7.3 CI/CD Pipeline & Deployment-Prozess

Die Pipeline wurde mit __Heroku__ eingerichtet. Heroku ist eine Platform-as-a-Service Anbieter, der den ganzen Deployment- und Testprozess für eine Applikation mit wenigen Klicks ermöglicht.
Als Erstes wird ein Konto auf dem Plattform eröffnet. Nach der erfolgreichen Erstellung des Konto wird der Nutzer auf die Dashboard-Seite umgeleitet. Um eine neue App zu deployen, wird auf die Schaltfläche _New → Create new app_ geklickt. 

Erstellung neuer App auf Heroku:
![Erstellung neuer App auf Heroku](/images/1_team_mystuff/ci1.jpg?width=50pc)

Danach muss ein App-Name eingegeben und eine Server-Region ausgewählt werden. Als Erstes wird das Backend-Deployment eingerichtet. In diesem Fall heißt die App my-stuff-backend und Region wird als Europe ausgewählt. Die Erstellung einer neuen App auf Heroku wurde damit durchgeführt. Danach wird man direkt in die Einstellungsseite umgeleitet, wo eine Deployment-Methode ausgewählt werden kann. Der gesamte Code von MyStuff liegt auf GitHub, deshalb wird hier GitHub als Deployment-Methode ausgewählt. Heroku wird sich mit unserem GitHub-Konto verlinken und danach muss eine Repository im Konto ausgewählt werden.

Auswahl der Deployment-Methode mit GitHub:
![Auswahl der Deployment-Methode mit GitHub](/images/1_team_mystuff/ci2.jpg?width=50pc)

Nachdem das Repository erfolgreich mit Heroku verlinkt ist, kann ein Branch ausgewählt werden, um zu deployen. Unser master-Branch wird dabei ausgewählt. Außerdem kann hier die Option _Automatic deploys_ für ein bestimmten Branch ein/ausgeschaltet werden. Dies bedeutet, wenn ein neuer Commit in den Branch kommt, wird die Pipeline das automatisch erkennen und einen neuen Deployment-Prozess durchführen. Falls diese noch Tests erkennen, werden diese ebenfalls durchgeführt. Als letztes wird beim _Manual deploy_-Bereich den gewünschten Branchs ausgewählt und auf die Schaltfläche _Deploy Branch_ geklickt. Damit wird der Prozess gestartet.

Auswahl des Branchs für Deployment-Prozess:
![Auswahl des Branchs für Deployment-Prozess](/images/1_team_mystuff/ci3.jpg?width=50pc)

Um den Prozess richtig auszuführen, muss ein Buildpack hinzugefügt werden. Dies liegt im Tab _Settings_.
Fürs Backend haben wir das Paket heroku/nodejs verwendet. Fürs Frontend haben wir das create-react-app-buildpack aus GitHub genommen. Dieses Paket liegt unter https://github.com/mars/create-react-app-buildpack.git

Folgende Abbildungen geben einen Überblick für den Build-Status des Backends und Frontends:

Übersicht des Deployment-Prozess des Backends:
![Übersicht des Deployment-Prozess des Backends](/images/1_team_mystuff/ci4.jpg?width=50pc)

Übersicht des Deployment-Prozess des Frontends:
![Übersicht des Deployment-Prozess des Frontends](/images/1_team_mystuff/ci5.jpg?width=50pc)

__Das Backend wird unter der URL-Adresse__: https://my-stuff-backend.herokuapp.com/ __freigegeben__. 

__Ebenfalls ist das Frontend unter__ https://my-stuff-htw.herokuapp.com/ __zu erreichen__.

#### 1.8 JavaScript End to End Testing Framework: Cypress

Die Tests wurden mit Cypress durchgeführt. Cypress ist ein Framework, mit dem End-to-End-Tests durchgeführt werden können. 

##### 1.8.1 Installation

Um Cypress nutzen zu können, muss es zunächst installiert werden. Die Installation erfordert im ersten Schritt die lokale Installation von __Node__. Danach muss cypress in dem Projekt, in dem man die Tests schreiben möchte, generiert werden. In unserem Fall wurde cypress im Frontend installiert, da mit cypress das Frontend getestet werden kann. Mit diesem Befehl ___npm install cypress --save-dev___ kann cypress automatisch in das gewünschte Projekt installiert werden. 

Die Installation generiert automatisch einen Ordner namens cypress im Projekt neu:
![Cypress](/images/1_team_mystuff/cypress.jpg?width=50pc)

Die Tests werden im Ordner Integration von cypress geschrieben:
![Integration](/images/1_team_mystuff/integration.jpg?width=50pc)

Struktur eines Tests aus Cypress:

```
describe("Abmelden", function () {
   before(() => {
       cy.visit("https://my-stuff-htw.herokuapp.com/login");
   });
   describe('Benutzer auslogen', function () {
       it("logout -> Alain", function () {

           cy.get(':nth-child(1) > a > #forward').click();

       });
   });
});
```

##### 1.8.2 Ausführung von Tests:

Die Ausführung der Tests wird über den folgenden Befehl durchgeführt: ___npx cypress open___. 
Nach der Ausführung dieses Befehls sieht man die Benutzeroberfläche von Cypress mit den verschiedenen geschriebenen Tests.

Folgende Tests wurden geschrieben: _new-modul-add_, _abmelden_, _create-user_, _login_
![Ausführung](/images/1_team_mystuff/ausfuehrung.jpg?width=50pc)

Es ist möglich, die Tests einzeln auszuführen oder alle Tests direkt auszuführen. Die Ergebnisse bleiben gleich, da die Tests entweder bestehen oder bei einem Fehler fehlschlagen. 

![Tests](/images/1_team_mystuff/tests.jpg?width=50pc)
Auf diesem Bild ist zu bemerken, dass die ausgeführten Tests alle fehlerfrei durchlaufen werden. Erfolgreiche Tests sind grün markiert, während fehlgeschlagene Tests rot markiert sind.

#### 1.9 Fazit

Die Planung sowie die Umsetzung anhand eines Prototyps wurde bei dem Projekt MyStuff erfolgreich umgesetzt. Der Prototyp enthält dabei die Grundlegenden Funktionalitäten, wie das Erstellen und Löschen von Modulen sowie das Anlegen und Bearbeiten von ToDos. Auch können neue Benutzer angelegt werden. Die Daten von den einzelnen Benutzern werden dabei erfolgreich in der MongoDB gespeichert. Des Weiteren konnte eine CI/CD-Pipeline erfolgreich aufgesetzt werden. Außerdem ist es möglich automatisierte Test durchzuführen.

Die Implementierung der Links mit automatisierten Tags konnte auch Zeitgründen nicht mehr komplett umgesetzt werden.