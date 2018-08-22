Seitennummerierung

# VIP-Event, 30. August 2018

## Ziel:
 - IoT Kompetenzen zeigen
 - Unterhaltsam
 
## Format:
 - 10-15'
 - Präsentation via Link auf Internet abrufbar


## Thema: 
# Wenn es vernetzten Maschinen "heiss" und "kalt" wird

Währenddem wir hier fahren, möchte ich Sie gedanklich in einem Operations-Saal "entführen".
Stellen Sie sich vor, Sie müssen operiert werden, und zwar am offenen Herzen.
Alles wird vorbereitet, geschickt werden sie vom Personal eingepackt und an all den Apparaten angeschlossen.
Der Anästhesist spricht Ihnen breruhingend Worte zu, dass Sie nun eine Weile ruhig schlafen werden. 

Doch einige Sekunden bevor Sie einschlafen, fällt Ihnen ein Gerät auf:
 - Deren SW kennen Sie bestens: Sie haben selbst daran gearbeitet, als SW-Architekt.
 - Sie kennen die Use-Cases und die detaillierte Funktionalität. 
 - Sie haben auch an der Risikoanalyse mitgewirkt
 - Sie kennen die offenen Bugs
  
Frage: Wie werden Sie diese letzten Sekunden vor dem Einschlafen erleben?
Wird Ihnen "heiss" und "kalt"?

Mein Name ist Antonino Leanza, arbeite bei bbv als SW-Architekt, und erzähle Ihnen heute eine Geschichte darüber, wie mir und den Maschinen die ich programmiere "heiss" und "kalt" wird.

Als mein erster Sohn zur Welt kam, befand ich mich plötzlich in eine ähnliche Situation, wie anfangs beschrieben. Alle von Ihnen, die Eltern sind, wissen genau, dass eine Entbindung kein Spaziergang ist.
Wir Männer können psychologisch etwas dazu beitragen. Da lag meine Frau, nach 23 Stunden Wehen, es ging nicht vorwärts, und sie hatte - ohne Witz - ein kaltes und ein warmes Bein. Zwischer einer Wehe und der nächsten, schmunzelten wir kurz darüber, und entschieden uns mit der Gynäkologin für einen Kaiserschnitt. Und plötzlich bemerkte ich es: das Anästhesie-Gerät. Nicht unser, sondern von der Konkurrenz. Ich kann Ihnen versichern: Ich hoffte sehr stark, die Konkurrenz hätte mindestens so gut wie wir gearbeitet!

--- 
## Seite 2
Alles verlief zum Glück gut und mein Sohn kam gesund zur Welt.

Damals arbeitete ich verstärkt im Embedded-Umfeld. Heute erstelle ich Cloud-Lösungen. Vor einigen Monaten, habe ich an einem IoT-Projekt gearbeitet. Das Produkt hatte zwar keine direkten Folgen für Personen. Das bedeutet aber keineswegs, dass es weniger anspruchsvoll war.

 - Immer kleinere, low-power Geräte müssen in der Lage sein, Daten auszutauschen. 
 - Die vorhandenen Umsystem müssen berücksichtigt werden.
 - Wichtige Daten müssen schnell zu den richtigen Personen kommen (Hot-Path)
 - Alle Daten müssen zudem zuverlässig abgelegt und abgefragt werden können (Cold-Path)
 - Alles produziert heutzutage Daten: danach werden die Maschinen ausgewertet.

---
## Seite 3
 - Wie können wir die Daten IHRER Geräte, zum einen SICHER halten, und auch so dass sie BEIZEITEN zu den richtigen Personen kommen?

Wie schafften es wir, ein Systemen zu realisieren, das zum einen nur so komplex wie nötig, zum anderen genau die Bedürfnisse unseres Kunden befriedigt?

---
## Seite 4
Ich möchte Ihnen erzählen, wie wir es für die Firma Agathon AG gemacht haben. Agatho produziert seit etwas mehr als 100 Jahren Hochpräzisions-Schleifmaschinen. Diese möchte nun Agathon an die Cloud knüpfen.

Warum? 
---
## Seiten 5 und 6

### Was sind die wichtigsten Use-Cases?
 - Der Schichtleiter muss am System den Betriebststand aller Maschinen des Maschinenparks einsehen können, sodass er die Maschinen mit Rohmaterial optimal versorgen kann.
 - Der Schichleiter soll vom System benachrichtigt werden wenn auf einer Maschinen ein Ausnahmezustand entsteht, sodass er den Fehler beheben eine möglichs hohe Auslastung sicherstellen kann.
 
---
## Seite 7
 - Der Schichtleiter soll eine Maschine auf einfache Art am System registrieren können, ohne Stammdaten pflegen zu müssen, somit spart er Zeit und kann sich sofort um das Wesentliche kümmern.
 
### Weitere strategische Gründe:
 - Erster Schritt in Richtung Industrie 4.0
 - Innovation

---
## Seite 8
Demnach, haben wir uns genügend Zeit genommen, um die funktionalen Anforderungen zu verstehen, nicht bereits schon eine konkrete Lösung.
 - Wer soll wann welche informationen sehen, und warum?

---
## Seite 9
Nebst den rein funktionalen Anforderungen sollte ich Sie eigentlich noch langweilen, mit weiteren Nicht-Funktionalen Anforderungen, die mit dem Kunden abgesprochen und priorisiert werden mussten. Diese beeinflussen stark die Architektur:
 - Geschwindigkeit
 - Erweiterbarkeit
 - Installierbarkeit
 - Verfügbarkeit
 - Skalierbarkeit
 - ...
 
