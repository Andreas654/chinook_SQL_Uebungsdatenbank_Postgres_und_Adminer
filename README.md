# PostgreSQL SQL Übungsdatenbank und Adminer

Dieses Repository stellt eine Codespace-Umgebung für eine PostgreSQL-Datenbank bereit, um Übungen mit SQL durchzuführen.

## Verwendung

1. Öffnen/Erstellen Sie einen Codespace für dieses Repository

2. Start Docker Container im Codespace mit
    - cd devcontainer  (Wechsel ins Verzeichnis devconatiner)
    - ./start.sh  (Start eines Skripts)

3. Starten Sie Adminer in einem Browser (z.B. unter "Ports" durch Klicken auf "weitergeleitete Adresse" für Port 8080 und Auswahl des icons "in Browser öffnen"). 
Anmeldeinforantionen für den Adminer:
    - Datenbanksystem: `postgresql`
    - Server: `postgres`
    - Benutzername: `your_user`
    - Passwort: `your_password`
    - Datenbank: `your_db`



5. Beispiel für einen SQL-Befehl
    - SET SCHEMA 'chinook';
    - SELECT * FROM artist;

6. Bei Bedarf: Verbindungsinformationen für die SQL-Datenbank  (zu verifizieren!)
    - Host: `localhost`
    - Port: `5432`
    - Benutzername: `your_user`
    - Passwort: `your_password`
    - Datenbank: `your_db`


## Chinook-Datenbank
Die Chinook-Datenbank ist eine Beispiel-Datenbank, die speziell für das Erlernen und Üben von SQL-Abfragen entwickelt wurde. Sie wurde als moderne Alternative zur klassischen Northwind-Datenbank geschaffen, mit einem Fokus auf digitale Medien. Das zugrunde liegende Szenario simuliert ein Unternehmen, das digitale Musikdateien verkauft – ähnlich wie der ehemalige iTunes Store von Apple. Die Datenbank ist realitätsnah aufgebaut und enthält typische Geschäftsobjekte wie Kunden, Mitarbeiter, Produkte (in diesem Fall Musikstücke), Rechnungen und Zahlungen. Chinook eignet sich hervorragend, um praxisnahe Abfragen zu formulieren, da sie viele gängige Strukturen enthält: 1:n- und n:m-Beziehungen, Hierarchien, Zeitstempel, Preisangaben und mehr. Sie ist in verschiedenen Versionen für unterschiedliche relationale Datenbanksysteme (u. a. SQLite, PostgreSQL, MySQL, SQL Server) verfügbar und wird weltweit in Lehre, Schulungen und Bewerbungstests eingesetzt. Für Studierende bietet sie eine ideale Grundlage, um SQL-Grundlagen sowie fortgeschrittene Techniken wie Joins, Aggregationen, Unterabfragen oder Window Functions zu erlernen.

## Beschreibung der Datenbank
Die Chinook-Datenbank bildet die Geschäftsprozesse eines digitalen Musikshops ab. Im Mittelpunkt stehen Kunden (Customer), die über den Shop Musikstücke kaufen. Diese Käufe werden durch Rechnungen (Invoice) dokumentiert, wobei jede Rechnung aus einer oder mehreren Rechnungspositionen (InvoiceLine) besteht. Eine Rechnungsposition verweist auf ein konkretes Musikstück (Track), das verkauft wurde.

Jedes Musikstück ist Teil eines Albums (Album), das wiederum einem bestimmten Künstler (Artist) zugeordnet ist. Zusätzlich besitzt jeder Track Angaben zum Genre (z. B. Rock, Jazz) sowie zum Dateiformat bzw. Medium (MediaType), z. B. MPEG Audio oder AAC. Diese Struktur erlaubt es, detaillierte Abfragen zu erstellen, z. B. zu den meistverkauften Genres, den erfolgreichsten Künstlern oder dem Umsatz pro Medium.

Das Unternehmen beschäftigt zudem Mitarbeiter (Employee), die z. B. als Vertriebs- oder Supportmitarbeiter arbeiten. Zwischen den Mitarbeitern besteht eine hierarchische Beziehung, da jeder Mitarbeiter einem Vorgesetzten zugeordnet sein kann (Self-Join). Kunden wiederum sind einzelnen Mitarbeitern als Betreuer zugewiesen, was zusätzliche Möglichkeiten für Auswertungen im Bereich Kundenmanagement und Vertrieb eröffnet.

Ein weiteres interessantes Detail ist die geographische Dimension: Kunden besitzen Informationen zu Adresse, Stadt und Land, sodass auch regionale Auswertungen (z. B. Umsatz nach Ländern) möglich sind. Gleichzeitig sind Rechnungen mit Zeitstempeln versehen, was Analysen über Zeiträume hinweg erlaubt – etwa Trends in Verkaufszahlen oder saisonale Schwankungen.

Durch diese miteinander verknüpften Tabellen ergibt sich ein realistisches Datenmodell, mit dem sich viele Aspekte echter Geschäftsanalysen simulieren lassen. Man kann hier sowohl einfache SQL-Abfragen als auch komplexe Auswertungen mit mehreren Joins, Aggregatfunktionen, Filterbedingungen oder Subqueries üben.

## Relationenschema der chinook Datenbank
![postgres - chinook](https://github.com/user-attachments/assets/4a30622b-6bea-4892-96d4-b364f8c1e894)


## Github Quelle für die DB Skripte
https://github.com/lerocha/chinook-database/tree/master


https://github.com/lerocha/chinook-database/tree/master/ChinookDatabase/DataSources
