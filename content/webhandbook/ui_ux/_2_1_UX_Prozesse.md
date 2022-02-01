---
title: 2.1 User Experience Prozesse
description : "Human-Centered Design"
tags: ["UX", "Human-Centered Design", "Usability Engineering", "User Experience Design"]
---

Um eine gute User Experience zu gewährleisten, sollte bereits bei der Entwicklung der Anwendung stets die UX betrachtet werden. Dies gilt für alle Entwicklungsphase. Beispielsweise sollten in der Anforderungsanalyse Kundenwünsche konkretisiert, in der Prototypen-Erstellung verschiedene UX-Aspekte angesprochen und beim Testen die UX evaluiert werden. Für diese Herangehensweise gibt es den Begriff Human-Centered Design.

Das Human-Centered Design (dt. menschenzentrierte Gestaltung, HCD), welcher früher auch als User-Centered Design oder Usability-Engineering bezeichnet wurde, ist ein als ISO-Norm festgehaltener Prozess mit vier Phasen. Von dem Begriff User Experience Design grenzt er sich insofern ab, als dass dieser zwar dasselbe Ziel hat, aber erst einsetzt, wenn das Produkt definiert ist und somit nicht die komplette Entwicklungsphase betrachtet. Das Ziel von HCD ist, die Nutzungsanforderungen zu erfüllen und die Methode wird oft als Herangehensweise zur Gestaltung und Entwicklung von gebrauchstauglichen interaktiven Systemen verwendet. Für den Prozess werden Kenntnisse und Techniken aus den Bereichen der Arbeitswissenschaft und Ergonomie, sowie der Usabilityforschung herangezogen. Der Vorteil von HCD ist, dass iterativ und nutzerzentriert an die Entwicklung des Produkts herangegangen wird, um Defizite in der Nutzung zu früh verdeutlichen und in der weiteren Entwicklung zu beheben.

Im Folgenden werden die in der Grafik dargestellten vier Phasen von HCD grob erläutert. Sie sind generell für die Entwicklung jeglicher interaktiven Produkte geeignet, jedoch soll hier mehr auf deren Anwendung auf die Entwicklung von Webanwendungen eingegangen werden. Vorraussetzung für den Start dieses Prozesses ist, dass zuständige Personen und Stakeholder identifiziert werden, geplant wird, inwieweit HCD in die generelle Entwicklungsmethode (Scrum, Wasserfall, etc) integriert werden kann und Raum für Kommunkation geschaffen wird. Außerdem ist eine zeitliche Planung und eine damit verbundene Meilenstein-Festlegung sinnvoll.

![2.2 Menschenzentrierte Gestaltung nach ISO 9241-210](/webhandbook/ui_ux/images/10.png?width=50pc)


1. Analysephase: Verstehen und definieren des Nutzungskontexts

Der Kontext einer Anwendung besteht laut ISO Norm aus „den Benutzermerkmalen, Aufgaben und organisanisatorische, technische und physische Umgebung [...], in dem das System verwendet wird“. Diese Informationen werde durch Methoden oder die Analyse von ähnlichen Systemen erforscht und diesen dann als Grundlage für die Entwicklung der Anwendung. Denn nur wenn der Kontext, indem die Anwendung genutzt wird, klar definiert ist, kann eine nutzerzentrierte Entwicklung von Anfang an erfolgen.
Die Definition des Nutzungskontext muss laut Norm dabei den Benutzer und sonstige Stakeholder, Merkmale der Benutzer, Ziele und Aufgaben sowie die Umgebung des Systems beschreiben. Letzteres beinhaltet die technische (Programmiersprache, Framework, Endgeräte) und die physische Umgebung (Internetverbindung, Beleuchtung). 

2. Spezifikationsphase: Festlegen der Nutzungsanforderungen

Basierend auf dem Nutzungskontext werden nun Nutzungsanforderungen abgeleitet. Mögliche Nutzeranforderungen sind dabei folgenden:
- Anforderungen, welche durch die Betrachtung des Nutzungskontexts und speziell 
- Anforderungen, welche bereits durch festgelegte Normen und Richtlinien zu UX, UI und Gebrauchtauglichkeit stammen.
- Anforderungen, welche die Usability adressieren. Hierbei sollen auch messbare Kritierien aufgenommen werden, die die Zufriedenheit im beschrieben Nutzungskontext.
- Anforderungen, die durch organisatorische Aspekte der Anwendung benötigt werden.

Die Anforderungen müssen generell durch Stakeholder verifiziert, nachprüfbar und widerspruchsfrei sein. Falls im Verlauf der Iterationen Unklarheiten deutlich werden, gilt es diese zu dokumentieren und die Anforderungen weiter zu spezifizieren.
Die festgelegten Nutzungsanforderungen sind Teil der Gesamtanforderungen eines interaktiven Systems und damit auch Teil des Lastenhefts.

3. Designphase: Erarbeitung von Gestaltungslösungen

In dieser Phase werden nun Lösungen entwickelt. Folgende Grundsätze der Gestaltung sind in ISO 9241-110 beschrieben und gilt es dabei zu involvieren: Aufgabenangemessenheit, Selbstbeschreibungsfähigkeit, Konformität mit Benutzererwartungen, Lernförderlichkeit, Steuerbarkeit, Fehlertoleranz und Individualisierbarkeit.

4. Evaluationsphase: Evaluierung der Gestaltungslösungen

Ziel dieser Phase ist es, für jeder der vorherigen Phasen Feedback vom Nutzer zu erhalten und dadurch Problem der entwickelten Lösungen aufzuzeigen. Im Idealfall erfüllt die Gestaltungslösung bereits bei der ersten Iteration alle Nutzungsanforderungen und der Anwendung ist damit feritgstellt. Im Normfall ist die vierte Phase jedoch der Anfang einer neuen Iteration in jede andere Phase, wodurch Inkrement stetig verbessern wird, bis alle Anforderungen erfüllt sind.

Da der HCD Prozess viele Aspekte und Methoden vereint, sollen nun einzelne Teilaspekte im folgenden Kapitel vorgestellt werden, um einen besseren Überblick von HCD zu ermöglichen. Das Ziel aller dieser Komponenten ist es, dass der Nutzer seine Aufgaben gut (effektiv, effizient und zufriedenstellend) durchführen kann.