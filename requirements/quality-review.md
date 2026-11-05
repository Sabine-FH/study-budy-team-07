### Quality Review – Digital Study Buddy

**Mission 03 – Teil 2: Find the Defect**

Wir haben die 15 Anforderungsentwürfe REQ-001 bis REQ-015 zuerst einzeln geprüft, dann untereinander verglichen und auf Widersprüche geprüft. Grundlage ist die Requirements Quality Checklist:

- **Inhalt - Beschreiben wir das richtig? :** Vollständigkeit, Korrektheit/Adäquatheit, Notwendigkeit, keine vorzeitigen Entwurfsentscheidungen, Konsistenz, Überprüfbarkeit
- **Dokumentation - Beschreiben wir es verständlich? :** Verständlichkeit, Eindeutigkeit (Requirements Smells, mehrere Sachverhalte in einem Satz), Dokumentationsregeln
- **Abgestimmtheit - Ist es mit den beteiligten geklärt? :** Stakeholder:innen-Einbeziehung, Konfliktklärung, Abstimmung nach Änderungen

Viele Anforderungen haben mehr als ein Problem. Wir nennen deshalb immer zuerst das wichtigste und erwähnen die anderen kurz dazu. Lösungen schreiben wir hier noch keine, es geht erstmal nur darum, die Fehler zu finden. Wo uns die Informationen fehlen, schreiben wir die offenen Punkte als Fragen auf. In Klammern steht jeweils, wen wir dazu fragen müssten.

---

**REQ-001 – The Seven-Day Rule**
> „Das System muss Studierende automatisch benachrichtigen, wenn sie sieben Tage lang nicht im Online Campus aktiv waren.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Korrektheit/Adäquatheit
- **Fehlerbeschreibung:** Die Anforderung ist präzise, beruht aber auf einer unbelegten Annahme: dass fehlende Aktivität im Online Campus Unterstützungsbedarf anzeigt. Studierende lernen aber auch am Wochenende, offline mit heruntergeladenen Materialien oder nur vor Abgaben. Die sieben Tage sind nicht begründet. *Weitere Mängel:* „Aktiv“ ist nicht wirklich definiert (Dokumentation – Eindeutigkeit). Es ist kein Bedarf nachgewiesen (Inhalt – Notwendigkeit).  
- **Mögliche Konsequenz:** Fehlalarme bei selbstständig Lernenden, Benachrichtigungen werden ignoriert oder abbestellt. Studierende, die zwar eingeloggt sind, aber nicht vorankommen, werden übersehen.
- **Fehlende Informationen:**
  - Erzählen Sie von einer konkreten Situation, in der Sie bemerkt haben, dass ein:e Studierende:r Unterstützung braucht. Woran haben Sie es erkannt? (Lehrendenvertretung, Studiengangsleitung)
  - Welche Benutzer:innenaktionen lassen sich überhaupt verlässlich messen? (IT & Online-Campus-Team)
  - Welche Ausnahmen gelten, z. B. Ferien, Krankheit, Dienstreisen? (Studierendenvertretung, Lehrendenvertretung)

**REQ-002 – Fast and Friendly**
> „Der Study Buddy muss schnell, intuitiv und besonders benutzerfreundlich sein.“

- **Qualitätsaspekt:** Dokumentation
- **Qualitätskriterium:** Eindeutigkeit (Requirements Smells)
- **Fehlerbeschreibung:** „Schnell“ und „intuitiv“ sind Requirements Smells, „besonders benutzerfreundlich“ ebenso. Für wen, bei welcher Aufgabe und unter welchen Bedingungen das gelten soll, bleibt offen. *Weitere Mängel:* Es gibt keine Akzeptanzkriterien (Inhalt – Überprüfbarkeit). Performance und Benutzbarkeit sind zwei Anforderungen in einem Satz.
- **Mögliche Konsequenz:** Die Anforderung ist nicht abnahmefähig, jede Umsetzung lässt sich als erfüllt oder nicht erfüllt argumentieren. Konflikte bei der Abnahme sind absehbar.
- **Fehlende Informationen:**
  - Bei welchen Tätigkeiten im Study Buddy ist Geschwindigkeit für Studierende wirklich wichtig? (Studierendenvertretung)
  - Welche Antwortzeiten sind technisch realistisch? (IT & Online-Campus-Team)
  - Mit welchem Verfahren und an welchen Aufgaben soll Benutzbarkeit nachgewiesen werden, auch für Studierende mit Beeinträchtigungen? (Expert:innen für Barrierefreiheit und Inklusion)