Eine Übersicht finden Sie im ISO 25010-Standard, was übrigens in jedem SW-Projekt als Checkliste eingesetzt werden sollte. 

---
## Seite 10

Slide: Symbole Agilität und DevOps

Funktionale und Nicht-Funktionale Anforderungen sollten vom gesamten Team gut verstanden werden. Genauso wichtig ist es, die Enduser zu involvieren, ihnen regelmässig den Stand des Systems vorzuführen, sodass sie möglichst früh ihre Rückmeldung dazu geben können. Aus sollte jede Funktionseinheit automatisiert testbar sein. Das alles heisst Agil, das alles heisst DevOps-Philosophie.

Warum braucht es das eigentlich?
Was passiert, wenn man das nicht macht?

Kommen wir zum Beispiel von anhin zurück.
Stellen Sie sich vor, Sie wachen noch während der Herz-OP auf. 

- Herr Chirurg!
- Ja?
- Entschuldigung, dass ich störe, habe plötzlich Schmerzen.
- Wo? Am Herz?
- Nein, am rechten Fuss. Ist das normal?
- Äh, ja. Aber machen Sie sich keine Sorgen. Beseitigen wir in einer nächsten OP.

Etwas skurril? Wissen Sie wieviele unserer Kunden "am offenen Herz" eines Systems arbeiten?
Dieselben wundern sich dann über Nebeneffekte: Warum klappert es an einer völlig anderen Stelle, die mit der Änderung nicht zu tun hat?

Warum dauert das Erstellen von Releases immer länger? Warum wird das Team selbst dann nicht schneller, wenn ich zur Not mehr leute beiziehe?
... Das alles trägt eine unsichtbare Unterschrift: "MfG, Spaghetticode".

Weitere Knackpunkte: in Cloud-Szenarien ist die Fehlersuche, ohne geeignete Massnahmen, um Potenzen komplexer. Man sich eine Menge Ärger sparen, wenn die Business-Logik automatisiert getestet wird, und zwar automatisiert, und zwar nach jeder Änderung, losgelöst von jeglicher Cloud-Infrastruktur. 
DevOps und Test-Driven-Development heissen hier die Schlagworte.

---
## Seite 11
In der Präsentation sehen sie die System-Architektur die nach einigen Iteration entstanden ist.

Sie sehen für die Clienst 2 Schnittstellen:
- IoT-Clients müssen sich zunächst registrieren.
- Dann senden sie über MQTT Telemetrie-Daten
- Alle Teilnehmer, die sich auf ein Gerät gepairt haben, erhalten die Daten, sei es als Push-Notification, oder in der App.

---
## Seite 12

Cloud-Architektur Slide löschen

Weitere Eigenschaften der gewählten Lösung:
 - PaaS-Lösung, Managed Services, keine IaaS
 - Message-Spezifisches Routing der Nachrichten (Hot- und Cold-Paths)
 - Trennung Konfigurations- und Betriebsdaten-DB
 - Wir bauen stark auf Serverless Functions auf, parallel ausführbar, beliebig skalierbar
 - Ausfallsicherheit, garantiert duch Service-Level-Agreements
 - Leichtgewichtige Standard-Schnittstellen
 - ISO-Schnittstelle MQ Telemetry Transport und  
 - REST (REpresentational State Transfer)
 
 "Ok, Ok. Mag alles cool sein, aber wieviel kostet mir das?"
 
---
## Seite 13 und 14
 Sehr berechtigte Frage. Man kann vorher die Betriebskosten grob abschätzen, indem man die benötigten Cloud-Komponenten annimmt und ein Mengengerüst der Daten erstellt.
 Im nachhinein können wir sagen, die Schätzung stimmte recht gut.

---
## Seite 15
# Fazit
- Herr Scholze (Geschäftsführender Vizepräsident von Agathon) ist heute unter uns, und er wird Ihnen bestätigen können, dass es für sowohl für Agathon, als auch für bbv ein sehr erfolgreiches Projekt war.
  - 2-Wöchiges Proof-Of-Concept, danach Implementierung durch 2 bbv-MA, pünktlich 3 Monate später abgeliefert
- Risiko-Minimierung dank PoC und MVP-Ansatz
- PaaS Lösung dank Azure Managed Services
  - Konformität mit internationalen und industrie-spezifischen und Security and Privacy-Standards (GDPR, ISO 27001)
- Keine CapEx für HW, nur OpEx (Pay-As-You-Go )
- Flexibilität durch Agilität und DevOps
  - Test- und Prod-Umgebung
  - Schnelle Release-Zyklen, autom. Deployment
  - Planung integriert mit Entwicklungsumgebung
- Zugriff auf Expertise innerhalb der bbv

 
---
## Seite 16
# Ausblick
- Analyse und Reporting 
  - Big Data
- Basis schaffen für weitere Services und Dienstleistungen
  - Remote Update von Soft- und Firmware
  - Allg. Maintenance-Bereich
  - Aber auch --> Preventive und ev. Predictive Maintenance
- Geräte-Funktionen
  - Gezielten Eingriff ermöglichen, z.B. Not-Stopp

   
Gerne stehe ich Ihnen später für Fragen zur Verfügung, nicht für Herz-OPs, sondern für innovative Cloud-Lösungen.


Frage-Runde
- Security: Kein Remote Control der Maschinen, Azure Managed Services mit Compliance Zertifizierungen
- Datenschutz: Keine sensiblen, personenbezogenen Daten, Aus Daten lassen sich keine fundierten Rückschlüsse schliessen auf Intellectual Property
- Aufwand/Kosten
- Kundenfeedback
