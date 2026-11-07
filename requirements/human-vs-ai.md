### Human-Version
Die Ergebnisse aus Teil 3 wurden als Grundlage verwendet, um die ursprünglichen Requirements zu überarbeiten und zu verbessern. Dabei wurden die zuvor identifizierten Qualitätsmängel berücksichtigt.

**REQ-001**    
Ursprüngliche Version: Das System muss Studierende automatisch benachrichtigen, wenn sie sieben Tage lang nicht im Online Campus aktiv waren.  
Verbesserung: Das System soll Studierende bei möglichen (vor definierten) Anzeichen für Unterstützungsbedarf benachrichtigen können.  

**REQ-002**
Ursprüngliche Version: Der Study Buddy muss schnell, intuitiv und besonders benutzerfreundlich sein.
Verbesserung: Der Study Buddy soll für Studierende einfach und verständlich bedienbar sein. 

**REQ-003**
Ursprüngliche Version: Das System muss bevorstehende Abgaben anzeigen, personalisierte Erinnerungen versenden, Lernfortschritte analysieren und Lehrende über Schwierigkeiten informieren.
Verbesserung: Das System soll auf bevorstehende Abgabetermine zugreifen können und diese den Studierenden anzeigen können. Die weiteren Funktionen (personalisierte Erinnerungen, Lernfortschrittsanalysen und Benachrichtigungen an Lehrende) müssen separat auf ihre Notwendigkeit geprüft werden.

**REQ-008**
Ursprüngliche Version: Das System muss alle Studierenden unabhängig von ihren Einstellungen über kritische Studienereignisse benachrichtigen.
Verbesserung: Das System soll Studierende über relevante Studienereignisse informieren können. Dabei muss definiert werden, welche Ereignisse als kritisch gelten und ob diese von der Benachrichtigungsdeaktivierung ausgenommen werden müssen. Der Widerspruch zu REQ-007 muss vorher geklärt werden.

**REQ-011**
Ursprüngliche Version: Studierende müssen für den Study Buddy ein separates Benutzerkonto mit eigenem Passwort erstellen.
Verbesserung: Der Study Buddy muss das bereits bestehende Authentifizierungssystem der Hochschule verwenden. Eine zusätzliche Benutzerverwaltung oder ein separater Login dürfen nicht eingerichtet werden.

---

### KI-Version
Requirements Review – Digital Study Buddy
1. Bewertungsgrundlage
Die fünf Anforderungen werden anhand der drei Qualitätsaspekte Inhalt, Dokumentation und Abgestimmtheit überprüft.
- Inhalt: Ist die Anforderung fachlich sinnvoll, notwendig, eindeutig und ausreichend vollständig?
- Dokumentation: Ist sie verständlich, präzise, einzeln prüfbar und nachvollziehbar formuliert?
- Abgestimmtheit: Ist erkennbar, dass die Anforderung mit den relevanten Stakeholdern abgestimmt wurde und keine ungeklärten Konflikte bestehen?
Die vergebenen Status bedeuten:
Status	Bedeutung
REWRITE	Die Anforderung kann auf Grundlage der vorhandenen Informationen präzisiert oder umformuliert werden.
INVESTIGATE	Wesentliche Informationen fehlen. Vor einer endgültigen Formulierung sind fachliche Klärungen erforderlich.
RECONSIDER	Die Anforderung enthält eine grundlegend fragwürdige Festlegung, die zunächst hinsichtlich ihrer Notwendigkeit überprüft werden sollte.

Die vorliegenden Entwürfe enthalten keine dokumentierten Stakeholderentscheidungen. Daher kann bei keiner Anforderung eine tatsächlich erfolgte Abstimmung bestätigt werden.