**REQ-003 – The All-in-One Feature**
> „Das System muss bevorstehende Abgaben anzeigen, personalisierte Erinnerungen versenden, Lernfortschritte analysieren und Lehrende über Schwierigkeiten informieren.“

- **Qualitätsaspekt:** Dokumentation
- **Qualitätskriterium:** Eindeutigkeit (mehrere Sachverhalte in einem Satz)
- **Fehlerbeschreibung:** Vier eigenständige Funktionen mit unterschiedlichen Prioritäten, Bedingungen und Berechtigungen stehen in einem Satz. Zusätzlich sind „bevorstehend“, „personalisiert“, „analysieren“ und „Schwierigkeiten“ unbestimmt. *Weitere Mängel:* Die Information an Lehrende betrifft die Privatsphäre der Studierenden, deren Einbeziehung ist nicht erkennbar (Abgestimmtheit).
- **Mögliche Konsequenz:** Der Erfüllungsstatus ist nicht feststellbar (was gilt, wenn drei von vier Teilen umgesetzt sind?). Getrennte Priorisierung ist nicht möglich, und die datenschutzsensible Teilfunktion wird unbemerkt mitbeauftragt.
- **Fehlende Informationen:**
  - Welche Quelle und Priorität hat jede der vier Teilfunktionen? (Studiengangsleitung, Studierendenvertretung)
  - Was gilt als „Schwierigkeit“, und wie unterscheidet sich Lernfortschritt zwischen Lehrveranstaltungen? (Lehrendenvertretung)
  - Dürfen Lehrende über Schwierigkeiten einzelner Studierender informiert werden? (Datenschutz & Informationssicherheit, Studierendenvertretung)

**REQ-004 – The Perfect Prediction**
> „Das System muss zuverlässig erkennen, welche Studierenden ihr Studium nicht erfolgreich abschließen werden.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Korrektheit/Adäquatheit
- **Fehlerbeschreibung:** Gefordert ist eine sichere Vorhersage, die nicht möglich ist. Studienerfolg hängt von Faktoren ab, die das System nicht kennt, etwa Beruf, Familie, Gesundheit oder auch Finanzierung. Was nach der Erkennung passieren soll, ist nicht beschrieben. *Weitere Mängel:* „Zuverlässig“ ist ohne Zielwert, und die Erfüllung zeigt sich erst Jahre später (Inhalt – Überprüfbarkeit).
- **Mögliche Konsequenz:** Falsche Einstufungen können zu Stigmatisierung und Demotivation führen. Dazu kommen rechtliche und ethische Risiken durch Profiling.
- **Fehlende Informationen:**
  - Welches Problem soll gelöst werden, und wer hat die Anforderung eingebracht? (Studiengangsleitung)
  - Was passiert mit dem Ergebnis, und wer erhält es? (Studiengangsleitung, Studierendenvertretung)
  - Ist eine solche automatisierte Einstufung zulässig? (Datenschutz & Informationssicherheit)

