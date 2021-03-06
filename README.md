# M300_LB02

## Inhaltsverzeichnis

-   01 - Einstieg
-   02 - Docker / Kubernetes Umsetzung
-   03 - Sicherheitsaspekte
-   04 - Abschluss

### Persönlicher Stand

Ich habe aus dem Betrieb schon einige Erfahrungen mit Virtualisierung gemacht.
Mit Vagrant habe ich bisher noch keine Erfahrungen gemacht.
Virtualisierung und die Automatisierung davon ist für mich aber ein sehr spannendes Thema und ich 
freue mich mehr darüber zu lernen und das in der Zukunft anzuwenden.

Github hatte ich noch nie zuvor benutzt.Ehrlich gesagt habe ich nicht gewusst was das ist.
### Einrichten

### Git bash

1. Git bash herunterladen 
2. Git bash installieren

Anschliessend wird noch das Repository auf den lokalen Computer kopiert.
```
$ git clone https://github.com/mc-b/M300      #Repository klonen
 ```
  
### GitHub Account

1. GitHub Account erstellen
2. Mit Git bash SSH Key erstellen
3. SSH Key dem Agent hinzufügen
4. SSH Key dem GitHub Konto hinzufügen

### Virtualbox

1. Virtualbox herunterladen
2. Virtualbox installieren

### Visual Studio Code

1. Visual Studio Code herunterladen
2. Visual Studio Code installieren
3. Extensions installieren
4. Einstellungen anpassen


---
### Dockerfile
Dockerfile ist eine Datei, die verwendet wird, um Images zu erstellen, indem Anweisungen aus einer Datei gelesen werden. Der Standardname wird als Dockerfile verwendet. Sie können eine Dockerdatei im aktuellen Verzeichnis mit spezifischen Anweisungen erstellen und ein benutzerdefiniertes Image nach Ihren Anforderungen erstellen.
### Kubernetes
Kubernetes ist eine beliebte Open-Source-Plattform für die Container-Orchestrierung - also für die Verwaltung von Anwendungen, die aus mehreren, weitgehend in sich geschlossenen Laufzeiten, den sogenannten Containern, bestehen. 
### Docker-Compose
Docker Compose ist ein weiteres optimales Werkzeug für Docker zum Einrichten von Multi-Container-Umgebungen. Erstellen Sie damit eine einzige Compose-Datei mit der Definition aller Container mit ihren Umgebungen. Sie können ganz einfach einen einzigen Befehl verwenden, um Images zu erstellen und alle Container auszuführen.
### Docker-Desktop
Man muss Docker Desktop herunterladen und installieren, damit man Docker unter Windows bedienen kann. Sobald man das installiert hat, kann man im Hyper-V eine Virtuelle Maschine aufinden. 
### Docker-Image
Ein Image ist eine unveränderliche Datei, die im Wesentlichen eine Momentaufnahme eines Containers ist. Die Images können mit dem Build-Befehl erstellt werden.
### Docker-Container
Ein Docker-Container ist eine isolierte Umgebung für das Paketieren und Ausführen von Anwendungen. Docker bietet die Möglichkeit, eine Anwendung in Side-by-Side Containern auszuführen, um eine bessere Rechendichte zu erreichen. Sie können mehrere Container auf einem einzigen Host ausführen. Sie können diese Container einfach von einem Host zu einem anderen Host verschieben.
### Kennt die Docker-Befehle