REQ-001 · The Seven-Day Rule
REWRITE
Original: Das System muss Studierende automatisch benachrichtigen, wenn sie sieben Tage lang nicht im Online Campus aktiv waren.
Qualitätsanalyse
Aspekt	Identifizierter Qualitätsmangel
Inhalt	Der Begriff „aktiv“ ist nicht definiert. Unklar ist, ob beispielsweise ein Login, ein Seitenaufruf oder eine Lernaktivität zählt.
Dokumentation	Der Zeitraum von sieben Tagen ist genannt, aber die genaue Berechnung, der Benachrichtigungszeitpunkt und der Kommunikationskanal fehlen.
Abgestimmtheit	Es ist nicht belegt, dass die Sieben-Tage-Grenze fachlich begründet oder mit Studierenden und Hochschulverantwortlichen abgestimmt wurde.

Zusätzlich ist ungeklärt, ob der Study Buddy auf die erforderlichen Aktivitätsdaten des Online Campus zugreifen kann. Die technische Verfügbarkeit darf nicht vorausgesetzt werden.
Verbesserte Anforderung (vorläufig)
Das System muss Studierende automatisch benachrichtigen, wenn für sie im Online Campus während sieben aufeinanderfolgender Tage keine Aktivität erfasst wurde.

Diese Formulierung übernimmt die vorgegebene Sieben-Tage-Regel, ohne sie als fachlich validiert darzustellen.

Offene Klärungen: Definition von Aktivität, Berechnung des Zeitraums, Häufigkeit und Kanal der Benachrichtigung, Datenverfügbarkeit sowie fachliche Begründung der sieben Tage.

Vorgeschlagene Akzeptanzkriterien (vorläufig):
1. Nach sieben aufeinanderfolgenden Tagen ohne erfasste Aktivität wird eine Benachrichtigung ausgelöst.
2. Wird innerhalb dieses Zeitraums eine Aktivität erfasst, wird die Bedingung der siebentägigen Inaktivität nicht erfüllt.
Diese Kriterien sind erst nach verbindlicher Definition von „Aktivität“ und der zeitlichen Berechnungslogik vollständig testbar.

REQ-002 · Fast and Friendly
INVESTIGATE
Original: Der Study Buddy muss schnell, intuitiv und besonders benutzerfreundlich sein.
Qualitätsanalyse
Aspekt	Identifizierter Qualitätsmangel
Inhalt	„Schnell“, „intuitiv“ und „besonders benutzerfreundlich“ sind subjektive Qualitätsbegriffe ohne fachliche Konkretisierung.
Dokumentation	Es fehlen messbare Kriterien, relevante Nutzungsszenarien, Testbedingungen und Zielwerte. Dadurch ist die Anforderung nicht objektiv überprüfbar.
Abgestimmtheit	Es ist nicht dokumentiert, welche Nutzungserwartungen Studierende haben oder welche Qualitätsziele mit den Stakeholdern vereinbart wurden.

Verbesserte Anforderung
Eine endgültige, testbare Anforderung lässt sich aus den vorhandenen Informationen nicht ableiten.

Als Struktur für eine spätere Spezifikation kann dienen:
Das System muss die noch festzulegende Kernaufgabe [Aufgabe] unter definierten Nutzungsbedingungen innerhalb von [Zeitgrenze] ausführen.

Für Benutzerfreundlichkeit wären beispielsweise konkrete Nutzungsszenarien und messbare Kriterien für die erfolgreiche Aufgabenerledigung festzulegen.

Offene Klärungen: Welche Funktionen sind zeitkritisch? Was verstehen die relevanten Nutzergruppen unter einfacher Bedienung? Welche Leistungs- und Usability-Ziele werden vereinbart?

Akzeptanzkriterien: Derzeit keine fachlich begründbaren Kriterien ableitbar. Konkrete Sekundenwerte, Erfolgsquoten oder Klickzahlen wären unbegründete Annahmen.

