# Schlüsselinventur – IHK-Abschlussprojekt

Neuentwicklung dynamischer Inventur-Berichte für die Schlüsselexemplar-Inventur 
im System **agentes Key Store Management (aKSM)**.

## Ausgangssituation
Kunden des aKSM-Systems führen regelmäßig Inventuren durch, um den 
Buchbestand (Soll) mit dem tatsächlichen Bestand (Ist) abzugleichen. 
Da die Software erweitert wurde, um einzelne Schlüssel-Exemplare an 
Schlüsselbunden zu erfassen, basierten die alten Inventur-Berichte 
noch auf veralteter Logik und zeigten Schlüsselbunde nur als 
Gesamtobjekt an – eine zuverlässige Inventur war so nicht mehr möglich [file:99].

## Projektziel
Neuentwicklung der zwei zentralen Reporting-Komponenten auf Basis der 
neuen n:1-Datenbankstruktur:
- **Inventurliste (Laufzettel)** – löst Schlüsselbunde dynamisch in 
  Einzelschlüssel auf und zeigt Gravurnummern zur eindeutigen Identifikation
- **Inventurdifferenzliste** – übersichtliche Darstellung aller Abweichungen 
  (z. B. "Fehlt", "Gefunden") als Arbeitsgrundlage für den Organisator [file:99]

## Meine Aufgaben
- Vollständige Neuentwicklung der dynamischen Berichtsstrukturen
- Implementierung der Datenbeschaffung über Datenbank-Views und Groovy
- Schlüsselbund-Logik über Eltern-Kind-Zuordnung in Groovy-Skripten
- Dynamische Spaltensteuerung je nach Inventurart (Person, Schrank, Depot)
- Integration der Reports in die Java-Anwendung [file:100]

## Eingesetzte Technologien
- **JasperReports / JRXML** – Berichtslayout
- **Groovy** – Skriptlogik und Datenaufbereitung
- **MySQL** – Datenbank (Views statt JPQL für die Datenbeschaffung)
- **Java (IntelliJ)** – Systemintegration
- **Git** – Versionierung

## Inhalt dieses Repositories
- `projektantrag.pdf` – Ursprünglicher Projektantrag mit Zielsetzung
- `antrag-anlagen.pdf` – Anlagen zum Projektantrag (Fachkonzept-Auszüge)
- `inventurschluessel-dokumentation.pdf` – Vollständige Projektdokumentation
- `inventur-depot-handout.pdf` – Handout zur Präsentation
- `praesentation.pdf` – Präsentationsfolien

## Hinweis
Aus Datenschutz- und Vertraulichkeitsgründen wird hier ausschließlich 
die Dokumentation veröffentlicht, kein Produktivcode des Unternehmens.

## Kontakt
**Mousa Al Ataallah**  
[LinkedIn](https://www.linkedin.com/in/mousa-al-ataallah)
