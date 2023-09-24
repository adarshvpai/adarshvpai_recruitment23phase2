## Embedded

## Basics of Arduino

Arduino is tool that helps you control electronic stuff with code

   ## Arduino Trifecta
   
   1. Hardware
   2. IDE
   3. Code

## Arduino Basic Projects

   ## 1. Ultrasonic Interface
   
   1. Simple Ultrasonic Interface in TinkerCAD that can detect the approximate distance from an object and display it in the serial monitor.
   2. Components required: Arduino Uno(AU), Ultrasonic Distance Sensor(USDS), Connecting wires.
   3. The 5V pin of AU was connected to the VCC of USDS.
   4. The GND of AU was connected to GND of USDS.
   5. The digital pin D10 of AU was connected to TRIGG of USDS.
   6. The digital pin D9 of AU was connected to ECHO of USDS.
   7. Necessary Code for the project was written in the Code tab of AU.
   8. When the simulation was turned on the distance of the object was displayed on the Serial Monitor.

  ## 2. Light Intensity Measurement using LDR

  1. Simple LDR circuit with Arduino and Multimeter to measure the intesity of the light.
  2. Components required: Arduino Uno(AU), Photoresistor(LDR), Red LED, Voltage multimeter,2 1k ohm resistor, Connecting Wires.
  3. Connect Analog A0 pin of AU to LDR terminal 1.
  4. Connect 5V of Au to LDR terminal 2.
  5. Connect GND of LDR to terminal 2 of LDR, cathode of Red LED and negative of multimeter.
  6. Connect 1k ohm resistor between GND of AU and terminal 2 of Red LED.
  7. Connect Digital pin D9 to anode of Red LED and positive of multimeter.
  8.  Necessary Code for the project was written in the Code tab of AU.
  9.  When the simulation was turned on we can adjust the light above the photoresistor which will change the value in multimeter and the intensity of the Red LED.

  ## 3. Temperature Sensor

  1. A temperature sensor circuit with smoke sensor and buzzer
  2. Components required: Arduino Uno(AU), Temperatur Sensor(TMP36), Gas Sensor, Piezo Buzzer, Red LED, 1k ohm resistor, Connecting wires
  3. Connect GND of Au to GND of TMP, Negative of buzzer and H1,A2 port of Gas Sensor, cathode of Red LED.
  4. Connect 5V of AU to Power of TMP, B1,H@,B2 of Gas Sensor.
  5. Connect 1k ohm resistor in between GND and A2 of Gas Sensor.
  6. Connect the Analog pin A0 to A1 of Gas sensor.
  7. Connect the Analog pin A1 to Vout of TMP.
  8. Connect the Digital pin D13 to anode of Red LED.
  9. Connect !k ohm resistor in between D13 pin and anode of Red LED.
  10. Connect the Digital pin D7 to positive of Piezo Buzzer.
  11. Necessary Code for the project was written in the Code tab of AU.
  12.  When the simulation was turned on we can adjust the temperature above the TMP36 and we can adjust the smoke above the gas sensor
  13.  The Temp Reading and Smoke Reading will be displayed in the Serial Monitor and if the Gas reading goes above 100 the piezo buzzer will turn on.