REQ-003 · The All-in-One Feature
INVESTIGATE
Original: Das System muss bevorstehende Abgaben anzeigen, personalisierte Erinnerungen versenden, Lernfortschritte analysieren und Lehrende über Schwierigkeiten informieren.
Qualitätsanalyse
Aspekt	Identifizierter Qualitätsmangel
Inhalt	Vier unterschiedliche Funktionen werden zusammengefasst. „Personalisiert“, „Lernfortschritte“ und „Schwierigkeiten“ sind fachlich nicht definiert.
Dokumentation	Die Anforderung ist nicht atomar und nur schwer unabhängig testbar. Auslöser, Datenquellen, Empfänger und Ergebnisse der jeweiligen Funktionen fehlen.
Abgestimmtheit	Besonders die Analyse individueller Lernfortschritte und die Weitergabe von Informationen an Lehrende benötigen eine Klärung von Zweck, Zugriffsberechtigungen und Datenschutz. Eine entsprechende Abstimmung oder Freigabe ist nicht belegt.

Verbesserte Anforderungen (Aufteilung)
Die vorhandenen Funktionswünsche sollten zunächst in vier eigenständige Anforderungsentwürfe aufgeteilt werden.
ID	Überarbeiteter Entwurf	Weiterer Klärungsbedarf
REQ-003a	Das System muss Studierenden ihre bevorstehenden Abgaben anzeigen.	Bedeutung von „bevorstehend“, Datenquelle, Aktualisierung
REQ-003b	Das System muss personalisierte Erinnerungen an Studierende versenden.	Personalisierungsregeln, Auslöser, Inhalte, Kanäle
REQ-003c	Das System muss die Lernfortschritte von Studierenden analysieren.	Messgrößen, Datenbasis, Analysezweck, Ergebnisdarstellung
REQ-003d	Das System muss Lehrende über Schwierigkeiten von Studierenden informieren.	Definition von Schwierigkeiten, Empfänger, Umfang, Berechtigungen und erforderliche Freigaben

Die Aufteilung verbessert die Dokumentationsqualität, löst aber noch nicht die fachlichen Unklarheiten.

Akzeptanzkriterium für REQ-003a (vorläufig):

- Ein vorhandener, einem Studierenden zugeordneter und nach der noch festzulegenden Definition bevorstehender Abgabetermin wird diesem Studierenden angezeigt.

Für REQ-003b bis REQ-003d sind ohne weitere Entscheidungen keine ausreichend konkreten Akzeptanzkriterien formulierbar.

Insbesondere darf REQ-003d nicht allein aufgrund des ursprünglichen Entwurfs als genehmigte Informationsweitergabe interpretiert werden.

REQ-008 · No Exceptions
RECONSIDER
Original: Das System muss alle Studierenden unabhängig von ihren Einstellungen über kritische Studienereignisse benachrichtigen.
Qualitätsanalyse
Aspekt	Identifizierter Qualitätsmangel
Inhalt	„Kritische Studienereignisse“ ist undefiniert. Außerdem ist unklar, warum ausnahmslos alle Studierenden unabhängig von ihren Einstellungen benachrichtigt werden müssen.
Dokumentation	Es fehlen Ereigniskategorien, Empfängerkriterien, Ausnahmen, Kanäle und Regeln für die Zustellung.
Abgestimmtheit	Die Einschränkung individueller Einstellungen ist nicht begründet. Ob entsprechende Vorgaben, Interessenabwägungen oder rechtliche Grundlagen bestehen, ist nicht dokumentiert.

Die Anforderung könnte mit der gewünschten Selbstbestimmung der Studierenden bezüglich Benachrichtigungen kollidieren. Ein tatsächlicher Stakeholderkonflikt ist damit jedoch noch nicht nachgewiesen.
Verbesserte Anforderung
Eine abschließende Neufassung ist derzeit nicht gerechtfertigt.

Ein möglicher, ausdrücklich noch zu prüfender Ansatz wäre:
Das System muss Studierende über für sie relevante kritische Studienereignisse gemäß noch festzulegenden Benachrichtigungsregeln informieren.

Diese Formulierung stellt keine bestätigte Anforderung dar. Insbesondere ist noch nicht entschieden, wann Benachrichtigungen verpflichtend sein dürfen und welche Einstellungen berücksichtigt werden müssen.

