---
title: "Microservices"
description: "Microservices"
tags: ["Microservices" ]
---

## Bedeutung
![Bedeutung](/webhandbook/microservices/images/2.png)
Microservices sind kleine Einheiten eines Systems, die eine Menge von Funktionen und Eigenschaften einer Entität besitzen. Sie folgen dem „Single-Responsibilty-Principle“ und übernehmen eine Funktionalität des Systems. Sie sind eingegrenzt, nur nach ihren zugewiesenen Aufgaben, die von den Entwicklern selbst definiert sind, auszuführen.  [2] 
Jeder Microservice bekommt ihre eigene Programmiersprache und Datenbanktyp als Umgebung. Alle Services laufen in ihrer eigenen Instanz.  

## Zweck von Microservices
![Zweck](/webhandbook/microservices/images/3.png)
Sinn und Zweck von Microservices ist es ein flexibles System zu entwickeln, um Systemausfälle zu verhindern, neue Features auszuliefern, ohne dabei anderen Funktionen aus anderen Quellen einzubeziehen.  Arbeitsprozessen sind auf den Services verteilt, sodass nicht ein Server alle Prozesse verwalten muss. Durch das Separieren des Codes auf mehreren Services können sich einzelne Teams auf einen Service fokussieren. Sie verlieren somit nicht den Überblick und können für den Service einfacher, neue Funktionalitäten implementieren, Tests schreiben und den Code bereitstellen. Je nach Bedarf, Last und Anfragen, kann ein Service hoch oder runter skaliert werden. Läuft ein Service nicht ordnungsmäßig, so kann dieser Service mit einer neuen Technologieumgebung ausgetauscht werden, sodass andere Service von der Änderung nicht betroffen sind. Ebenso können Teams sich schnell an neuen Technologien anpassen und diese an ihren Technologiestack für ein bestimmten Service einbinden und ggf. austauschen. 
![Zweck_2](/webhandbook/microservices/images/4.png)

