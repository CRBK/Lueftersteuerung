#  Projekt: Temperaturgesteuerter Lüfter

Ziel: Ziel dieses Projektes ist es den Temperatursensor MAX6675 am Arduino auszulesen und je nach Schwellwert ein Relais zu schalten welches am Lüfter angeschlossen ist.

## Benötigte Bauteile
•	Einfaches Relais für den Arduino
•	Thermosensor MAX6675
•	Arduino
•	Breadboard
•	Breadboardkabel
 
## Thermosensormodul MAX6675 
Das Modul MAX6675 hat zwei Anschlusseiten einmal zum Microcontroller (z.b Arduino) und einmal zum Sensor ( + und -).
Das Modul wird wie folgt angeschlossen

-Modul MAX6675                           Arduino
-GND (ground)	                           GND
-VCC	                                    5V
-SCK (serial clock)	                     10
-CS (chip select)	                       9
-SO (serial output) 	                    8
 
Um das Modul anzusteuern, muss eine Bibliothek runtergeladen werden, welche man im Internet findet. Diese Bibliothek muss über den Quellcode eingebunden werden. Im Quellcode kann unter anderem der Schwellwert der Temperatur eingestellt werden ab wann das Relais durchschalten soll. Außerdem kann im Quellcode angegeben werden ob die Einheit Celsius oder Fahrenheit sein soll.