Notwendige Abstimmungen: Definition kritischer Ereignisse, betroffene Personengruppen, verpflichtende oder optionale Benachrichtigungen, rechtliche und organisatorische Grundlagen sowie mögliche Ausnahmen.

Akzeptanzkriterien: Noch nicht sinnvoll spezifizierbar, solange Ereignisse und Benachrichtigungsregeln nicht feststehen.

REQ-011 · The New Login
RECONSIDER
Original: Studierende müssen für den Study Buddy ein separates Benutzerkonto mit eigenem Passwort erstellen.
Qualitätsanalyse
Aspekt	Identifizierter Qualitätsmangel
Inhalt	Die Anforderung schreibt eine konkrete Authentifizierungslösung vor, ohne das zugrunde liegende Bedürfnis oder die Notwendigkeit eines zusätzlichen Kontos zu erläutern.
Dokumentation	„Separat“ ist nicht näher definiert. Es fehlen Informationen zu Benutzerverwaltung, Registrierung und zum Verhältnis zu bestehenden Hochschulzugängen.
Abgestimmtheit	Es ist nicht dokumentiert, ob diese Lösung mit Studierenden, IT-Betrieb und Informationssicherheit abgestimmt wurde. Alternativen wie die Nutzung einer bestehenden Hochschulidentität wurden nicht nachweislich geprüft.

Ein separates Benutzerkonto könnte zusätzlichen Verwaltungsaufwand verursachen. Ob eine Anbindung an bestehende Hochschulsysteme möglich oder erwünscht ist, geht aus dem Entwurf nicht hervor.
Verbesserte Anforderung (lösungsneutraler Entwurf)
Das System muss Studierenden eine Authentifizierung für die Nutzung des Study Buddy ermöglichen.

Diese Formulierung erhält das aus der ursprünglichen Anforderung erkennbare Authentifizierungsziel, ohne bereits eine separate Kontoverwaltung vorzuschreiben.

Offene Klärungen: Ist ein separates Konto tatsächlich erforderlich? Gibt es nutzbare bestehende Identitäten? Welche organisatorischen und sicherheitsbezogenen Vorgaben gelten? Wer verwaltet Benutzerkonten und Zugriffsberechtigungen?

Akzeptanzkriterien: Erst nach Festlegung des Authentifizierungskonzepts konkretisierbar. Die ursprüngliche Pflicht zur Erstellung eines zusätzlichen Kontos sollte bis dahin nicht als verbindlich betrachtet werden.

2. Zusammenfassende Bewertung
Anforderung	Hauptproblem	Status
REQ-001	Unklare Aktivitätsdefinition und nicht begründeter Zeitraum	REWRITE
REQ-002	Subjektive, nicht messbare Qualitätsziele	INVESTIGATE
REQ-003	Mehrere Funktionen, unklare Datenverarbeitung und Informationsweitergabe	INVESTIGATE
REQ-008	Nicht begründete verpflichtende Benachrichtigung unabhängig von Einstellungen	RECONSIDER
REQ-011	Nicht begründete Festlegung auf eine konkrete Authentifizierungslösung	RECONSIDER

3. Gesamtfazit aus Requirements-Engineering-Sicht
Die fünf Anforderungsentwürfe sind in ihrer derzeitigen Form noch nicht ausreichend spezifiziert, um sie vollständig und zuverlässig abnehmen zu können.

Die wesentlichen Verbesserungsmaßnahmen sind:
1. Begriffe präzisieren: Beispielsweise „Aktivität“, „Benutzerfreundlichkeit“ und „kritische Studienereignisse“ eindeutig definieren.
2. Anforderungen atomisieren: Die vier Funktionen aus REQ-003 getrennt dokumentieren und bewerten.
3. Lösungsneutralität prüfen: Insbesondere bei REQ-011 zunächst das Authentifizierungsbedürfnis klären, bevor eine technische Lösung verbindlich vorgeschrieben wird.
4. Stakeholderabstimmungen nachholen: Benachrichtigungspflichten, Datennutzung und Informationsweitergabe müssen fachlich geklärt werden.
5. Prüfbarkeit herstellen: Akzeptanzkriterien erst dann konkretisieren, wenn die erforderlichen fachlichen Entscheidungen vorliegen.
Wichtige Unterscheidung: Eine sprachlich verbesserte Anforderung ist noch keine fachlich validierte Anforderung. Die vorgenommenen Umformulierungen stellen deshalb, wo Informationen fehlen, ausdrücklich vorläufige Entwürfe dar.

