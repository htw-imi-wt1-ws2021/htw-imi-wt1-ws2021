---
title: CI/CD
tags: ["chapter"]
chapter: true
---

# CI: CONTINUOUS INTEGRATION / CD: CONTINUOUS DELIVERY PIPELINE


CI ist eine Abkürzung für Continuous Integration, was auf Deutsch kontinuierliche In-
tegration bedeutet. Dieser Vorgang ermöglicht es den Mitgliedern eines Teams, kontinu-
ierlich neue Codes in einem bestimmten Repository zu speichern. Dann dieser Datenmen-
ge führt CI automatisch Tests durch und prüft die Fehlerfreiheit. Gleichzeitig unterstützt
es die Softwareentwicklung, indem es Fehler schneller meldet und Lösungen anbietet.
Folgende Schritte werden als Pipeline bezeichnet: Der Programmierer lädt den Code in
das Repository hoch. CI empfängt die Daten automatisch und führt den Test durch. Durch
verschiedene Metriken stellt CI sicher, dass der Quellcode unter allen Bedingungen feh-
lerfrei ist. Wenn es einen Fehler entdeckt, korrigiert es ihn automatisch im Rahmen seiner
Möglichkeiten. Jeder Prozess wird mit einer Rückmeldung versehen, so dass der Benut-
zer den Entwicklungsfortschritt der Software nachvollziehen kann. Außerdem werden die
gemachten Fehler erkannt und daraus für das nächste Mal gelernt.
Im Rahmen des Moduls Webanwendungen wird ein kleines Buchkapitel über diesen Pro-
zess geschrieben. In dem Buch wird zuerst die Definition geschrieben. Die Bedeutung
der Begriffe CI und CD und ihre Beziehung zueinander werden erklärt. Anhand einer
Abbildung über die Softwareentwicklung kann der Prozess visuell dargestellt werden.
Anschließend werden die Elemente der Pipeline vorgestellt. Die Phasen, die eine Pipe-
line enthält, werden grundlegend beschrieben. Abschließend werden die am häufigsten
verwendeten Tools, die den Prozess unterstützen, vorgestellt. Am Ende des Artikels wird
ein Beispiel für eine Pipeline mit Codes beschrieben, die auf dem einem ausgewählten
Framework basieren. Die folgende Gliederung soll einen Überblick über das Buchkapitel
geben:

1. Ansatz von CI/CD: Definition
2. Unterschied zwischen CI und CD
3. Elemente einer CI/CD-Pipeline
4. CI/CD-Werkzeuge
5. Beispiel eine Pipeline