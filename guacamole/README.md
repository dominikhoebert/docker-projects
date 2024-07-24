## Usage

TODO

## Installation

1. VNC/RDP
   1. Windows   
TODO
   2. macOS  
`System Settings` -> `General` -> `Sharing` -> `Screen Sharing` activieren (Kann verwendet werden um Screen sharing kurzfristig zu deaktivieren)  
Weiters sollten die entsprechenden Screen Sharing Settings gesetzt werden auf `i`

2. Docker  
Download und installiere [Docker Desktop](https://www.docker.com/)  
Docker ist korrekt installiert, wenn in der GUI die linke untere Ecke grün ist.

3. Container  
Erstelle in deinem Benutzerverzeichniss einen Ordner `guacamole`.  
Erstelle [compose.yml](https://github.com/dominikhoebert/docker-projects/blob/master/guacamole/compose.yml) in diesem Ordner  
Öffne das Terminal und führe folgende zwei Befehle aus  
```
cd guacamole
docker compose up -d
```

4. Config  
Die Weboberfläche sollte nun über [http://localhost](http://localhost) erreichbar sein  
Standart Login `guacadmin`/`guacadmin`  
Settings oben rechts auf `guacadmin`

   1. Password  
Das Standartpasswort sollte in Preferences geändert werden (manche   
Schüler kennen das Standartpasswort)  
   2. Connection  
`Connections` -> `New Connection`  
Beliebieger Name z.B. `Schule`  
Protocol: RDP (Windows); VNC (macOS)  
Maximum number of connections: 60  
Maximum number of connections per user: 60  
Hostname: `host.docker.internal`  
Port: TODO (Windows); 5900 (macOS)  
Authentication: Benutzername und Passwort des Geräts eingeben  
Display:  
Read-Only aktivieren  
Cursor: Remote  
Color Depth 32-Bit  
Encoding: UTF-8  
-> Save ganz unten
   3. Schueler User  
Users -> New User  
Username: schueler  
Password: schueler  
Connections: Schule aktivieren  
-> Save ganz unten
