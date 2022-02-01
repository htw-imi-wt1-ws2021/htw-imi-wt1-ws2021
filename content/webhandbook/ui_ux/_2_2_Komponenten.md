---
title: 2.2 Komponenten des User Experience Prozesses
description : "Komponenten"
tags: ["UX", "Benutzerrecherche", "Informationsarchitektur", "Visualisierung"]
---

#### 2.2.1 Benutzerrecherche
Einer der elementaren Bausteine für eine erfolgreiche Benutzererfahrung ist ein klares Verständnis davon, wer die Benutzer sind und was sie von der Anwendung fordern und erwarten. Dies ist bereits vor der Planung der eigentlichen Anwendung hilfreich, da so ein Produkt entwickelt werden kann, welches nützlich für den Endnutzer ist.
Die Interaction Design Foundation gliedert Benutzerrecherche dabei in zwei Teile: die qualitativen und den quantitativen Forschung, welche jeweils *attitudinal* (dem Nutzer zuhören) und *behavioral* (die Handlungen des Nutzers beobachten) erfolgen kann. Sie empfehlen außerdem eine Mischung aus all diesen Vorgehenweisen zu verwenden.

Ist die Benutzerrecherche fortgeschritten, könnten die Ergebnisse in Form von *Personas* festgehalten werden. Eine Persona ist ein fiktiver Charakter mit einer fiktiven Persönlichkeit, demografischen, psychografischen und anderen Merkmalen. Der Charakter basiert jedoch auf der jeweiligen Zielgruppe, um die Suche nach Lösungen zu unterstützen, die am besten zu den jeweiligen Nutzergruppen passen. Hierfür werden üblicherweise drei bis vier Personas erstellt, welche mit Namen, Bild und Zusammenfassung zu wesentlichen Aspekten in Form einer DIN-A4 Seite dargestellt werden. Diese dienen jedem Beteiligten während des Projekts, sich die Probleme und Bedürfnisse der Zielgruppe vor Augen zu behalten.

Der letzte Schritt für ein fundiertes Wissen über die Benutzer und Zielgruppe ist das Entwickeln von Benutzerszenarien für die Personas. Sie stellen realistische Situation dar, in welchen sich die Nutzer befinden und in denen die Anwendung dem Nutzer bestmöglich dienen soll. Die Basis dafür bildet die vorgangegangene Benutzerrecherche und die Personas. Wichtig ist ferner die Beschreibung des Aspekts, welche Motivation und Ziele der Nutzer hat und welche Aufgaben er tätigen muss, um diese zu erfüllen. Außerdem sollte erläutert werden, in welchen Situationen er die Anwendung nutzt und welche Herausforderungen sich daraus ergeben. Ein komplett ausgearbeitetes Beispiel hierfür ist in der Abbildung 1.3 zu sehen.

![2.2.1 Beispiel ausgearbeitete Benutzerrecherche](/webhandbook/ui_ux/images/8.PNG?width=45pc)

Zusammenfassend ist dieser Aspekt der UX signifikant für die Attribute *useful* und *usable* des UX Honeycombs.

#### 2.2.2 Informationsarchitektur
Bei der Entwicklung einer Anwendung ist es bedeutsam, sich im Vorfeld mit der Organisation und Strukturierung von Inhalten zu befassen. Dafür müssen Fragen beantwortet werden wie „Wie soll der Nutzer durch die Anwendung navigieren?“ oder „Nach welcher Indexierung erfolgt die Suchmaschine der Anwendung?“. Vor allem bei komplexeren Anwendungen ist eine frühe Planung und Feedback der Nutzer unabdingbar.
Dabei wird zwischen zwei Arten von Informationsarchitektur unterschieden: Top-Down-Informationsarchitektur und Bottom-Up-Informationsarchitektur. Für beide Arten ist eine vorherige Benutzerrecherche notwendig, aus der hervorgeht, welche Informationen die Nutzer wohl am meisten benötigen. Demnach wird bei der Top-Down-Architektur, die Anwendung so konzipiert, dass der Nutzer ausgehend von der Startseite aus effektiv und einleuchtend zu den benötigten Informationen navigieren kann. Bei der Bottom-Up-Architektur hingegen wird beachtet, wie der Nutzer sich zurechtfindet, wenn er über einen beliebigen Punkt in die Webseite einsteigt, beispielsweise durch den Aufruf der Seite über eine Suchmaschine.
Zur Abbildung und Planung der Informationsarchitektur eignen sich *Site Maps*. Ein Beispiel hierfür ist die Side Map der Webseite von Apple.

![2.2.2 Beispiel Side Map](/webhandbook/ui_ux/images/7.PNG?width=45pc)

Dieser Aspekt der UX hat direkte Auswirkungen auf das Attribut *findable* im UX Honeycombs.

