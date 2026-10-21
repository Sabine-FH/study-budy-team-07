# Aufgabe 02b Plot Twist

#### Handelt es sich um eine Anforderung, eine Rahmenbedingung oder eine Lösungsvorgabe?
Rahmenbedingung + Lösungsvorgabe  
Es ist eine verbindliche technische Rahmenbedingung, wenn der Study Buddy das bestehende Authentifizierungssystem verwenden muss. Zusätzlich kann die Vorgabe auch als Lösungsvorgabe betrachtet werden, weil eben schon festgelegt wird, wie die Authentifizierung technisch erfolgen soll. 

***

#### Welche möglichen Auswirkungen hat diese Vorgabe auf den Study Buddy? 
- Änderung/Erweiterung der technischen Vorgaben -> Weil der Study Buddy an das bestehende Authentifizierungssystem angebunden werden soll, könnten bestimmte Schnittstellen notwendig sein, die vorher nicht notwendig waren.
- Eingeschränkte Flexibilität -> Weil das Authentifizierungssystem schon besteht, muss sich die technische Umsetzung an die Möglichkeiten/Einschränkungen des bereits bestehenden Systems orientieren.
- Benutzerfreundlichkeit -> Studierende kennen das System schon und es muss kein zusätzlicher Login bedacht werden.
- Abhängigkeit und Verfügbarkeit -> Wenn das Authentifizierungssystem nicht verfügbar ist, kann das auch den Zugriff zu dem Study Buddy beeinträchtigen, also muss auch die Abhängigkeit der Verfügbarkeit in Betracht gezogen werden und möglicherweise ein Ausfallmechanismus (Failsafe) dazu bedacht werden.
- Berechtigungen -> Es muss geregelt werden, welche Nutzer:innen auf welche Funktionen und Daten zugreifen dürfen. Dabei muss sichergestellt werden, dass durch die gemeinsame Verwendung des Authentifizierungssystems keine unberechtigten Zugriffe auf andere Anwendungen oder deren Daten möglich sind..
- Technische Kapazitäten -> Da das Authentifizierungssystem schon fertig ist, sollte auch geprüft werden, ob das bestehende System die zusätzlichen Zugriffe durch den Study Buddy bewältigen kann oder ob dadurch Leistungs- oder Verfügbarkeitseinschränkungen entstehen könnten. 

***

#### Welche Fragen müssen Sie mit der IT klären?
- Welches Authentifizierungssystem wird derzeit verwendet und welche technischen Schnittstellen bietet es?
- Wie kann der Study Buddy in dieses Authentifizierungssystem integriert werden?
- Welche Benutzerinformationen und Berechtigungen werden über das System bereitgestellt?
- Sind zusätzliche technische Komponenten oder Anpassungen notwendig?
- Welche Datenschutz- und Sicherheitsmaßnahmen sind bereits vorhanden?
- Müssen spezielle Datenschutz- und Sicherheitsmaßnahmen ergänzt werden für den Study Buddy?

***

#### Welche weiteren Stakeholder könnten davon betroffen sein? 
- Datenschutz- und Informationssicherheitsverantwortliche - Für den Schutz personenbezogener Daten, Zugriffskontrollen und Sicherheitsanforderungen
- IT / Betreiber:innen des Online Campus - Für die technische Integration, Schnittstellen, Wartung und Betrieb
- Studierende - Für Fragen zu Benutzerfreundlichkeit und möglichen Zugriffsproblemen, die bereits da sind durch das derzeitige Authentifizierungssystem
