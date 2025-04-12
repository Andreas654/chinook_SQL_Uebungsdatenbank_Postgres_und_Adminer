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

# PostgreSQL Practice Repository

Dieses Repository stellt eine Codespace-Umgebung für eine PostgreSQL-Datenbank bereit, um Übungen mit SQL durchzuführen.

## Verwendung

1. Öffnen Sie dieses Repository in Codespaces.
2. Verbinden Sie sich mit der PostgreSQL-Datenbank mit den folgenden Verbindungsinformationen:
    - Host: `localhost`
    - Port: `5432`
    - Benutzername: `youruser`
    - Passwort: `yourpassword`
    - Datenbank: `yourdatabase`
