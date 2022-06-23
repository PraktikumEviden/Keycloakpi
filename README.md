# Keycloakpi

setup von Keycloak auf dem Raspberrypi 4 mithilfe von docker.

1. Docker auf dem Raspberry installieren und mit dem folgendem docker starten.
     https://registry.hub.docker.com/r/ruifigueiredo/rpi-keycloak

2. Nachdem der docker gestartet wurde, sollte er unter der Adress des raspberrypi's laufen unter dem Port: 8180 bei mir war es z.B http://raspberrypi.local:8180/auth/
   Du kannst dich anschließend mit dem namen: admin password: admin anmelden

3. Nun konfigurieren wir den keycloak. #Note: Falls dir die Folgenden Namensgebung nicht gefällt, kannst du sie einfach unter Angular src/app/environments   /keycloak.config.ts ändern.# Darauf erstellt ihr realm, mit dem namen myrealm. Danach erstell ihr ein Client mit dem namen angular,und konfigurieren ihn.   Base & Admin URL = http:/raspberrypi.local/auth:8180 ,Web Origins und Valid Redirect Url's müssen konfiguriert werden.
4. Zum Schluss muss noch noch ein Client mit dem Namen angular angelegt werde, oder einen anderen, falls du es in der config geändert hast.

Zusatz: Wenn du Benutzer im login Fenster anlegen möchtest, musst du noch bei myreal unter login User registration einschalten.