---

### Quality Showdown

**REQ-001 - The Seven-Day Rule**
| Bewertungskriterium | Human | AI |
|---|:---:|:---:|
| Fachliche Angemessenheit | 4 | 2 |
| Eindeutigkeit und Verständlichkeit | 2 | 3 |
| Vollständigkeit und Überprüfbarkeit | 1 | 3 |
| Umgang mit Annahmen | 4 | 3 |
| Abstimmung und Konflikte | 3 | 2 |
| **Gesamt** | **14/25** | **13/25** |

**Begründung:**
Die Human Version verzichtet auf die unbegründete Frist von sieben Tagen und konzentriert sich stattdessen auf mögliche Anzeichen für Unterstützungsbedarf. Allerdings ist nicht eindeutig definiert, welche Anzeichen gemeint sind und wann eine Benachrichtigung erfolgen soll.  
Die AI Version ist konkreter formuliert und enthält vorläufige Akzeptanzkriterien. Sie übernimmt jedoch die Sieben-Tage-Regel als verpflichtende Anforderung, obwohl deren fachliche Notwendigkeit nicht nachgewiesen wurde.  
**Fazit:** Die Human Version ist fachlich vorsichtiger, während die AI Version konkreter formuliert ist. Bei beiden sind aber noch offene Punkte, die weitere Klärungen benötigen.  

### REQ-002 – Fast and Friendly

| Bewertungskriterium | Human | AI |
|---|:---:|:---:|
| Fachliche Angemessenheit | 4 | 4 |
| Eindeutigkeit und Verständlichkeit | 3 | 4 |
| Vollständigkeit und Überprüfbarkeit | 1 | 2 |
| Umgang mit Annahmen | 4 | 5 |
| Abstimmung und Konflikte | 2 | 4 |
| **Gesamt** | **14/25** | **19/25** |

**Begründung:**
Die Human Version ist einfacher und verständlicher formuliert als das Original. Allerdings sind die Begriffe "einfach" und "verständlich" noch immer subjektiv und auch nicht messbar. Außerdem wird die ursprüngliche Anforderung an die Geschwindigkeit nicht mehr berücksichtigt.  
Die AI Version erkennt, dass die ursprünglichen Anforderungen nicht ausreichend definiert sind und keine überprüfbaren Kriterien vorliegen. Sie erfindet keine konkreten Werte, sondern zeigt auf, welche Informationen noch benötigt werden. Allerdings liefert auch die KI noch keine vollständig überprüfbare Anforderung, sondern nur eine Vorlage mit Platzhaltern.  
**Fazit:** Die AI Version ist in diesem Fall hilfreicher, weil sie die fehlenden Informationen genauer identifiziert und unbegründete Annahmen vermeidet. Die Human Version ist kürzer und verständlicher, behebt aber nicht alle Qualitätsprobleme.  

### REQ-003 – The All-in-One Feature

| Bewertungskriterium | Human | AI |
|---|:---:|:---:|
| Fachliche Angemessenheit | 3 | 4 |
| Eindeutigkeit und Verständlichkeit | 3 | 4 |
| Vollständigkeit und Überprüfbarkeit | 2 | 3 |
| Umgang mit Annahmen | 2 | 4 |
| Abstimmung und Konflikte | 2 | 4 |
| **Gesamt** | **12/25** | **19/25** |

