### **Final Requirements – Study Buddy**

**1. Einleitung**

In diesem Dokument werden fünf ausgewählte Anforderungen für den Study Buddy abschließend überarbeitet. Als Grundlage dienen die Ergebnisse aus Teil 3 sowie der Vergleich zwischen der Human- und der AI-Version.

Bei der Überarbeitung wurden sowohl die festgestellten Qualitätsmängel als auch die Verbesserungsvorschläge aus beiden Versionen berücksichtigt. Dabei wurde nicht automatisch die jeweils besser bewertete Formulierung übernommen. Entscheidend war, ob sie fachlich sinnvoll ist und mit den bereits bekannten Rahmenbedingungen des Projekts übereinstimmt.

Wenn wichtige Informationen noch fehlen, wird die betreffende Anforderung nicht künstlich vervollständigt. Stattdessen wird festgehalten, was noch geklärt werden muss. So wird vermieden, dass Annahmen oder Vorschläge bereits als verbindliche Anforderungen dargestellt werden.

### **2. Finale Anforderungen**
### **REQ-001 – The Seven-Day Rule**

**Ursprüngliche Anforderung:**

Das System muss Studierende automatisch benachrichtigen, wenn sie sieben Tage lang nicht im Online Campus aktiv waren.

**Finaler Status: INVESTIGATE**

**Finale Entscheidung:**

Die ursprüngliche Sieben-Tage-Regel wird vorerst nicht als verbindliche Anforderung übernommen. Es muss zunächst geklärt werden, woran ein möglicher Unterstützungsbedarf überhaupt erkannt werden kann und ob eine Benachrichtigung in solchen Situationen sinnvoll ist.

Als vorläufige Formulierung für die weitere Untersuchung dient:
Das System soll Studierende bei zuvor definierten Anzeichen für möglichen Unterstützungsbedarf unterstützen können.

Damit wird der ursprüngliche Gedanke einer frühzeitigen Unterstützung beibehalten, ohne bereits festzulegen, dass fehlende Aktivität im Online Campus automatisch eine Benachrichtigung auslösen muss.

**Begründung:**

Die Human-Version geht hier in die richtige Richtung, weil sie die unbegründete Sieben-Tage-Regel nicht einfach übernimmt. Allerdings ist auch die dort vorgeschlagene Formulierung noch nicht ausreichend konkret. Es bleibt offen, welche Anzeichen auf Unterstützungsbedarf hindeuten und wie das System darauf reagieren soll.

Die KI-Version liefert zwar eine genauere Formulierung und erste Akzeptanzkriterien, hält aber weiterhin an den sieben Tagen fest. Da weder die fachliche Begründung für diesen Zeitraum noch die Definition von Aktivität geklärt sind, wäre es nicht sinnvoll, diese Vorgabe bereits als verbindlich festzulegen.

**Noch zu klären ist:**

 - Welche Situationen können tatsächlich auf einen Unterstützungsbedarf hinweisen?
 - Wie werden Aktivitäten außerhalb des Online Campus berücksichtigt?
 - Welche Daten dürfen für die Einschätzung verwendet werden?
 - Wann ist eine Benachrichtigung sinnvoll und welche Form sollte sie haben?
 - Welche Rolle übernehmen Studierende und Lehrende bei der Einschätzung des Unterstützungsbedarfs?
 - Die Annahme, dass fehlende Aktivität im Online Campus automatisch auf Unterstützungsbedarf hinweist, ist weiterhin ungeklärt.

### **REQ-002 – Fast and Friendly**

**Ursprüngliche Anforderung:**

Der Study Buddy muss schnell, intuitiv und besonders benutzerfreundlich sein.

**Finaler Status: INVESTIGATE**

**Finale Entscheidung:**

Die Anforderung kann derzeit noch nicht ausreichend konkret formuliert werden. Zunächst müssen die wichtigsten Nutzungssituationen und die Erwartungen der Studierenden untersucht werden.

