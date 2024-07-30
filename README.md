# Sammlung an simplen Docker Compose

## Usage

Run first:
```bash
docker network create --driver bridge proxy
```

## Services

| Service                                                               | Port                                   |
| --------------------------------------------------------------------- | -------------------------------------- |
| [Adguard Home](https://hub.docker.com/r/adguard/adguardhome)          | [3002](http://localhost:3002) 53 67 68 |
| [Adminer](https://www.adminer.org/)                                   | [8081](http://localhost:8081)          |
| [Alpine](https://hub.docker.com/_/alpine)                             | docker exec -it alpine /bin/sh         |
| [Authentik](https://goauthentik.io/)                                  | [9001](http://localhost:9001)          |
| [Cloudcmd](https://cloudcmd.io/)                                      | [8000](http://localhost:8000)          |
| [CockroachDB](https://www.cockroachlabs.com/)                         | 26257                                  |
| [Code Server](https://github.com/linuxserver/docker-code-server)      | [8443](http://localhost:8443)          |
| [Dawarich](https://github.com/Freika/dawarich)                        | [3007](http://localhost:3007)          |
| [DBGate](https://dbgate.org/)                                         | [8084](http://localhost:8084)          |
| [Dockge](https://github.com/louislam/dockge)                          | [5002](http://localhost:5002)          |
| [Dozzle](https://dozzle.dev/)                                         | [8087](http://localhost:8087)          |
| [Firebird](https://firebirdsql.org/)                                  | 3050                                   |
| [Glances](TODO)                                                       | [TODO](http://localhost:)              |
| [Grafana-Loki](https://grafana.com/docs/loki/latest/)                 | [3000](http://localhost:3000) 3100     |
| [Gramps Web](https://www.grampsweb.org/)                              | [81](http://localhost:81)              |
| [Guacamole](https://github.com/jwetzell/docker-guacamole)             | [80](http://localhost)                 |
| [Home Assistant](https://www.home-assistant.io/)                      | [8123](http://localhost:8123)          |
| [Homepage](https://gethomepage.dev)                                   | [3045](http://localhost:3045)          |
| [InfluxDB](https://www.influxdata.com/)                               | [8086](http://localhost:8086)          |
| [JDownloader2](https://jdownloader.org/jdownloader2)                  | [5800](http://localhost:5800)          |
| [libsql](https://github.com/tursodatabase/libsql)                     | 5001 8098                              |
| [MariaDB](https://mariadb.org/)                                       | 3306                                   |
| [MySpeed](https://github.com/gnmyt/myspeed)                           | [5216](http://localhost:5216)          |
| [MySQL 8](https://www.mysql.com/)                                     | 3308                                   |
| [Nextcloud](https://github.com/nextcloud/docker)                      | [8080](http://localhost:8080)          |
| [nginx](https://hub.docker.com/_/nginx)                               | [82](http://localhost:82)              |
| [Obsidian-LiveSync](https://github.com/vrtmrz/obsidian-livesync)      | [5984](http://localhost:5984/_utils/)  |
| [Olivetin](https://github.com/OliveTin/OliveTin)                      | [1337](http://localhost:1337)          |
| [PHPmyAdmin](https://hub.docker.com/_/phpmyadmin)                     | [8083](http://localhost:8083)          |
| [Plex](https://github.com/linuxserver/docker-plex)                    | [32400](http://localhost:32400)        |
| [Portainer](https://www.portainer.io/)                                | [9000](http://localhost:9000)          |
| [PostgreSQL 15](https://www.postgresql.org/)                          | [5432](http://localhost:5432)          |
| [Radarr](https://github.com/linuxserver/docker-radarr)                | [7878](http://localhost:7878)          |
| [SQLChat](https://github.com/sqlchat/sqlchat)                         | [3005](http://localhost:3005)          |
| [Telegraf](https://www.influxdata.com/time-series-platform/telegraf/) |                                        |
| [traefik](https://doc.traefik.io/traefik/)                            | [8085](http://localhost:8082) 83 444   |
| [Transmission](https://github.com/linuxserver/docker-transmission)    | [9091](http://localhost:9091)          |
| [Uptime Kuma](https://github.com/louislam/uptime-kuma)                | [3001](http://localhost:3001)          |
| [Watchtower](https://containrrr.dev/watchtower/)                      |                                        |
| [Watchtower](https://containrrr.dev/watchtower/)                      |                                        |
| [Webtrees](https://github.com/fisharebest/webtrees)                   | [86](http://localhost:86)              |
| [Whoami](https://hub.docker.com/r/traefik/whoami)                     | [84](http://localhost:84)              |
| [whoDB](https://github.com/clidey/whodb)                              | [8082](http://localhost:8082)          |
| []()                                                                  | [](http://localhost:)                  |



![homepage1](homepage1.jpg)
![homepage2](homepage2.jpg)

## ToDo

- moodle
- kavita
- mealie
- metube
- pinchflat
- netalertx
- netdata
  - demo: https://app.netdata.cloud/spaces/netdata-demo/rooms/all-nodes
- stirlingpdf
- redis
- tinyfilemanager
- vaultwarden
- https://github.com/ChristianLempa/boilerplates/tree/main/docker-compose
  - cadvisor
  - heimdall
  - homer
  - influxdb2
  - pihole

### Übung

- Adguard
  - localhost DNS Server möglich?
- Nginx Proxy Manager
- beliebige App
- gemeinsames poxy Docker Netzwerk

### add to readme and homepage

- webtrees
- sqlchat
- postgres15
- olivetin
- whoami
- glances

## Tools

- [Composerize](https://www.composerize.com/)