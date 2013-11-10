A common theme in this field will be resetting the Arduino Voltage Reference.


By adjusting the voltage scale, you can "amplify" using software (or save on an analog amp stage).

For example, a certain dissolved oxygen sensor has a range from 0 to 50mV, if you find a good 60mV voltage reference (possibly by using a voltage divider on the 5v or 3.3v pin), then you would virtually have a full scale without having to amplify the signal further.

### Code to include in the setup:

```arduino
analogReference(INTERNAL);
```

### General Options

* DEFAULT
* INTERNAL: the built-in reference:
  * 1.1 volts on the ATmega168 or ATmega328 
  * 2.56 volts on the ATmega8 
  * *Note: Arduino Mega Has 2 references (so you will need to specify, see [only for mega](#only-for-the-arduino-mega)*
* EXTERNAL: You Choose the Voltage Reference (must be between 0V and 5V for Uno, ref voltage cannot be negative or exceed whichever voltage your board runs on)

###  Only for the Arduino Mega
*  INTERNAL1V1: use the built-in 1.1V reference
*  INTERNAL2V56: use the built-in 2.56V reference

#### Further Information
For further information check out this link: http://arduino.cc/en/Reference/AnalogReference
