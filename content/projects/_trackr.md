---
title: Trackr
weight: 2
tags: ["projekt4"]
pre: "<b>4. </b>"
---

![Trackr Logo](/images/4_team_trackr/trackr_logo.png?width=30pc)


Änderungen einfach Tracken.

## 1 Teammitglieder

Julia, Hedi, Ben, Lisa

## 2 Ausgangslage

Die meisten Programmierer_innen nutzen Anwendungen wie Github, Gitlab, Bitbucket etc., um Code zu versionieren und um kollaborativ daran mit anderen zu arbeiten. Wenn es jedoch um das Erstellen und Verfassen von Textdokumenten geht, die nichts mit Code zu tun haben, gibt es verschiedene Ansätze, die jeder für sich verfolgt. Manche speichern mehrere lokale Versionen eines Dokuments mit verschiedenen Titeln ( z.B. der Klassiker “Abgabe_final_final2_FINAL”), andere überschreiben einfach immer wieder ihre Dateien. Daneben gibt es Online-Plattformen wie Google Docs, auf denen man kollaborativ an Textdokumenten arbeiten kann und bei denen automatisch Versionen erstellt werden, wobei das Feature vielen nicht bekannt ist – abgesehen davon, dass Google Docs eine proprietäre Anwendung ist und einen Google-Account voraussetzt. Sowas wie Github für Textdokumente aller Art, die man thematisch gruppieren und sortieren kann, wäre doch cool, oder?

## 3 Ziele

Das Ziel unseres Projekts ist es, eine Webanwendung zu erstellen, bei der man Textdokumente hochladen kann, die automatisch versioniert werden. Wir wollen keinen weiteren Texteditor bauen, sondern den Upload von Markdown-Files ermöglichen. Zudem soll kollaborativ an den Texten gearbeitet werden können. Ähnlich wie bei Github soll es möglich sein, Unterschiede zwischen zwei Versionen eines Textes miteinander vergleichen zu können und womöglich Änderungen aus zwei Dokumenten zu mergen. 

## 4 Use Cases

Die Anwendung kann für folgende Fälle verwendet werden:

- Ich bin kein/e Programmierer_in oder habe kein Github Pro Account (weshalb alle Repos öffentlich sind) und möchte trotzdem meine Markdown-Dateien versionieren. (Das klärt die Frage: “Warum nicht einfach Github dafür benutzen?”)
- Studierende wollen an einem Projekt zusammenarbeiten (z.B. unser Webhandbook) und müssen verschiedene Markdown-Files erstellen und zusammen daran arbeiten. 
- Beispiel aus dem Alltag: Bei einem Fragebogen für das PROFIT-Mentoring wurde eine Text-Datei rumgeschickt, die schlecht formatiert war und somit nicht gut zu bearbeiten. Stattdessen könnte man eine Markdown Datei in einem Ordner teilen, auf die jeder zugreifen kann und in einem einheitlichen Format editieren kann.


## 5 Technologien

- MEVN-Stack (MongoDB, Express.js, Vue.js (3), Node.js)
- Typescript
- Testing Frameworks Frontend: Vue Testing Utils, Cypress, Jest
- Testing Frameworks Backend: Jest
- Docker


## 6 Herausforderungen

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

## 7 Beschreibung 

In einer Webanwendung soll es möglich sein, Orderstrukturen anzulegen und in diesen Ordnern per Drag & Drop Dateien hochzuladen. Beim Upload eines neuen Dokuments wird automatisch eine Version mit dem Datum des aktuellen Tages erstellt. Wenn nun ein weiteres Mal ein Dokument im selben Ordner mit dem gleichen Namen und der gleichen Dateiendung hochgeladen wird, so wird automatisch eine weitere Version für das Dokument hinzugefügt, sodass sich nun zwei Dokumente im Versionsverlauf befinden. Bei Klick auf das Dokument bekommt man einen Überblick über alle bereits erstellten Versionen und kann diese jeweils herunterladen, löschen oder manuell noch eine neue Version hinzufügen. 

Wählt man zwei Versionen eines Dokuments aus, kann man sich die Unterschiede beider Versionen in einem Fenster, in dem beide Dokumente dargestellt werden, ansehen. Hier wäre es wünschenswert, dass hinzugefügte, veränderte oder gelöschte Zeilen als solche markiert werden und man Änderungen aus einer der Versionen in die andere übernehmen kann, um z.B. zwei Versionen zu einer neuen zu mergen.

Die Anwendung ist so konzipiert, dass zukünftig ermöglicht werden soll, dass Ordner freigegeben und mit anderen geteilt werden können, um gemeinsam darin zu arbeiten. So könnte eine Projektgruppe gemeinsam an Texten arbeiten, indem sich jeder den aktuellen Stand runterladen, bearbeiten und als neue Version hochladen könnte. Im Rahmen der verbleibenden Wochen wird das Collaboration-Feature aber nicht mehr umgesetzt.

![Storyboard](/images/4_team_trackr/storyboard_trackr.jpg?width=40pc)

## 8 Verlauf & Schritte

