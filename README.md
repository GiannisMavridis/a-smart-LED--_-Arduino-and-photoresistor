light-activated-LED-_-Arduino
=============================

We build a "smart" LED that turns on only when there is a little ambient light.
If the ambient light is enough,the led automatically turns off .
In some countries the street lights work like this.

The key hardware element we need for this project is a photoresistor(we can also use a phototransistor).
The photoresistor is a light-dependent resistor. Its resistance increases as light intensity decreases and
vice versa.For more information read here http://en.wikipedia.org/wiki/Photoresistor

Our "smart" LED is made up of two small circuits.

-Firstly, it is the photoresistor's circuit that counts the ambient light.It is just a voltage divider circuit.
(see the schematic for more info)

-Also, it is the LED 's circuit. It is just a resistor connected in series with te LED we like to turn on and off.

The Arduino's analog pin A0 is connected to the Vout of the first circuit.
The Arduino's digital pin 7 controls the LED .

The idea is to compare the value,that we read from the pin A0,with a threshold and then to decide whether we should or not
turn on the LED.



