# Spieltag-PLUS-UML
UML Diagramme zum Projekt Spieltag PLUS

## Use-Case-Diagramm

Das Use-Case-Diagramm zeigt die wichtigsten Akteure und Funktionen der Plattform Spieltag-PLUS.

### Akteure
- Fan
- Stadionpersonal
- Admin
- KI-System

### Zentrale Funktionen
- Ticketkauf
- Stadionzugang
- Sicherheitsüberwachung
- Community-Funktionen
- KI-Analysen

![Use-Case-Diagramm](images/use-case.png)

## Komponentendiagramm

Das Komponentendiagramm zeigt die wichtigsten Softwaresysteme von Spieltag-PLUS und deren Abhängigkeiten.
Als Komponenten habe ich unter Beachtung des "Think Big" nicht einzelne Klassen gezeichnet, sondern größere Bausteine der Plattform.

### Komponenten

- Webanwednung
- Mobile-App
- Ticketing-System
- Community-System
- KI- & Analytics-Service
- Sicherheits-Service
- Benutzerverwaltung
- Datenbank

![Komponentendiagramm](images/komponentendiagramm.png)

# Klassendiagramm

## Enthaltene Klassen

- Benutzer
- Ticket
- Spiel
- Stadion
- Verein
- Kommentar
- KI Analyse

## Verwendete UML-Elemente: Komposition / Aggregation / Assoziation und Kardinalitäten

### Erklärung Beziehungen


Komposition

Spiel ♦── Ticket

Ein Ticket existiert nur im Kontext eines bestimmten Spiels.
Findet das SPiel nicht statt, verfällt das Ticket für diese spezielle Spiel mit diesem speziellen Datum.

Benutzer ♦── Kommentar

Kommentare gehören zu einem Benutzer und werden von diesem erstellt.
Falss Benutzer gelöscht wird, ist auch sien Kommentar weg.

Aggregation

Stadion ◇── Spiel

Ein Stadion kann mehrere Spiele austragen.

Spiel ◇── KI Analyse

Zu einem Spiel können mehrere Analysen erzeugt werden.

Benutzer ◇── Ticket

Ein Benutzer besitzt 0 oder mehr Tickets.

Assoziation

Verein ─── Spiel

Ein Verein hat mehrere Spiele.


![Klassendiagramm](images/klassendiagramm.png)

# Aktivitätsdiagramm

## Ziel

 UML-Aktivitätsdiagramm: Es beschreibt den Ablauf eines Ticketkaufs vom Auswählen eines Tickets bis zur erfolgreichen Speichern eines Tickets.


## Ablauf

1. Ticket auswählen
2. Benutzer anmelden
3. Falls der Benutzer unbekannt ist, Registrierung durchführen
4. Zahlung durchführen
5. Zahlung prüfen
6. QR-Code generieren
7. Ticket speichern
8. Prozess beenden

## Verwendete UML-Elemente

- Startknoten
- Endknoten
- Aktivitäten
- Kontrollflüsse
- Entscheidungsknoten
- Schleife

## Diagramm

![Aktivitätsdiagramm](images/aktivitaetsdiagramm.png)