**REQ-005 – Monday Morning**
> „Alle Studierenden müssen jeden Montag um 08:00 Uhr eine personalisierte Fortschrittsübersicht per E-Mail erhalten.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Notwendigkeit
- **Fehlerbeschreibung:** Es ist nicht erkennbar, welchen Bedarf die Übersicht erfüllt. Sie kann hilfreich sein, Studierende können eine weitere wöchentliche Nachricht aber auch als störend empfinden oder ihren Fortschritt lieber selbst abrufen. *Weitere Mängel:* E-Mail, Montag und 08:00 Uhr sind Lösungsentscheidungen vor der Bedarfsklärung (Inhalt – keine vorzeitigen Entwurfsentscheidungen). Für berufstätige Studierende ist der Zeitpunkt möglicherweise ungeeignet. „Alle müssen erhalten“ widerspricht REQ-007.
- **Mögliche Konsequenz:** Eine Funktion ohne Nutzen wird gebaut und als Spam wahrgenommen. Bessere Alternativen werden ausgeschlossen.
- **Fehlende Informationen:**
  - Erzählen Sie von der letzten Situation, in der Sie den Überblick über Ihren Studienstand verloren haben. Was hätte geholfen? (Studierendenvertretung)
  - Was soll eine Übersicht zeigen? (Studierendenvertretung)
  - Ist die Übersicht nach REQ-007 abbestellbar? (Studierendenvertretung, Studienadministration)

**REQ-006 – The Missing Definition**
> „Wenn ein kritischer Lernrückstand vorliegt, muss das System geeignete Maßnahmen einleiten.“

- **Qualitätsaspekt:** Dokumentation
- **Qualitätskriterium:** Eindeutigkeit und Verständlichkeit
- **Fehlerbeschreibung:** Bedingung und Reaktion sind beide undefiniert. Für „kritischer Lernrückstand“ fehlen Bezugsgröße und Schwelle, „geeignete Maßnahmen“ ist ein Smell und überlässt die Entscheidung der Umsetzung. *Weitere Mängel:* Es lässt sich kein Testfall ableiten (Inhalt – Überprüfbarkeit). Würde etwa die Studiengangsleitung informiert, wären Studierende, Datenschutz und Lehrende nicht abgestimmt (Abgestimmtheit).
- **Mögliche Konsequenz:** Das Entwicklungsteam trifft fachliche Entscheidungen, für die es gar nicht zuständig ist. Die Maßnahmen bleiben wirkungslos oder werden übergriffig.
- **Fehlende Informationen:**
  - Was ist ein „kritischer Lernrückstand“, und wer legt das fest? (Studiengangsleitung, Lehrendenvertretung)
  - Welche Maßnahmen darf das System selbst auslösen, und wann braucht es eine Person? (Studiengangsleitung, Datenschutz & Informationssicherheit)
  - Gibt es bei der Studiengangsleitung die Kapazität, auf solche Fälle zu reagieren? (Studiengangsleitung)

**REQ-007 – The Notification Paradox**
> „Studierende müssen sämtliche Benachrichtigungen jederzeit deaktivieren können.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Konsistenz (Konflikt mit REQ-008)
- **Fehlerbeschreibung:** Die Anforderung widerspricht direkt REQ-008, wonach Benachrichtigungen unabhängig von den Einstellungen zugestellt werden müssen, und ebenso REQ-005. „Sämtliche“ und „jederzeit“ lassen keine Ausnahmen zu. *Weitere Mängel:* Was als „Benachrichtigung“ gilt, ist nicht definiert. Der Konflikt muss von den Stakeholder:innen geklärt werden (Abgestimmtheit – Konfliktklärung).
- **Mögliche Konsequenz:** Das Entwicklungsteam muss selbst entscheiden, wie es den Widerspruch auflöst, obwohl das gar nicht seine Entscheidung ist. Studierende bekommen trotz Abmeldung Nachrichten oder verpassen wichtige Informationen.
- **Fehlende Informationen:**
  - Welche Arten von Benachrichtigungen soll es überhaupt geben?(Studierendenvertretung, Studienadministration)
  - Welche davon sollen nicht abschaltbar sein, und wer entscheidet das? (Studierendenvertretung, Studienadministration)

