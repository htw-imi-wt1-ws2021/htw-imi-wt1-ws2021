---
title: "Serviceorientierte Modellierung"
description: "Serviceorientierte Modellierung"
tags: ["Microservices", "Services" ]
---

## Kernaspekte einer Microservice-Architektur 
Zwei Hauptmerkmale für eine Microservice-Architektur sind einerseits unabhängige Verknüpfungen und andererseits starke Zusammenhänge zwischen den Services.  Ändert sich ein Service, ohne andere Komponenten zu ändern und zu benötigen, so ist dieser Dienst unabhängig.  Eigenschaften und Methoden, die zusammenhängend sind, gehören in einem Modul.  
Um Probleme genau einzugrenzen und Abhängigkeiten zu verhindern, ist „Domain-driven Design“ (deutsch: domänengetriebenes Design) ein wichtiges Werkzeug. Die Ansätze u.a. das Domänenwissen der Abteilung/ Branchen, „Ubiquitous Language“ und „Bounded Context“ sind für das Konzeptionieren von Nöten.

## Ubiquitous Language
In der Realität arbeiten neben Entwickler auch Domänenexperten. Sie besitzen die Expertise eines Fachbereichs und vermitteln den Entwicklern das fehlende Wissen des Areals. Die Bedeutung eines Wortes sind bei beiden Parteien nicht dieselben. Diese Fachleute sprechen ihren eigenen Dialekt, so dass Entwickler sie nicht verstehen. Bei Akronymen von technischen bzw. fachlichen Begriffen kommen oft Missverständnisse zustande. Da eine gemeinsame Sprache im Team oder in der Organisation fehlt, sind somit die Kernanforderungen für die geschriebene Software nicht klar definiert und eingrenzbar. 
Entwickler und Experten müssen in einer gemeinsamen Sprache kommunizieren. Von daher ist die „Modell-basierte“-Sprache vorteilhaft. Diese Sprache beschreibt die Modelle, in diesem Fall die Domäne, dessen Name und ihre Eigenschaften sowie ihre herausragenden Operationen der Klassen. Diese Herangehensweise erleichtert es Entwickeln unter sich aber auch mit Domänenfachkräften zu kommunizieren. Diese Terminologie spiegelt sich auch im Quellcode, in „Use-Case“-Diagrammen und in Funktionsspezifikationen ab. 

## Bounded Context 
![Bounded Context](/webhandbook/microservices/images/5.png)
Das Konzept hinter „Domain-Driven-Design“ ist, dass ein Hauptdomäne zum Beispiel ein Unternehmen eine Menge von „begrenzten Kontexte“ (auf Englisch: „Bounded Context“) verfügt. In den Kontexten befinden sich Modelle. Jeder Kontext besitz eine Schnittstelle, wodurch sich die Modelle ihre Information untereinander austauschen können.  
Abbildung 5 illustriert eine Konzeption mit „Bounded Context“. Die farblich umhüllten Rahmen sind die „begrenzten Kontexten“ im System. Alle Modelle haben eine interregionale Beziehung zwischen min. einen oder mehreren Entitäten. Die Pfeile in solch einer Abbildung weisen darauf hin, welche Entität die Information einer anderen Domäne verwenden bzw. gespeichert werden darf. 

