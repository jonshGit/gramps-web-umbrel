# Gramps Web Community App Store für umbrelOS 2.0

Dieses Repository ist als eigener Umbrel Community App Store aufgebaut.

## Installation

1. Repository auf GitHub anlegen.
2. Alle Dateien dieses Repositorys hochladen.
3. In umbrelOS den Community App Store hinzufügen:
   `App Store -> ... -> Community App Stores -> Add`
4. Die URL dieses GitHub-Repositories eintragen.
5. Nach dem Aktualisieren des App Stores `Gramps Web` installieren.

## App-ID

`genealogy-gramps-web`

Die App verwendet den offiziellen Gramps-Web-Container und zusätzlich einen
Celery-Worker sowie Valkey.

## Persistente Daten

Alle wichtigen Daten werden unter `${APP_DATA_DIR}/data/` gespeichert:

- grampsdb
- media
- users
- indexdir
- thumbnail_cache
- cache
- secret
- redis

## Sicherheit

Die App ist für die Nutzung innerhalb des Umbrel-Netzes gedacht. Für eine
Veröffentlichung im Internet muss HTTPS verwendet werden.

## Quellen

Gramps Web Docker Deployment:
https://www.grampsweb.org/install_setup/deployment/

Umbrel Community App Store Template:
https://github.com/getumbrel/umbrel-community-app-store
