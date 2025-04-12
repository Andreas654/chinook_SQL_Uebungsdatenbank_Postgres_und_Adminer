1. Start Docker Container mit
    cd devcontainer
    ./start.sh


2. Login Hinweise für Adminer

Datenbanksystem: postgreSQL
Server: postres
Benutzer: your_user
Password: your_password
Datenbank:  your_db

3. Beispiel für SQL Statement
SET SCHEMA 'chinook';
SELECT * FROM artist;

# PostgreSQL SQL Übungsdatenbank und Adminer

Dieses Repository stellt eine Codespace-Umgebung für eine PostgreSQL-Datenbank bereit, um Übungen mit SQL durchzuführen.

## Verwendung

1. Öffnen Sie einen Coidespace für dieses Repository
2. Start Docker Container mit
    - cd devcontainer  (Wechsel ins Verzuechnis devconatiner)
    - ./start.sh  (Start eines Skripts)

3. Starten Sie Adminer in einem Browser
Anmeldeinforantionen für den Adminer:
- Datenbanksystem: postgreSQL
- Server: postgres
- Benutzer: your_user
- Password: your_password
- Datenbank: your_db


4. Beispiel für einen SQL-Befehl
- SET SCHEMA 'chinook';
- SELECT * FROM artist;

5. Verbindungsinformationen für die SQL-Datenbank  (zu verifizieren!)
    - Host: `localhost`
    - Port: `5432`
    - Benutzername: `youruser`
    - Passwort: `yourpassword`
    - Datenbank: `your_db`
