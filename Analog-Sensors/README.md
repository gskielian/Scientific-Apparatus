A common theme in this field will be resetting the Arduino Voltage Reference.




Main link: http://arduino.cc/en/Reference/AnalogReference


```arduino
analogReference(INTERNAL);

```


* DEFAULT
* INTERNAL: the built-in reference:
  * 1.1 volts on the ATmega168 or ATmega328 
  * 2.56 volts on the ATmega8 
  * Arduino Mega Has 2 references (so you will need to specify, see [only for mega](only-for-the-arduino-mega)
* EXTERNAL: the voltage applied to the AREF pin (0 to 5V only) is used as the reference.

###  Only for the Arduino Mega
*  INTERNAL1V1: use the built-in 1.1V reference
*  INTERNAL2V56: use the built-in 2.56V reference
