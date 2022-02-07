---
title: Monolithische Applikationen
description: "Monolith"
tags: ["Microservice", "Monolithen"]
---

## Beschreibung und Aufbau
![Beschreibung](/webhandbook/microservices/1.png)
Monolithen sind in einer großen Codebasis geschrieben. Sämtliche Web-Prozesse des Business laufen über diesem Repository ab. Die Datenabfragen- und erstellungen erfolgen über eine Datenbankinstanz, die eine Menge von Tabellen hat. Der einzige Monolith ist für das Entgegennehmen der Anfragen von Browser- und mobilen Nativanwendungen zuständig. 

## Problem einer monolithischen Applikation 
Der Code wächst, je mehr Features ausgeliefert werden. Das Warten und Ändern des immer komplexer werdenden Codes ist erschwert, da selbst bei strengen Coderegeln immer wieder Eigenheiten und unterschiedliche Wissensstände der Entwickler zu komplexem und teilweise zu einarbeitungsintensivem Code führt. Einige Codeabschnitte, die zusammenhängend mit anderen Methoden sind, machen das Implementieren von neuen Services und Features und Lösen von Bugs schwierig [1].  
Der Monolith muss große Mengen an Daten verarbeiten und diese Informationen an Nutzern senden. Aufgrund der hohen Nutzeranfragen sind einige Services stark ausgelastet. Andere Services im System werden wenig oder nicht benutzt. Aufgrund der hohen Last fallen alle Services aus oder sind stark verlangsamt. Die Konsequenzen sind kaskadisch. Zudem sind monolithische Anwendungen schlecht skalierbar. 