**Begründung:**
Die Human Version konzentriert sich auf die Anzeige bevorstehender Abgabetermine und ist dadurch einfacher und verständlicher formuliert. Damit ist es zwar einfacher formuliert, arbeitet die anderen drei Funktionen jedoch nicht als eigenständige Anforderungen aus. Außerdem ist nicht geklärt, ob die benötigten Daten überhaupt zur Verfügung stehen und was genau als bevorstehender Abgabetermin gilt.  
Die AI Version teilt die ursprüngliche Anforderung in vier einzelne Anforderungen auf und berücksichtigt dadurch alle Funktionen. Zusätzlich werden offene Fragen und mögliche Datenschutzprobleme erkannt, insbesondere bei der Weitergabe von Informationen an Lehrende. Allerdings sind auch die KI-Anforderungen noch nicht vollständig überprüfbar und verwenden teilweise verpflichtende Formulierungen, obwohl die Funktionen noch nicht bestätigt wurden.  
**Fazit:** Die AI Version ist insgesamt vollständiger und berücksichtigt mehr mögliche Probleme. Die Human Version ist zwar einfacher formuliert, lässt aber wichtige Funktionen weg. Beide Versionen benötigen noch weitere Klärungen, bevor verbindliche Anforderungen entstehen können.  

### REQ-008 – No Exceptions

| Bewertungskriterium | Human | AI |
|---|:---:|:---:|
| Fachliche Angemessenheit | 4 | 4 |
| Eindeutigkeit und Verständlichkeit | 3 | 4 |
| Vollständigkeit und Überprüfbarkeit | 2 | 2 |
| Umgang mit Annahmen | 4 | 5 |
| Abstimmung und Konflikte | 4 | 4 |
| **Gesamt** | **17/25** | **19/25** |

**Begründung:**
Die Human Version formuliert die Anforderung verständlicher und erkennt, dass kritische Studienereignisse definiert werden müssen. Zusätzlich wird der Konflikt mit REQ-007 berücksichtigt und offengelassen, ob bestimmte Benachrichtigungen verpflichtend sein müssen.  
Die AI Version erkennt ebenfalls die fehlenden Definitionen und geht genauer auf die notwendigen Abstimmungen und möglichen Konflikte ein. Sie vermeidet unbegründete Entscheidungen und weist darauf hin, dass noch keine überprüfbaren Akzeptanzkriterien festgelegt werden können.     
**Fazit:** Die AI Version ist etwas ausführlicher und berücksichtigt mehr offene Fragen. Die Human Version erkennt aber ebenfalls die wesentlichen Probleme und trifft keine unbegründete Entscheidung über verpflichtende Benachrichtigungen.  

### REQ-011 – The New Login

| Bewertungskriterium | Human | AI |
|---|:---:|:---:|
| Fachliche Angemessenheit | 5 | 2 |
| Eindeutigkeit und Verständlichkeit | 5 | 4 |
| Vollständigkeit und Überprüfbarkeit | 4 | 2 |
| Umgang mit Annahmen | 5 | 2 |
| Abstimmung und Konflikte | 5 | 1 |
| **Gesamt** | **24/25** | **11/25** |

**Begründung:**
Die Human Version berücksichtigt die verbindliche Vorgabe der IT-Abteilung, dass das bestehende Authentifizierungssystem verwendet werden muss. Dadurch wird die ursprüngliche Anforderung korrigiert und klar festgelegt, dass keine zusätzliche Benutzerverwaltung oder ein separater Login eingerichtet werden darf.  
Die AI Version formuliert die Anforderung zwar verständlich und lösungsneutral, berücksichtigt dabei jedoch nicht die bereits bekannte technische Rahmenbedingung. Stattdessen wird die Nutzung bestehender Hochschulzugänge als offene Frage behandelt, obwohl diese Entscheidung bereits getroffen wurde.  
Auch bei der Human Version sind technische Details zur Integration und Berechtigungsverwaltung noch offen.  
**Fazit:** Die Human Version ist diesmal besser, da sie die verbindliche IT-Vorgabe berücksichtigt und den Widerspruch der ursprünglichen Anforderung behebt. Die AI Version erkennt zwar das Problem einer unnötigen zusätzlichen Benutzerverwaltung, ignoriert jedoch eine bereits festgelegte Rahmenbedingung.  