**REQ-008 – No Exceptions**
> „Das System muss alle Studierenden unabhängig von ihren Einstellungen über kritische Studienereignisse benachrichtigen.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Konsistenz (Konflikt mit REQ-007)
- **Fehlerbeschreibung:** „Unabhängig von ihren Einstellungen“ hebt REQ-007 auf. Eine bewusst entschiedene, begründete Ausnahme ist nicht erkennbar. *Weitere Mängel:* „Kritische Studienereignisse“ ist nicht definiert und kann beliebig ausgeweitet werden (Dokumentation – Eindeutigkeit).
- **Mögliche Konsequenz:** Ein ungelöster Widerspruch bleibt in der Spezifikation. Bei weiter Auslegung entsteht eine Benachrichtigungsflut trotz Abmeldung.
- **Fehlende Informationen:**
  - Welche Ereignisse gelten als „kritisch“, und wer legt das fest? (Studienadministration)
  - Werden diese Ereignisse bereits über andere Kanäle der Hochschule kommuniziert? (Studienadministration)

**REQ-009 – The Secret Dashboard**
> „Die Studiengangsleitung muss jederzeit auf sämtliche individuellen Lernaktivitäten aller Studierenden zugreifen können.“

- **Qualitätsaspekt:** Abgestimmtheit
- **Qualitätskriterium:** Stakeholder:innen-Einbeziehung und Konfliktklärung
- **Fehlerbeschreibung:** Die Anforderung bildet nur das Interesse der Studiengangsleitung ab. Studierende möchten selbst entscheiden, wer Informationen über ihr Lernverhalten erhält, und die IT braucht klare Vorgaben für Zugriffsrechte. Dieser Konflikt („Unterstützen oder überwachen?“), den wir schon in unserer Stakeholder:innen-Analyse festgehalten haben, ist nicht geklärt. *Weitere Mängel:* Der Zweck ist unklar (Inhalt – Notwendigkeit). Außerdem sollen laut Datenschutz nur so viele Daten verwendet werden, wie für einen Zweck wirklich nötig sind. Ein Zugriff auf alles und jederzeit passt dazu nicht.
- **Mögliche Konsequenz:** Rechtliche Risiken. Studierende fühlen sich überwacht und meiden den Study Buddy, damit verliert das System seinen Nutzen.
- **Fehlende Informationen:**
  - Welchen Bedarf hat die Studiengangsleitung, und würden zusammengefasste, anonymisierte Daten reichen? (Studiengangsleitung)
  - Welche Einflussmöglichkeiten sollen Studierende auf ihre Daten haben? (Studierendenvertretung, Datenschutz & Informationssicherheit)
  - Wer darf auf welche Daten zugreifen? (Datenschutz & Informationssicherheit)

**REQ-010 – The Invisible Source**
> „Der Study Buddy muss alle relevanten Informationen zu Lehrveranstaltungen automatisch aus den bestehenden Systemen übernehmen.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Vollständigkeit
- **Fehlerbeschreibung:** Weder die Quellsysteme noch die benötigten Informationen sind benannt. „Alle relevanten“ ist nicht abgegrenzt. *Weitere Mängel:* Die Anforderung setzt voraus, dass die Quelldaten vollständig und widerspruchsfrei sind. Sind Fristen in den Quellsystemen veraltet oder widersprüchlich, wird dieses Problem nur weitergereicht (Inhalt – Korrektheit).
- **Mögliche Konsequenz:** Aufwand und Machbarkeit sind nicht schätzbar. Fehlerhafte Fristen werden ungeprüft weitergegeben, Abgaben werden versäumt.
- **Fehlende Informationen:**
  - Welche Systeme und Daten sind gemeint, und gibt es dafür Schnittstellen? (IT & Online-Campus-Team)
  - Wer ist für die Aktualität der Daten verantwortlich, und welche Quelle gilt bei Widersprüchen? (Studienadministration)

