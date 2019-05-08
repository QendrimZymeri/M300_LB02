# M300_LB02

## Inhaltsverzeichnis

-   01 - Einstieg
-   02 - Docker / Kubernetes Umsetzung
-   03 - Sicherheitsaspekte
-   04 - Abschluss

## Persönlicher Stand

Ich habe aus dem Betrieb schon einige Erfahrungen mit Virtualisierung gemacht.
Mit Vagrant habe ich bisher noch keine Erfahrungen gemacht.
Virtualisierung und die Automatisierung davon ist für mich aber ein sehr spannendes Thema und ich 
freue mich mehr darüber zu lernen und das in der Zukunft anzuwenden.

Github hatte ich noch nie zuvor benutzt.Ehrlich gesagt habe ich nicht gewusst was das ist.
### Einrichten

## Git bash

1. Git bash herunterladen 
2. Git bash installieren

Anschliessend wird noch das Repository auf den lokalen Computer kopiert.
```
$ git clone https://github.com/mc-b/M300      #Repository klonen
 ```
  
## GitHub Account

1. GitHub Account erstellen
2. Mit Git bash SSH Key erstellen
3. SSH Key dem Agent hinzufügen
4. SSH Key dem GitHub Konto hinzufügen

## Virtualbox

1. Virtualbox herunterladen
2. Virtualbox installieren

## Visual Studio Code

1. Visual Studio Code herunterladen
2. Visual Studio Code installieren
3. Extensions installieren
4. Einstellungen anpassen


---
### Docker-Container
Ein Docker-Container ist eine isolierte Umgebung für das Paketieren und Ausführen von Anwendungen. Docker bietet die Möglichkeit, eine Anwendung in Side-by-Side Containern auszuführen, um eine bessere Rechendichte zu erreichen. Sie können mehrere Container auf einem einzigen Host ausführen. Sie können diese Container einfach von einem Host zu einem anderen Host verschieben.
### Kennt die Docker-Befehle

| Befehl       | Beschreibung                                       |
| ------------ | -------------------------------------------------- |
| docker run   | Führt ein Befehl in einem neuen Container aus      |
| docker start | Startet einen oder mehrere gestoppte Container     |
| docker stop  | Stoppt einen oder mehrere laufende Container       |
| docker build | Erstellt ein Image aus einem Docker-File           |
| docker pull  | Ladet ein Image aus der Registry                   |
| docker push  | Ladet ein Image in die Registry hoch               |
| docker exec  | Führt einen Befehl in einem laufenden Container aus |


### Sicherheitsaspekte

-   Lediglich der Port 80 des Web-Frontends und der Port 8080 der API wurdem via `LoadBalancer` nach Aussen freigegeben
-   Container laufen in einer dedizierten virtuellen Maschine in der Google Cloud
-   Die verwendeten Images definieren einen Benutzer und laufen nicht direkt als root
-   In Kubernetes wurden die Container in einzelne Deployments aufgeteilt

























Persönlicher Wissenstand im Bezug auf die wichtigsten Themen sind dokumentiert (Linux, Virtualisierung, Vagrant, Versionsverwaltung / Git, Mark Down, Systemsicherheit)
Im Betrieb arbeite ich täglich mit Virtuellen Server (ESXI Umgebung). Da mir Vagrant sehr fremd war, fragte ich in der Firma nach, ob sich jemand mit Vagrant auskennt. Leider kannte sich niemand im Team mit Vagrant aus. Dank den ersten Input von Herr Kählin über Vagrant, konnte ich meinen Teamkollegen erzählen was Vagrant ist und was es so macht. Sie fanden das sehr spannend. 




Im ganzen hat mir das Modul sehr Spass gemacht, auch wenn ich zu Beginn sehr viel Schwieriegkeiten hatte.
Dank diesem Modul, weiss ich jetzt wie man Vagrant-Files erstellt und sie anwendet. 
Das Vagrant hilft sehr und erleichtert die Aufgabe und spart sehr viel Zeit. Man kann in einem Vagrant-File mehrere Maschinen erstellen mit verschiedene Konfigurationen wie zB. Netzwerk usw. 
In der Zukunft werde ich sicherlich weiter mit Vagrant arbeiten und experimentieren. 


