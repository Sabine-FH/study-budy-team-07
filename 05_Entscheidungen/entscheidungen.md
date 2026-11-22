# Entscheidungen – Mission 04 (Anforderungskatalog)

## E-001 Quellen: nur Mission 01–03, Rohliste 1:1
**Entscheidung:** In die Rohliste kommen alle Aussagen aus Mission 01–03. Projektauftrag und LV-Inhalte werden nicht als Quelle verwendet.  
**Grund:** Die Aufgabe verlangt „alle Aussagen aus den Missionen 01 bis 03“.

## E-002 ID-Schema nach Ebene
**Entscheidung:** IDs nach Ebene, dreistellig: BR-001 = Business, UR-001 = User, SR-001 = System. Aussagen der Rohliste (RAW-001), offene Fragen (OQ-001) und Entscheidungen (E-001) sind ebenfalls dreistellig nummeriert.  
**Grund:** Keine Verwechslung mit REQ-001 bis REQ-015 aus Mission 3. Die Ebene ist an der ID sofort erkennbar, das erleichtert die Prüfung des Bezugs.  
**Alternative:** REQ ab 101.

## E-003 Stakeholder-Erwartungen als Quelle für Business und User
**Entscheidung:** Die Erwartungen aus Mission 2 werden als Business- bzw. User-Anforderungen übernommen.  
**Grund:** In Mission 1 und 3 wurden fast nur Systemanforderungen formuliert. Business- und User-Anforderungen stammen von Stakeholder:innen, und deren Erwartungen wurden in Mission 2 erhoben.

## E-004 Präzisierung mit Zielwerten
**Entscheidung:** Fünf Qualitätsanforderungen wurden aus Aussagen der Rohliste abgeleitet und mit einem Zielwert präzisiert:
| ID | Abgeleitet aus | Herkunft des Zielwerts |
|---|---|---|
| SR-010 | RAW-050 (Mission 2, Plot Twist, Berechtigungen) | Beispielwert des Teams |
| SR-013 | RAW-053 (Mission 3, REQ-002, „schnell“) | Mission 4, Teil C |
| SR-014 | RAW-053 (Mission 3, REQ-002, „intuitiv, benutzerfreundlich“) | Beispielwert des Teams |
| SR-015 | RAW-061 (Mission 3, REQ-010) | Mission 4, Teil C |
| SR-016 | RAW-033 und RAW-048 (Mission 2, Erwartungen IT und Plot Twist, Verfügbarkeit) | Beispielwert des Teams |

**Grund:** In Mission 01–03 gibt es keine abgestimmten Zielwerte, die Prüfliste verlangt aber mindestens fünf Qualitätsanforderungen mit Zahl.
**Wichtig:** Alle Zielwerte sind Beispielwerte und müssen in der Elicitation mit den Stakeholder:innen validiert werden (siehe OQ-018).

## E-005 Status
**Entscheidung:** Fast alle Anforderungen haben den Status „Entwurf“.
**Grund:** Es wurden noch keine Stakeholder:innen befragt. Die Interviews und Workshops aus Mission 1 sind nur geplant.
**Ausnahmen:**
- SR-005 „Abgestimmt“: verbindliche Vorgabe der IT (Mission 2, Plot Twist)
- SR-006 „Verworfen“: widerspricht dieser Vorgabe (Mission 3, REQ-011)
- SR-001 „Verworfen“: ersetzt durch SR-011 (siehe E-008)  

## E-006 Grenzfälle im Katalog
**Entscheidung:** UR-008, SR-002, SR-003 und SR-004 bleiben als Entwurf im Katalog, obwohl sie in Mission 3 als INVESTIGATE bewertet wurden.
**Grund:** Die Funktion selbst ist klar, offen sind nur Details. Die offenen Punkte stehen in der Liste offener Fragen.  

## E-007 Unklare Aussagen
**Entscheidung:** Unklare oder widersprüchliche Aussagen kommen nicht in den Katalog, sondern auf die Liste offener Fragen (OQ-001 bis OQ-018).  
**Beispiele:** REQ-001, 004, 005, 006, 008, 009, 012, 013, 015 und REQ-003d aus Mission 3. Die Anforderungen REQ-001 bis 003 aus Mission 1 entsprechen REQ-001, 005 und 006 aus Mission 3.  

## E-008 Anpassung nach Team-Review
**Entscheidung:**
- SR-011 wurde durch die Neuformulierung aus Teil C ersetzt.
- SR-012 wurde aus dem Katalog entfernt und als OQ-019 aufgenommen.
- SR-001 wurde auf „Verworfen“ gesetzt, weil die neue SR-011 sie ersetzt.

**Grund:** SR-011 und SR-012 waren die ursprünglichen Sätze aus Mission 3 (REQ-010 und REQ-014), die wir in Teil C bzw. in der Quality Review selbst als unklar („relevant“) oder nicht prüfbar („auf allen Geräten vollständig“) bewertet haben. SR-001 hätte sich mit der neuen SR-011 überschnitten und enthält den unklaren Begriff „bevorstehend“. Der Katalog soll unseren eigenen Analysen nicht widersprechen und keine doppelten Anforderungen enthalten.
**Hinweis:** Die ID SR-012 ist nicht mehr vergeben. Die übrigen IDs bleiben unverändert, damit alle Verweise stimmen.