In der ersten Phase von ca. zwei Wochen wurden die Entscheidungen bezüglich der unterstützten Dateiformate sowie der eingesetzten Technologien getroffen werden. Seitdem wird mithilfe von wöchentlichen Sprints die Anwendung implementiert. Wir verzichten dabei aus Zeitgründen auf die Erstellung und Evaluierung eines Prototyps.

![User Story Map](/images/4_team_trackr/user-story-map.png?width=40pc)

## 9 CI/CD

### 9.1 Automated Tests

We divided this section into frontend and backend tests because they run independently from each other and cover different things.We did not write integration tests, which would be ideal if you want to test the communication between the frontend and the backend, but these tests are very complex to write and therefore we focused mainly on Unit Tests or E2E tests.

#### 9.1.1 Frontend

Ideally the frontend tests should cover things like interactions with the UI, in our case especially the file upload, creation and deletion in combination with the Vuex store and the Vue Router. They should make sure that each view and component is rendered correctly and that passing props works smoothly. There are two ways to write tests to assure that: E2E tests or unit tests.

We used two different Frameworks for those kind of tests:
- E2E Tests with Cypress
- Unit Tests with Jest

Cypress is a really nice Framework that lets you write E2E tests and see them run in a browser, so you can visually see what’s happening, jump forward, back or pause the test at any point. It’s mostly a way for testing UI components and user interaction with them, but in a more visual way. 

Unfortunately, it turned out quite hard to test the Vue Application with Cypress. That’s when we found that there is a thing like Vue Test Utils (https://vue-test-utils.vuejs.org), Vue’s own library for writing tests in combination with the popular testing Framework Jest. These tests were very straightforward and easy to write, because the documentation is really good and there are a lot of utility functions you can use.

The only really “hard” thing about it to understand is what you do with all your dependencies in your test: The Vue Components and Views mostly rely on the Vuex Store or the Vue Router, but you cannot test all these things together in unit tests. So the solution is to mock these things, meaning creating a “dummy” Vuex Store or Router in the tests that replace the actual implementation and return a certain value you define – now we were able to solely test the components and views without being dependent on other functionality in the App. 

All together, we wrote these tests:

- E2E/
  - components
    - File.spec.ts
    - Header.spec.ts
    - Modal.spec.ts
    - UploadButton.spec.ts
- Unit
  - components/
    - CreateFileVersionButton.spec.ts
    - File.spec.ts
    - Modal.spec.ts
    - UploadButton.spec.ts
  - views/
    - FileVersions.spec.ts

They cover the correct rendering of basic UI elements, making sure that clicking e.g. on the Upload Button triggers the correct Vuex Action and Router Action or that the contents of a previously created file are displayed correctly. 

#### 9.1.2 Backend

The backend tests are crucial to ensure a correct working API. The backend is responsible for fetching data from the MongoDB and providing it in the form of JSON objects that can then be used in the frontend. The tests are written using the JEST testing framework and deal with correct handling of the data primitives in use. 

We tried two approaches to test the API. In the first one, we worked with a common-jest.js file that handles the setup of the testing environment, e.g. the database connection, the import of necessary Mongoose schema files and other dependencies. These can then be used in the actual test files. We also created a folder in this setup where mock data can be accessed to fill the database. In this setup we currently have one test file (fileVersionsController.spec.js) which contains a test that first writes mock data to the MongoDB, retrieves it and then accesses the matching API endpoint to check whether the data was added correctly. 

While in the first approach the library “supertest” was used for mocking the network requests and response objects of the API, the second approach used JESTs own capabilities for mocking. The tests are contained in a single file with all necessary logic for setting up the database connection and resetting it after every test to start the next one in a clean and reliable state.

#### 9.2 Code Quality Assurance

We used ESlint (https://eslint.org) for Code Quality Assurance in our project. ESlint statically analyzes the code to find problems and quality issues. It allows the developers to define certain rules that work besides ESlint’s built-in rules. You can even make it fix problems automatically on save, or manually by selecting proposed improvements or fixes. In combination with Prettier (https://prettier.io), which enables us to format our code in an uniform way, it’s a very handy tool to see e.g. unused or undefined variables, errors and other miscellaneous bugs. It also supports TypeScript so it comes in very handy when checking types and proposing the right types.

#### 9.3 Deployment Pipeline
The code is built and integrated via GitHub Actions. On every commit and pull request to the master branch, the CI pipeline gets triggered. It would also be possible to trigger the pipeline with tags that are added to a commit. In this case, only major releases would trigger a new deployment of the application. Since our project is rather small right now and is only scheduled to have a limited number of releases, we chose a different solution.

Our current pipeline works as follows: The tests for the frontend and the backend will be conducted in parallel, while the job for the dockerization of the application will wait until the tests are run successfully. A commit with failing tests will not get merged. Following these steps, the docker image will be deployed on the server. 

#### 9.4 Continuous Deployment
We first need the credentials and description to where we should deploy our application – this is still on hold as we are waiting for the other group to give us this information. However since we already use Docker Compose for developing our project, everything is already containerized and therefore  system independent. So it will not be hard to get it running on the server.


## 10 Link zum Projekt

[Unser Projekt](http://localhost:8080)

#### 11 Screenshots vom Projekt

-

#### 12 Link zum Sourcecode

[Code can be found here.](https://github.com/JuliaZamaitat/trackr/tree/database)