Dabei soll insbesondere geklärt werden, welche Aufgaben mit dem Study Buddy erledigt werden sollen und woran eine einfache Bedienung erkennbar ist.

**Begründung:**

Die Human-Version vereinfacht die ursprüngliche Formulierung, indem sie den Study Buddy als einfach und verständlich bedienbar beschreibt. Das ist zwar leichter lesbar, löst aber das eigentliche Problem nicht: Auch diese Begriffe sind subjektiv und können ohne weitere Festlegung nicht objektiv überprüft werden. Außerdem wird der ursprüngliche Aspekt der Geschwindigkeit nicht mehr berücksichtigt.

Die KI-Version zeigt genauer auf, welche Informationen für eine überprüfbare Anforderung fehlen. Dazu gehören konkrete Nutzungsszenarien sowie messbare Kriterien für die Bedienbarkeit und Leistung. Dieser Ansatz wird für die weitere Untersuchung übernommen. Konkrete Zielwerte werden jedoch noch nicht festgelegt, da dafür eine fachliche Grundlage fehlt.

**Noch zu klären ist:**

- Welche Aufgaben sollen Studierende mit dem Study Buddy erledigen können?
- Welche Nutzungssituationen sind besonders wichtig?
- Was verstehen Studierende unter einer einfachen und verständlichen Bedienung?
- Bei welchen Funktionen spielt die Reaktionsgeschwindigkeit eine besondere Rolle?
- Wie kann die erfolgreiche Nutzung objektiv überprüft werden?

Erst wenn diese Punkte geklärt sind, können konkrete und überprüfbare Kriterien für die Benutzerfreundlichkeit und Geschwindigkeit festgelegt werden.

### **REQ-003 – The All-in-One Feature**

**Ursprüngliche Anforderung:**

Das System muss bevorstehende Abgaben anzeigen, personalisierte Erinnerungen versenden, Lernfortschritte analysieren und Lehrende über Schwierigkeiten informieren.

**Finaler Status: INVESTIGATE**

**Finale Entscheidung:**

Die ursprüngliche Anforderung umfasst vier unterschiedliche Funktionen, die getrennt betrachtet werden müssen. Für die weitere Untersuchung werden daher folgende Entwürfe festgehalten:

| ID | Vorläufiger Anforderungsentwurf | Noch zu klären |
| :--- | :--- | :--- |
| REQ-003a | Das System soll Studierenden ihre bevorstehenden Abgaben anzeigen können. | Was gilt als bevorstehend? Woher stammen die Daten und wie werden sie aktualisiert? |
| REQ-003b | Das System soll personalisierte Erinnerungen an Studierende versenden kön | Nach welchen Regeln werden Erinnerungen erstellt und versendet? |
| REQ-003c | Das System soll den Lernfortschritt von Studierenden analysieren können. | Welche Daten und Messgrößen werden verwendet und welchem Zweck dient die Analyse? |
| REQ-003d | Das System soll Lehrende über mögliche Schwierigkeiten von Studierenden informieren können. | Was gilt als Schwierigkeit und welche Informationen dürfen an Lehrende weitergegeben werden? |

Bei diesen Formulierungen handelt es sich um vorläufige Entwürfe. Es ist noch nicht entschieden, ob alle vier Funktionen tatsächlich benötigt werden oder umgesetzt werden sollen.

**Begründung:**

Die Human-Version konzentriert sich auf die Anzeige bevorstehender Abgaben. Dadurch wird die Anforderung übersichtlicher, allerdings bleiben die drei anderen ursprünglichen Funktionen ohne eigene Ausarbeitung.

Die KI-Version schlägt vor, alle vier Funktionen getrennt zu betrachten. Das ist sinnvoll, da sie unterschiedliche Ziele verfolgen und jeweils eigene fachliche und technische Voraussetzungen haben. Besonders bei der Analyse des Lernfortschritts und der Weitergabe von Informationen an Lehrende müssen auch Datenschutz und Zugriffsberechtigungen berücksichtigt werden.