| Befehle           | Beschreibung
| --------------    | ------------------------------------
| docker run        | Befehl zum Starten neuer Container
| docker ps         | Überblick über die aktuellen Container, wie z.B. Namen, IDs und Status                                            
| docker images     | Liste lokaler Images aus, wobei Informationen zu Repository-Namen, Tag-Namen und Grösse enthalten sind
| docker rm         | Entfernt einen oder mehrere Container. Gibt die Namen oder IDs erfolgreich gelöschter Container zurück
| docker rmi        | Löscht das oder die angegebenen Images. Diese werden durch ihre ID oder Repository- und Tag-Namen spezifiziert
| docker start      | Startet einen (oder mehrere) gestoppte Container
| docker stop       | Stoppt einen oder mehrere Container (ohne sie zu entfernen). Nach dem Aufruf von docker stop für einen Container wird er in den Status »exited« überführt.
|  docker kill      | Schickt ein Signal an den Hauptprozess (PID 1) in einem Container. Standardmässig wird SIGKILL gesendet, womit der Container sofort stoppt.
| docker logs       | Gibt die "Logs" für einen Container aus. Dabei handelt es sich einfach um alles, was innerhalb des Containers nach STDERR oder STDOUT geschrieben wurde.
| docker inspect    | Gibt umfangreiche Informationen zu Containern oder Images aus. Dazu gehören die meisten Konfigurationsoptionen und Netzwerkeinstellungen sowie Volumes-Mappings.
| docker diff       | Gibt die Änderungen am Dateisystem des Containers verglichen mit dem Image aus, aus dem er gestartet wurde.
| docker top        | Gibt Informationen zu den laufenden Prozessen in einem angegebenen Container aus.
| docker build      | Der Befehl docker build erfordert ein Dockerfile und einen Build Context. 


### Sicherheitsaspekte

-   Lediglich der Port 80 des Web-Frontends und der Port 8080 der nach Aussen freigegeben wurde
-   Container laufen in einer dedizierten virtuellen Maschine in der Google Cloud


## Netzwerkplan Nginx
+---------------------------------------------------------------+
! Container-Engine: Docker                                      !	
+---------------------------------------------------------------+
! Gast OS: Ubuntu 16.04                                         !	
+---------------------------------------------------------------+
! Hypervisor: VirtualBox                                        !	
+---------------------------------------------------------------+
! Host-OS: Windows 10                                           !	
+---------------------------------------------------------------+
! Notebook - Schulnetz 10.x.x.x                                 !                 
+---------------------------------------------------------------+




### Testfälle

| Testfall                                                                                                                               | Resultat                                                                                                               |
| -------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| Vom Client (192.168.30.9) auf http://192.168.30.20/ zugreifen                                                                          | Funktioniert. Die Homepage des Webservers wird angezeigt auf alle Geräte die sich im lokalen Netz befinden                                                                                                       


*docker image ls* = mit diesem Befehl sieht man ob das Image erstellt wurde (test1)
*curl http://localhost:8080* = Hier kann man testen ob der Webserver überhaupt funktioniert, oder einfach im Browser localhost eingeben. Es erscheint der Inhalt der index.html Datei





## Persönlicher Wissenstand im Bezug auf die wichtigsten Themen sind dokumentiert (Linux, Virtualisierung, Vagrant, Versionsverwaltung / Git, Mark Down, Systemsicherheit)

Im Betrieb arbeite ich täglich mit Virtuellen Server (ESXI Umgebung). Da mir Docker und Vagrant sehr fremd war, fragte ich in der Firma nach, ob sich jemand mit Docker auskennt oder sogar das benutzt. Leider fand ich niemand in der Firma der das "beherrscht". Ich musste das selbst erlernen und mit Hilfe der Inputs vom Herr Kählin konnte ich etwas erstellen. Bevor ich mit Docker begonnen habe machte ich mich schlau wie das überhaupt funktioniert. Herr Kählin erklärte das uns und zeigte sogar noch ein Video dazu, aber ich hatte es nicht zu 100% verstanden und machte mich im Internet schlau, damit ich das verstehe. 



## Reflexion
Im ganzen hat mir das Modul sehr Spass gemacht, auch wenn ich zu Beginn sehr viel Schwieriegkeiten hatte.
Dank diesem Modul, weiss ich jetzt wie man Dockerfiles und Images erstellt und sie anwendet. 
Das Docker hilft sehr und erleichtert die Aufgabe und spart sehr viel Zeit und Ressourcen! 
In der Zukunft werde ich sicherlich weiter mit Docker arbeiten und experimentieren. 


