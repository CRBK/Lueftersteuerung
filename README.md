# Lueftersteuerung

* geht ein wenig ausführlicher * 

 Lüftergeschwindigkeit per Taster steuern

Um einen Lüfter steuern zu können, muss man seine Versorgungsspannung regulieren. Das macht man mit dem Arduino, indem man per analogWrite Befehl ein PWM Signal ausgibt. Der PWM Wert kann dabei zwischen 0 und 255 liegen, wobei 0 = 0% und 255 = 100% ist.

Mit Hilfe von zwei Tastern wird der PWM Wert schrittweise erhöht, bzw. gesenkt, um so die Geschwindigkeit des Lüfters zu steuern.
Der Code für 3 Pin Lüfter und 4 Pin PWM Lüfter unterscheidet sich dabei nicht, der Aufbau allerdings schon. Den 4 Pin PWM Lüfter kann man ohne zusätzliche Bauteile an eine 12V Stromversorgung und den Arduino anschließen, aber für die Ansteuerung eines 3 Pin Lüfters braucht man noch einen Transistor der über den Arduino angesteuert wird, da die Ausgänge des Arduinos nicht genügend Strom und Spannung liefern um einen Lüfter anzutreiben.