Deshalb wird die Aufteilung aus der KI-Version übernommen. Gleichzeitig bleibt die fachliche Zurückhaltung der Human-Version erhalten: Die Funktionen werden zunächst untersucht und nicht automatisch als bestätigte Anforderungen behandelt.

**Noch zu klären ist:**

- Welche der vier Funktionen werden von den Studierenden tatsächlich benötigt?
- Sind die erforderlichen Informationen bereits in bestehenden Systemen vorhanden?
- Wie aktuell und zuverlässig sind diese Daten?
- Was bedeutet eine personalisierte Erinnerung konkret?
- Welche Daten dürfen für die Analyse des Lernfortschritts verwendet werden?
- Unter welchen Voraussetzungen dürfen Informationen über mögliche Schwierigkeiten an Lehrende weitergegeben werden?

Insbesondere bei REQ-003c und REQ-003d müssen Zweck, Datenverarbeitung und Zugriffsberechtigungen vor einer möglichen Umsetzung geklärt werden.

### **REQ-008 – No Exceptions**

**Ursprüngliche Anforderung:**

Das System muss alle Studierenden unabhängig von ihren Einstellungen über kritische Studienereignisse benachrichtigen.

**Finaler Status: RECONSIDER**

**Finale Entscheidung:**

Die ursprüngliche Vorgabe, alle Studierenden unabhängig von ihren persönlichen Einstellungen zu benachrichtigen, wird vorerst nicht übernommen.

Zunächst muss festgelegt werden, welche Studienereignisse tatsächlich als kritisch gelten und ob es Gründe gibt, bestimmte Benachrichtigungen verpflichtend zu versenden.

Als möglicher Ansatz für eine spätere Formulierung kann dienen:
Das System soll Studierende über für sie relevante Studienereignisse gemäß noch festzulegenden Benachrichtigungsregeln informieren können.

Diese Formulierung ist noch nicht als endgültige Anforderung zu verstehen. Insbesondere ist damit nicht entschieden, ob bestimmte Benachrichtigungen verpflichtend sein müssen.

**Begründung:**

Sowohl die Human- als auch die KI-Version erkennen, dass die ursprüngliche Anforderung wichtige Definitionen vermissen lässt. Die Human-Version berücksichtigt zusätzlich den Zusammenhang mit REQ-007, wonach Studierende alle Benachrichtigungen deaktivieren können sollen.

Die KI-Version geht ausführlicher auf mögliche Ausnahmen, Empfängerkriterien und organisatorische beziehungsweise rechtliche Grundlagen ein. Außerdem wird richtigerweise darauf hingewiesen, dass ein möglicher Konflikt mit der Selbstbestimmung der Studierenden noch kein nachgewiesener Stakeholderkonflikt ist.

Für die finale Entscheidung werden beide Ansätze berücksichtigt. Die verpflichtende Benachrichtigung unabhängig von den persönlichen Einstellungen wird zunächst infrage gestellt. Gleichzeitig muss REQ-008 gemeinsam mit REQ-007 betrachtet werden, damit am Ende keine widersprüchlichen Benachrichtigungsregeln entstehen.

**Noch zu klären ist:**

- Welche Studienereignisse gelten tatsächlich als kritisch?
- Für welche Studierenden sind diese Ereignisse relevant?
- Welche Benachrichtigungen müssen gegebenenfalls verpflichtend sein?
- Welche Einflussmöglichkeiten sollen Studierende auf ihre Benachrichtigungseinstellungen haben?
- Welche organisatorischen und rechtlichen Grundlagen gelten?
- Wie können REQ-007 und REQ-008 miteinander vereinbart werden?

Ein tatsächlicher Konflikt zwischen den Stakeholdern ist bisher nicht nachgewiesen. Die unterschiedlichen Anforderungen müssen jedoch noch abgestimmt werden.

### **REQ-011 – The New Login**

**Ursprüngliche Anforderung:**

Studierende müssen für den Study Buddy ein separates Benutzerkonto mit eigenem Passwort erstellen.

