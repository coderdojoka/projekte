# Roboter Auto Workshop


## Notes
Dieser Workshop wird mit dem ELEGOO Smart Robot Car Kit V3.0 Uno ausgeführt.
In dem Kit befinden sich ein UNO R3, ein Ultraschallsensor, ein Line Tracking Modul, ein Bluetooth Modul und ein Infrarotsensor mit Fernbedienung.
Auf der Elegoo-Website gibt es einen Download-Link für das Kit in dem man eine Übersicht zum Auto, die Bauanleitung und Beispielcode für 5 Lessons in verschiedenen Sprachen findet:
- https://www.elegoo.com/download/
Außerdem gibt es die Elegoo Bluetooth App für iOS und Android mit der Befehle an den Roboter über Bluetooth gesendet werden können:
- https://itunes.apple.com/us/app/elegoo-ble-tool/id1195318538?mt=8
- https://play.google.com/store/apps/details?id=com.femtoapp.rootsence.bleutils

## Workshops
Bei der Reihenfolge der einzelnen Workshops haben wir uns ungefähr an den Projekten die Elegoo für das Robot Car Kit vorschlägt orientiert. In jedem Teil können einzelne Code-Teile schon vorgegeben und manche Funktionen in einer Präsentation gezeigt werden damit der Code abgetippt werden kann. Mit diesen Teilen kann dann herumexperimentiert werden. 

### 1 - Einführung (und ggf. Arduino IDE Installation)
Hier können die Kinder den Roboter einfache Bewegungen wie vorwärts/rückwärts und links/rechts fahren lassen. Dazu werden das Arduino IDE Setup und Konzept (setup(), loop()) vorgestellt. Eventuell kann man auf einem USB-Stick noch zusätzlich den Arduino IDE-Download mitbringen um die Installation zu erleichtern:
- https://www.arduino.cc/en/Main/Software

### 2 - Ultraschallsensor
Im zweiten Teil wird der Ultraschallsensor des Roboter Autos genutzt um Kollisionen mit Hindernissen zu vermeiden. Dazu muss erst einmal der Servo gesteuert werden um den Sensor geradeaus, links oder rechts auszurichten. Anschließend kann ein Puls gesendet und empfangen werden und über eine einfache (vorgegebene) Funktion mit dem empfangenen Signal die Entfernung ausgerechnet werden.
Erst einmal soll der Roboter einfach vor einer Wand stoppen, anschließend kann ein einfaches "Labyrinth" (zum Beispiel aus Stühlen) aufgebaut werden aus dem der Roboter herausfinden muss.

### 3 - Serielle Schnittstelle nutzen
Der Roboter kann auch genutzt werden um Nachrichten über die serielle Schnittstellt zu senden oder zu empfangen. Dazu werden einfache print-Befehle eingeführt und der serielle Monitor in der Arduino IDE gezeigt. Das kann auch später bei der Bluetooth-/Infrarotsteuerung helfen.

### 4 - Steuerung über die Infrarot-Fernbedienung
Erst einmal werden Signale über die Infrarot-Fernbedienung gesendet die als HEX-Code vom Roboter interpretiert werden. Wenn die Tastenbelegung dem jeweiligen Code zugeordnet worden ist können diese Befehle dann als vorwärts/rückwärts/abbiegen-Befehle genutzt werden um den Roboter fernzusteuern.

### 5 - Linienverfolgung
Dafür wird erst einmal das schwarze Tape (im Kit enthalten) auf einem weißen Papier genutzt um zu gucken wie sich die Ausgabe des Liniensensors ändert wenn schwarz oder weiß wahrgenommen wird. Dann kann man eine etwas kompliziertere Form auf einen Tisch kleben (um einen helleren Hintergrund zu haben) der die Roboter folgen müssen. 

### Verschiedene
- GPS-Projekt: Verbindung des Roboters mit einem GPS-Modul um ihn über die Angabe von GPS-Daten fahren zu lassen
- BLE-App: Steuerung des Roboters über die BLE-App, funktioniert relativ selbsterklärend, allerdings ist die Verbindung zum Roboter manchmal etwas aufwendiger und muss jedes mal neu erfolgen wenn das Programm neu geladen wurde. 
