# Keycloakpi

setup von Keycloak auf dem Raspberrypi 4 mithilfe von docker.

1.Docker auf dem Raspberry installieren und mit dem folgendem docker starten.
     https://registry.hub.docker.com/r/ruifigueiredo/rpi-keycloak

2. Nachdem der docker gestartet wurde, sollte er unter der Adress des raspberrypi's laufen unter dem Port: 8180 bei mir war es z.B: http:10.42.0.219:8180
   Du kannst dich anschließend mit dem namen: admin password: admin anmelden

3. Nun konfigurieren wir den keycloak. Note: Falls dir die Folgenden Namensgebung nicht gefällt, kannst du sie einfach unter Angular src/app/environments/keycloak.config.ts ändern. Darauf erstellt ihr realm, mit dem namen myrealm 

![alt text](https://github.com/[PraktikumAtos]/[Keycloakpi]/blob/[main]/image.png?raw=true)