**Finaler Status: REWRITE**

**Finale Anforderung:**

Der Study Buddy muss das bereits bestehende Authentifizierungssystem der Hochschule verwenden. Eine zusätzliche Benutzerverwaltung oder ein separater Login dürfen nicht eingerichtet werden.

**Begründung:**

Bei dieser Anforderung liegt bereits eine verbindliche technische Rahmenbedingung aus dem Projekt vor: Der Study Buddy muss das bestehende Authentifizierungssystem der Hochschule verwenden.

Die Human-Version berücksichtigt diese Vorgabe und korrigiert damit die ursprüngliche Forderung nach einem separaten Benutzerkonto.

Die KI-Version schlägt hingegen eine allgemeine, lösungsneutrale Authentifizierungsanforderung vor. Dabei wird die Nutzung bestehender Hochschulzugänge erneut als offene Frage behandelt. Das ist in diesem Fall nicht passend, da die entsprechende Rahmenbedingung bereits feststeht.

Deshalb wird die Human-Version als Grundlage für die finale Anforderung übernommen. Offen bleiben lediglich die technischen Details der Integration und die Verwaltung der Zugriffsberechtigungen.

**Noch zu klären ist:**

- Welche Schnittstellen und Integrationsmöglichkeiten stellt das bestehende Authentifizierungssystem bereit?
- Wie werden Benutzerrollen und Zugriffsberechtigungen für den Study Buddy geregelt?
- Welche zusätzlichen Sicherheitsanforderungen müssen bei der Integration berücksichtigt werden?
- Welche Auswirkungen hat die Integration auf den bestehenden Online Campus?

Die Verwendung des bestehenden Authentifizierungssystems ist eine festgelegte Rahmenbedingung. Die konkrete technische Umsetzung muss noch mit den zuständigen Stellen geklärt werden.

### **3. Zusammenfassung der finalen Entscheidungen**
   
| Anforderung | Status | Ergebnis |
| :--- | :--- | :--- |
| REQ-001 – The Seven-Day Rule | INVESTIGATE | Unterstützungsbedarf und geeignete Anzeichen müssen zunächst geklärt werden. |
| REQ-002 – Fast and Friendly | INVESTIGATE | Nutzungssituationen und überprüfbare Qualitätskriterien fehlen. |
| REQ-003 – The All-in-One Feature | INVESTIGATE | Die vier Funktionen werden getrennt untersucht und sind noch nicht bestätigt. |
| REQ-008 – No Exceptions | RECONSIDER | Verpflichtende Benachrichtigungen unabhängig von den Einstellungen sind noch nicht begründet. |
| REQ-011 – The New Login | REWRITE | Das bestehende Authentifizierungssystem der Hochschule muss verwendet werden. |

### **4. Fazit**

Die Überarbeitung zeigt, dass die Human- und die KI-Version unterschiedliche Stärken haben. Die Human-Version berücksichtigt teilweise bereits bekannte Projektentscheidungen und formuliert offene Punkte eher zurückhaltend. Die KI-Version liefert dafür häufig eine ausführlichere Analyse und macht fehlende Informationen deutlicher sichtbar.

Für die finale Fassung wurden deshalb die sinnvollsten Aspekte aus beiden Versionen übernommen. Bei REQ-003 wurde beispielsweise die Aufteilung der KI-Version verwendet, während bei REQ-011 die Human-Version ausschlaggebend war, da sie die bereits festgelegte technische Rahmenbedingung berücksichtigt.

Nicht alle Anforderungen konnten abschließend formuliert werden. Bei vier der fünf Anforderungen fehlen noch fachliche Informationen oder notwendige Abstimmungen. Diese Punkte bleiben bewusst offen, anstatt unbegründete Entscheidungen zu treffen.

Damit bildet das Dokument eine nachvollziehbare Grundlage für die weitere Anforderungsanalyse und die spätere Abstimmung mit den relevanten Stakeholdern.