**REQ-011 – The New Login**
> „Studierende müssen für den Study Buddy ein separates Benutzerkonto mit eigenem Passwort erstellen.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Konsistenz mit verbindlichen Rahmenbedingungen
- **Fehlerbeschreibung:** Die Anforderung widerspricht der verbindlichen Vorgabe aus dem Plot Twist, das bestehende Authentifizierungssystem der Hochschule zu verwenden. Anders als diese begründete Vorgabe legt REQ-011 eine Lösung ohne Begründung fest. *Weitere Mängel:* Kein Bedarf für ein eigenes Konto ist dokumentiert (Inhalt – Notwendigkeit).
- **Mögliche Konsequenz:** Ablehnung durch die IT und Nacharbeit. Zusätzliche Passwörter erhöhen das Sicherheitsrisiko und die Nutzungshürde.
- **Fehlende Informationen:**
  - Woher stammt die Anforderung, und steckt ein legitimer Bedarf dahinter (z. B. Nutzer:innen ohne Hochschulkonto)?(IT & Online-Campus-Team)
  - Welche Benutzerinformationen und Rollen stellt das bestehende System bereit? (IT & Online-Campus-Team)

**REQ-012 – The Universal Recommendation**
> „Das System muss jeder studierenden Person jederzeit die optimale individuelle Lernstrategie empfehlen.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Korrektheit/Adäquatheit
- **Fehlerbeschreibung:** Eine objektiv „optimale“ Lernstrategie gibt es nicht, denn sie hängt von Vorwissen, Lebenssituation und verfügbarer Zeit ab, die das System nicht kennt. Ein Bedarf an Strategieempfehlungen ist nicht belegt. *Weitere Mängel:* „Optimal“ ist ein Smell und nicht messbar (Inhalt – Überprüfbarkeit).
- **Mögliche Konsequenz:** Unrealistische Erwartungen, nicht abnahmefähig. Unpassende Empfehlungen schaden dem Lernerfolg und der Glaubwürdigkeit des Systems.
- **Fehlende Informationen:**
  - Erzählen Sie von einer Situation, in der Sie beim Lernen nicht weitergekommen sind. Was hat Ihnen damals gefehlt? (Studierendenvertretung)
  - Wer verantwortet fachlich die Inhalte von Lernempfehlungen? (Lehrendenvertretung)

**REQ-013 – The Silent Change**
> „Änderungen an Abgabeterminen müssen automatisch übernommen werden, ohne dass eine erneute Bestätigung erforderlich ist.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Korrektheit/Adäquatheit
- **Fehlerbeschreibung:** Eine Terminänderung wird wie ein reiner Datenabgleich behandelt. Für Studierende ist sie aber ein relevantes Ereignis, besonders wenn ein Termin vorverlegt wird. Bei stiller Übernahme bemerken sie die Änderung möglicherweise nicht. *Weitere Mängel:* Unklar ist, wessen Bestätigung entfällt (Dokumentation – Eindeutigkeit). Offen ist auch, ob die Änderung ein kritisches Ereignis nach REQ-008 ist.
- **Mögliche Konsequenz:** Fristen werden versäumt, mit Folgen für Leistungsnachweise. Fehlerhafte Änderungen aus Quellsystemen werden ungeprüft verbreitet.
- **Fehlende Informationen:**
  - Wer ändert Termine heute, und wie werden Studierende derzeit informiert? (Studienadministration, Lehrendenvertretung)
  - Wessen Bestätigung soll entfallen, und warum? (Lehrendenvertretung, Studienadministration)

**REQ-014 – The Accessibility Shortcut**
> „Der Study Buddy muss auf allen Geräten vollständig barrierefrei funktionieren.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Überprüfbarkeit
- **Fehlerbeschreibung:** Der Bedarf ist berechtigt, aber es gibt keinen Standard, keine Konformitätsstufe und kein Prüfverfahren. *Weitere Mängel:* „Allen Geräten“ und „vollständig“ sind Absolutbegriffe und so nicht erfüllbar (Dokumentation – Eindeutigkeit). Betroffene Studierende sind nicht einbezogen.
- **Mögliche Konsequenz:** Nicht abnahmefähig. Wird erst später klar, was Barrierefreiheit konkret heißt, muss das fertige System nachträglich umgebaut werden. Das kostet viel Aufwand, oder es bleiben Lücken, und Studierende mit Behinderung werden ausgeschlossen.
- **Fehlende Informationen:**
  - Welche rechtlichen Vorgaben und welcher Standard gelten für die FernFH? (Expert:innen für Barrierefreiheit und Inklusion)
  - Welche Geräte nutzen Studierende tatsächlich? (Studierendenvertretung, IT & Online-Campus-Team)

