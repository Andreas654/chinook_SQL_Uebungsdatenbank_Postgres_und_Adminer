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