#### 2.2.3 Visualisierung
Meist reicht es nicht aus, nur in der Theorie von einer Anwendung zu sprechen. Deshalb ist eine Visualisierung in jeglicher Form sinnvoll, um die Anwendung zu erproben und Feedback einzuholen. Auch dieser Aspekt kann eine positive Beeinflussung der Attribute *useful* und *usable* des UX Honeycombs hervorbringen.
Im Folgenden sollten die gängigsten Formen erläutert werden. Sie sind dabei aufsteigend nach deren Aufwand und damit verbundenen *Fidelity* (dt. Detaillierungsgrad) gelistet:

__Skizzen__

Eine Skizze ist eine meist handgezeichnete Darstellung, die hilft abstrakte Überlegungen verbildlicht und erste Konkretisierungen zur Struktur und Funktionen der Webseite festzuhalten. Sie schafft einheitliches Verständnis und auch Raum für weitere Fragen und Aspekte, die zu klären sind. Vorteil dieser Art der Visualisierung ist die Schnelligkeit und Vorläufigkeit. Denn dadurch ist es möglich, einfach Änderungen vorzunehmen und innovative Ansätze zu fördern.
Generell eignen sich Skizzen vor allem für die Anfangsphase des Projekts. Von Vorteil sind dabei Informationen wie Personas, Use Cases und bereits definierte Anforderungen an das System.

__Wireframes__

Die nächste Stufe von Visualisierung sind Wireframes. Der Begriff kommt ursprünglich aus dem Industrieumfeld, wo es als Möglichkeit genutzt wird, schnell 3D-Objekte zu instanziieren, die nur die geplante äußere Form besitzt. Ebenso werden Wireframes in UXD genutzt, indem sie bereits die Originalgröße der fertigen Anwendung besitzen und somit verdeutlichen, ob die Überlegungen aus den Skizzen sinnvoll sind. Auch hier sind die tatsächlichen Inhalte noch nicht notwendig und Designvorschläge sogar unerwünscht, weswegen oft mit Platzhaltertexten und -bildern gearbeitet wird. Wichtig ist dennoch, im Wireframe zu verdeutlichen, an welcher Stelle in Zukunft Elemente wie das Logo, Kopf- und Fußzeile oder Inhaltsbereiche sind. Mögliche Tool zur Erstellung von Wireframes sind Balsamiq, Adobe XD oder Visio von Microsoft, durch die die Entwicklung beschleunigt wird. Je nachdem wie ausgereift die Wireframes sind, dienen sie teilweise schon als Grundlage für User Test oder für die Programmierer. Ersteres wird vor allem durch *Wireflows* möglich, die einzelne Wireframes miteinander verknüpfen, wodurch der Nutzer sich quasi durch die Anwendung bewegen können. In der folgenden Grafik ist ein Beispiel für Wireframes einer E-Commerce-Webseite dargestellt.

![2.2.3 Beispiel Wireframe](/webhandbook/ui_ux/images/9.PNG?width=50pc)

__Mockups__

Mit Mockups werden nun die konzeptionellen Überlegungen aus vorherigen Schritten mit einem Designkonzept umgesetzt. Dabei sind Themen wie Farben, Typografie, Abstände und Bilder von Bedeutung.
Auch Mockups können wie Wireframes nutzbar sein, wodurch sie wie eine täuschend echte Attrappe auf Testnutzer wirken können. Das hier eingeholt Feedback ist insofern wertvoll, als dass der Nutzer durch sie ein gutes Gefühl dafür bekommt, wie sich die Anwendung in Zukunft verhalten kann.

__Prototypen__

Nicht zu verwechseln mit Paperprototypen, welche mehr einer detaillierten Skizze ähneln, sind Prototypen die Umsetzung der Mockups, welche elementare Funktionalitäten des Endprodukts beinhalten und gegebenenfalls schon mit den vorgesehenen Programmiersprache oder Framework umgesetzt sind. Der Vorteil gegenüber Mockups ist, dass nicht nur die Struktur und das Design erprobt werden können, sondern auch tatsächlichen Teile der Funktionen.
Diese Form der Visualisierung ist die aufwendigste und deshalb nicht geeignet für schnelles Feedback, jedoch für qualitativ wertvolles. Denn jedes UX Problem, welches im Prototypen sichtbar wird, kann vor der tatsächlichen Umsetzung behoben werden und somit Entwicklungskosten sparen. Dennoch sollte vor der Erstellung eines Prototyps klar festgelegt werden, wie hoch der Umfang des Prototyps ist und welche Ziele durch ihn erreicht werden sollen. Außerdem ist die Festlegung des Endgeräts, auf dem der Prototyp nutzbar sein soll, relevant für die Entwicklungskosten.