**REQ-015 – The AI Knows Best**
> „Ein KI-Modell muss anhand der Nutzungsdaten automatisch entscheiden, welche Studierenden zusätzliche Betreuung benötigen.“

- **Qualitätsaspekt:** Inhalt
- **Qualitätskriterium:** Keine vorzeitigen Entwurfsentscheidungen
- **Fehlerbeschreibung:** Die Technologie („KI-Modell“) ist festgelegt, bevor das Problem verstanden ist. Ob eine automatische Entscheidung überhaupt die geeignete Lösung ist, wurde nicht geprüft. *Weitere Mängel:* Das System soll ohne menschliche Beteiligung über Menschen entscheiden, ohne dass Studierende, Lehrende und Datenschutz einbezogen wurden (Abgestimmtheit). Wie bei REQ-001 ist unbelegt, dass Nutzungsdaten Betreuungsbedarf abbilden.
- **Mögliche Konsequenz:** Schwer nachvollziehbare Fehlentscheidungen und Benachteiligung bestimmter Gruppen. Dazu kommen Vertrauensverlust, rechtliche Risiken und hoher Aufwand.
- **Offene Fragen:**
  - Welche Unterstützungsaufgaben gibt es heute, und wer übernimmt sie aktuell? (Lehrendenvertretung, Studiengangsleitung)
  - Soll das System entscheiden oder nur Hinweise für eine Person liefern? (Studiengangsleitung, Datenschutz & Informationssicherheit)
  - Welche Daten dürfen dafür verwendet werden? (Datenschutz & Informationssicherheit)

---

**Widersprüche zwischen Requirements**

- **REQ-007 widerspricht REQ-008 und REQ-005**: REQ-007 will, dass man alle Benachrichtigungen abschalten kann, REQ-008 und REQ-005 schreiben Pflichtbenachrichtigungen vor. Es fehlt eine abgestimmte Einteilung der Benachrichtigungsarten.
- **REQ-013 widerspricht möglicherweise REQ-008**: REQ-013 will Terminänderungen still übernehmen, REQ-008 verlangt eine Benachrichtigung bei kritischen Studienereignissen. Ob eine Terminänderung ein solches Ereignis ist, ist nicht geklärt.

**Weitere Zusammenhänge zwischen Requirements**

Diese Punkte sind keine direkten Widersprüche, zeigen aber Überschneidungen und Abhängigkeiten, die geklärt werden müssen.

- **REQ-001, REQ-003, REQ-004, REQ-006 und REQ-015**: Ähnliche Risikobegriffe (Inaktivität, Schwierigkeiten, Abbruch, Lernrückstand, Betreuungsbedarf) ohne gemeinsame Definition.
**REQ-003, REQ-006, REQ-009 und REQ-015**: Weitergabe individueller Lerndaten, der Konflikt zwischen Unterstützung und Überwachung ist nirgends geklärt.
**REQ-003, REQ-005 und REQ-013 hängen von REQ-010 ab**: Alle brauchen Fristdaten aus REQ-010, deren Qualität ungeklärt ist.

**Befunde zur gesamten Anforderungen**

- **Vollständigkeit:** Es gibt keine Datenschutzanforderung, obwohl mehrere Anforderungen personenbezogene Lerndaten verarbeiten. Barrierefreiheit ist nur als Einzeiler vorhanden.
- **Dokumentationsregeln und Verfolgbarkeit:** Keine Anforderung hat Quelle, Begründung, Priorität, Status oder Akzeptanzkriterien.
- **Verständlichkeit:** Es fehlt ein Glossar für Begriffe wie Lernfortschritt, Inaktivität oder kritischer Lernrückstand.
