---
title: "Standards und Entscheidungen"
description: "Standards und Entscheidungen"
tags: ["Microservices", "Decision", "Standads", "Principles"]
---

## Technologie-Entscheidung
Aufgrund der Microservice-Architektur sind die Entwickler nicht eingeschränkt, eine und dieselbe Technologiebasis zu nutzen. Jedes Team einer einzelnen Microservice kann eigenständig entscheiden welche Programmiersprache, Tools, Frameworks und Datenbanksystem sie verwenden wollen. Der wichtigste Faktor für die Auswahl ist die Expertise des Teams. Neben der Expertise ist die Unterstützung der gewünschten Programmierumgebung bei einem Anbieter (Serveranbieter, Cloud-Provider) wichtig. 

## Prinzipien und Standards 
Beim Entwickeln von Services ist für die Programmierer wichtig, dass sie einen Leitfaden befolgen. Der Software-Architekt ist für das Aufstellen von Prinzipien verantwortlich.  Diese Regeln geben den Entwicklern einen Überblick, wie sie die Services konzipieren sollen und lösen Barrikaden und erleichtern das Konstruieren einer immer komplex wachsenden Anwendung. 
Neben Prinzipien sind einheitliche Standards notwendig. Bei interregionalen Kommunikationen zwischen den Services sollte ein gemeinsames Mittel verwendet werden. Die gesamte Organisation entscheidet, ob sie SOAP, HTTP-REST, RPC, synchrone- oder asynchrone Programmierung für ihren Projekt nutzen wollen. 
Ebenfalls sollte die Organisation in Betracht ziehen, ob sie externe Module/Plugins für die Services verwenden oder ob sie vorgefertigten Codevorlagen für neuentwickelte Dienste schreiben wollen. 

