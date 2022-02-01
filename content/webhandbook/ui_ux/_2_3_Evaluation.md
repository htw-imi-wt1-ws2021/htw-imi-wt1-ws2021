---
title: 2.3 Evaluation von User Experience
description : "User Experience"
tags: ["UX", "User Experience", "Benutzererfahrung"]
---

#### 2.3 Evaluation
Um die beschriebenen Komponenten umzusetzen und somit die UX zu optimieren, gilt es, diese fortlaufend zu evaluieren. Hierfür existieren verschiedene Methoden, welche in die Kategorien formative Evaluation oder summative Evaluation eingeordnet werden können. Ersteres beschreibt dabei fortlaufende Methoden zur Evaluation eines Produktes während der Entwicklung, wodurch Bereiche mit Verbesserungspotenzial identifiziert werden sollen. Summative Evaluationen hingegen werden kurz vor oder nach Abschluss einer Entwicklungsphase durchgeführt, um zu prüfen, inwieweit die Anforderungen an das Produkt und dessen Qualität erfüllt sind.

Wichtig ist dabei, dass auch immer der Nutzungskontext betrachtet werden muss. Dazu zählen Preim und Dachselt die Benutzergruppe, die Aufgabe und die Umgebung, in der ein interaktives System benutzt wird. Mit Umgebung ist tatsächlich die physische Umgebung gemeint, da beispielsweise das Nutzen einer Anwendung im Freien auf einem mobilen Endgerät sich von den Ansprüchen unterscheidet, die an eine interaktive Anwendung im Operationssaal gestellt werden. In Bezug auf Webanwendung steht vor allem die Betrachtung der Nutzung auf verschiedenen Endgeräten wie PC, Tablet oder Smartphone an erster Stelle. Außerdem der Sinn der Anwendung von Bedeutung, da beispielsweise eine Anwendung für Online-Banking möglichst seriös und nicht verspielt wahrgenommen werden soll. Im Gegensatz dazu stehen Webanwendungen für freizeitorientierte Angebote, die auch Spaß machen dürfen.

Insgesamt wird empfohlen, mehrere Methoden zur Evaluation einer Anwendung zu nutzen und diese auch iterativ während der Entwicklung der Anwendung durchzuführen. Dadurch werden viele Aspekte erfasst und die bestmögliche UX geschaffen. Die Nielsen Norman Group zählte jedoch 2014 20 Methoden zu den gängigsten:

Usability-Lab Studies - Ethnographic Field Studies - Participatory Design - Focus Groups - Interviews - Eyetracking - Usability Benchmarking - Moderated Remote - Usability Studies - Unmoderated Remote - Panel Studies - Concept Testing - Diary/Camera Studies - Customer Feedback - Desirability Studies - Card Sorting - Clickstream Analysis - A/B Testing - Unmoderated UX Studies - True-Intent Studies - Intercept Surveys - Email Surveys

Im Folgenden sollen nun auf drei der Methoden genauer eingegangen werden.

__Nutzerbefragungen__

Eine konkrete Methode zur Evaluation der UX von Webanwendungen ist das Durchführen von Nutzerbefragungen. Diese zählen zu der Kategorie formative Evaluation und können online oder in Präsenz mit einer ausgewählten Nutzerschaft erfolgen. Letztere Variante liefert dabei im Gegensatz zu ersterem qualitative Ergebnisse statt quantitative. Von Interesse sind hierbei auch demografische Informationen über die Nutzer, da diese den Kontext der Antworten konkretisieren.
Eine standardisierte Methode von Nutzerbefragungen ist der AttrakDiff-Fragebogen, welcher von Prof. Dr. Marc Hassenzahl entwickelt wurde. Es basiert auf seiner Idee von hedonistischen und pragmatischen Qualitäten, welche die Basis des Attraktivitätsurteils über die Anwendung bildet. Pragmatische Qualitäten sind dabei übliche Usabilityaspekte, während hedonistische eher Aspekte wie Spaß und Nutzungsfreude betrachten. Der Fragebogen besteht aus 28 Items, welche im Format eines semantischen Differentials abgefragt werden. Auf eine Skala von jeweils gegensätzlichen Adjektiven wie „verwirrend - übersichtlich“  oder „zu selbstorientiert - zu handlungsorientiert“ kann der Nutzer aus sieben Abstufungen wählen. Der jeweilige Mittelwert eines Items bildet den Skalenwert für pragmatische und hedonische Qualität, sowie der Attraktivität der Anwendung.

__Eye Tracking__

Eye Tracking (dt. Blickbewegungsmessung) ist eine summative Methode zur Evaluation der UX, welche die Bewegung des Blicks des Nutzers beobachtet. Auf einem niedrigeren Niveau ist auch das Mouse Tracking möglich, welches lediglich die Mausbewegung aufnimmt.
Der Ablauf besteht darin, dass der Nutzer - meist ohne jegliche Vorkenntnisse - die Anwendung betrachten oder bei tiefergehenden Messungen festgelegte Aufgaben in der Anwendung durchführen muss. Dabei wird durch ein spezielles Eye Tracking Gerät oder bei einfachen Messungen mit einer üblichen Webcam seine Blickbewegung registriert. 
Zur Auswertung dieser Messung eignen sich *Heat* oder *Opacity Maps* oder *Gazeplots*, welche darstellen, wie der Nutzer die Anwendung wahrnimmt. Letzteres gibt sogar Aufschluss über die Reihenfolge, in welcher die Blickbewegung auf die Anwendung stattfindet. Je nach Intensität des Blicks zeigt sich dadurch beispielsweise die Dauer, die der Nutzer auf einer Area verbringt oder welche Elemente der Seite am meisten Aufmerksamkeit erregen oder komplett übersehen wurden. Die Bereiche der Anwendung, welche besonders deutlich wahrgenommen wurden, nennen sich *Areas of Interest*.

![5.1 Beispiel Heat Map](/webhandbook/ui_ux/images/4.jpg?width=20pc)
![5.2 Beispiel Opacity Map](/webhandbook/ui_ux/images/5.png?width=20pc)
![5.3 Beispiel Glazeplot](/webhandbook/ui_ux/images/6.png?width=20pc)

__Fokusgruppen__

Die Fokusgruppe, auch Gruppendiskussion genannt, ist eine Technik, um Meinungen, Bedenken, Gefühle und Erfahrungen von den Teilnehmern zu sammeln. Der Unterschied zu einer Benutzerbefragung ist dabei, dass die Fokusgruppe von einem Diskussionsleiter moderiert wird und bis zu zwei Stunden dauern kann. Dies geschieht unter der Voraussetzung, dass die Einzelpersonen in der Gruppe mitdiskutieren, sodass eine Gruppendynamik entsteht. Üblicherweise geschieht dies mit sechs bis neun Personen, die der Zielgruppe angehören und mehrfach mit unterschiedlichen Personen durchgeführt.
Mögliche Fragen, die hierbei beantworten, werden können, sind „Welche Inhalte und Funktionen werden momentan nicht genutzt und warum?“ oder „Welche Variante einer Idee, einer Funktion oder eines Designs bevorzugen die Nutzer?“.
Diese Methode kann zu jedem Zeitpunkt der Entwicklung angewendet werden, jedoch ist die Methode Fokusgruppe alleine nicht aussagekräftig genug für eine umfassende Evaluierung. Dies ist darauf zurückzuführen, dass Teilnehmer zwar durch ein dynamisches Gespräch viel wertvolle Aspekte ansprechen, die Anwendung selbst aber bei der tatsächlichen Nutzung anders verwendet wird, als im Gespräch ausgedrückt.