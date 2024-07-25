# Guacamole

Clientlose Screensharing app. Schüler brauchen nur die IP Adresse der Lehrperson in ihrem Browser eingeben um sich den Screen ansehen zu können.

Basiert auf [jwetzell/docker-guacamole](https://github.com/jwetzell/docker-guacamole)

## Verwendung

VNC Server starten, Docker und Guacamole starten
eigene IP Adresse mit Schülern teilen

## Installation

### 1. VNC/RDP
#### Windows
VNC Server wird benötigt, zB.:
[UltraVNC](https://uvnc.com/downloads/ultravnc.html) neuste Stabile Version herunterladen und installieren

##### UltraVNC konfigurieren  
Rechtsklick auf das UltraVNC Tray Icon -> Admin Properties  
VNV Passsword setzen -> OK

#### macOS  
`System Settings` -> `General` -> `Sharing` -> `Screen Sharing` activieren (Kann verwendet werden um Screen sharing kurzfristig zu deaktivieren)  
Weiters sollten die entsprechenden Screen Sharing Settings gesetzt werden auf `i`

### 2. Docker  
Download und installiere [Docker Desktop](https://www.docker.com/)  
Docker ist korrekt installiert, wenn in der GUI die linke untere Ecke grün ist.

### 3. Container  
Erstelle in deinem Benutzerverzeichniss einen Ordner `guacamole`.  
Erstelle [compose.yml](https://github.com/dominikhoebert/docker-projects/blob/master/guacamole/compose.yml) in diesem Ordner  
Öffne das Terminal und führe folgende zwei Befehle aus  
```
cd guacamole
docker compose up -d
```

### 4. Config  
Die Weboberfläche sollte nun über [http://localhost](http://localhost) erreichbar sein  
Standart Login `guacadmin`/`guacadmin`  
Settings oben rechts auf `guacadmin`

   #### 1. Password  
Das Standartpasswort sollte in Preferences geändert werden (manche   
Schüler kennen das Standartpasswort)  
   #### 2. Connection  
`Connections` -> `New Connection`  
Beliebieger Name z.B. `Schule`  
Protocol: VNC  
Maximum number of connections: 60  
Maximum number of connections per user: 60  
Hostname: `host.docker.internal`  
Port: `5900`  
Authentication:  
Benutzername und Passwort eingeben:  
UltraVNC: Username leer, Passwort wie gewählt  
macOS: User und Passwort des Geräts  
Display: Read-Only aktivieren  
Cursor: Remote  
Color Depth: 32-Bit  
Encoding: UTF-8  
u.a. entsprechend anpassen  
-> `Save` ganz unten
   #### 3. Schueler User  
`Users` -> `New User`  
Username: `schueler`  
Password: `schueler`  
Connections: Schule aktivieren  
-> `Save` ganz unten
