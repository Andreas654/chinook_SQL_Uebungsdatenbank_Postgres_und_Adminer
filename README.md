# PostgreSQL SQL Übungsdatenbank und Adminer

Dieses Repository stellt eine Codespace-Umgebung für eine PostgreSQL-Datenbank bereit, um Übungen mit SQL durchzuführen.

## Verwendung

1. Öffnen Sie einen Coidespace für dieses Repository
2. Start Docker Container mit
    - cd devcontainer  (Wechsel ins Verzeichnis devconatiner)
    - ./start.sh  (Start eines Skripts)

3. Starten Sie Adminer in einem Browser
Anmeldeinforantionen für den Adminer:
    - Datenbanksystem: `postgresql`
    - Server: `postgres`
    - Benutzername: `your_user`
    - Passwort: `your_password`
    - Datenbank: `your_db`



4. Beispiel für einen SQL-Befehl
    - SET SCHEMA 'chinook';
    - SELECT * FROM artist;

5. Verbindungsinformationen für die SQL-Datenbank  (zu verifizieren!)
    - Host: `localhost`
    - Port: `5432`
    - Benutzername: `your_user`
    - Passwort: `your_password`
    - Datenbank: `your_db`


## Pagila-Datenbank
Die Pagila-Datenbank ist eine Beispiel-Datenbank für PostgreSQL, die auf der bekannten Sakila-Datenbank von MySQL basiert. Sie wurde erstellt, um typische Geschäftsprozesse eines Filmverleihs zu modellieren, wie sie früher z. B. bei Blockbuster üblich waren. Der Name „Pagila“ ist ein Wortspiel aus „PostgreSQL“ und „Sakila“. Die Datenbank wird häufig im SQL-Training, im Unterricht und für Testzwecke verwendet, da sie ein realistisches, aber gut überschaubares Datenmodell bietet.

## Beschreibung der datenbank
Die Pagila-Datenbank modelliert die Abläufe eines fiktiven Filmverleih-Unternehmens mit mehreren Videotheken (Stores), Filmen, Kunden, Mitarbeitern und Zahlungsvorgängen. Die Struktur ermöglicht realitätsnahe Szenarien für praxisorientierte SQL-Abfragen.

Die wichtigsten Inhalte der Datenbank im Überblick:
•	film: Informationen über Filme, z. B. Titel, Länge, Sprache, Beschreibung, Bewertung und Mietkosten.
•	actor: Daten zu Schauspielern, die in Filmen mitspielen.
•	film_actor: Verbindungstabelle für die viele-zu-viele Beziehung zwischen Filmen und Schauspielern.
•	category: Enthält Filmkategorien wie Action, Comedy oder Drama.
•	film_category: Verbindungstabelle zwischen Filmen und Kategorien.
•	inventory: Einzelne physische Kopien von Filmen, die in einem bestimmten Store vorrätig sind.
•	store: Informationen zu Filialen des Filmverleihs.
•	address: Daten zu Adressen, die sowohl Kunden als auch Stores zugeordnet sein können.
•	city: Städte, denen Adressen zugeordnet sind.
•	country: Länder, in denen sich Städte befinden.
•	customer: Informationen zu Kunden wie Name, Adresse, E-Mail und aktiver Mitgliedschaft.
•	rental: Daten zu Ausleihvorgängen – welcher Kunde wann welchen Film ausgeliehen hat.
•	payment: Zahlungen, die mit Ausleihvorgängen verknüpft sind.
•	staff: Mitarbeitende, die in Stores arbeiten und Ausleihen oder Zahlungen bearbeiten.

Durch die Vielzahl von Tabellen und deren Beziehungen eignet sich die Pagila-Datenbank ideal für die Schulung in SQL. Sie erlaubt praxisnahe Auswertungen, zum Beispiel:
- Welche Filme wurden am häufigsten ausgeliehen?
- Wie viel Umsatz wurde pro Store erzielt?
- Welche Kunden sind besonders aktiv?
- Welche Schauspieler kommen besonders häufig vor?
Solche Fragestellungen helfen dabei, SQL-Kenntnisse auf reale Szenarien anzuwenden.
