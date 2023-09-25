## Embedded

## Basics of Arduino

Arduino is tool that helps you control electronic stuff with code

   ## Arduino Trifecta
   
   1. Hardware
   2. IDE
   3. Code

## Basic Serial Communication Protocol

Types of Communication Protocol:
1. Synchronous Comunication Protocol(SPI,I2C)
2. Asynchronous Comunication Protocol(UART,CAN)

   ## UART (Universal Asynchronous Receiver Transmitter)
   1. It is an Asynchronous Communication Protocol.
   2. Is ia Ad-Hoc type of Topology.
   3. It consist of two main components:Transmitter and Receiver.
   4. It uses Start bit and Stop bit before and after each transmission of data.
   5. It has Baud rate that defines the speed at which data is transmitted and both transmitter and receiver should be on same baud rate.
   6. UART is highly configurable.
   7. UART communication is reliable for short to moderate distances.
   8. UART is commonly used in embedded systems for communication between microcontrollers, sensors, display modules, GPS modules, and other peripheral devices.
   9. It is also used for communication with computers and other external equipment.
      Programming Approach
      Bit Banging:
      Bit banging is a method of serial communication used in microcontroller and embedded systems programming. It involves manually controlling the state of           individual digital pins to transmit or receive data without relying on dedicated hardware communication peripherals like UART, SPI, or I2C. Instead, the          microcontroller or embedded system's firmware directly manipulates the pins to send or receive individual bits of data.

      UART Peripherals:
      It ia method in which the Transmit register transfers full data to shift register and the shift register and it transfers this data byte by byte to the
      next device were the process is called parallel in serial out. The shift register of the next device collect the data one by one and transfer it to the
      receiver register all at once were the process is called serial in parallel out.

      UART Configuration

      1. Clock configuration
      2. Data Loading
      3. Data Transmission
      4. Monitor data: Looping Method or Interrupt Method

      Advantages of UART:
      - Easy to interface
      - Less Hardware
      - Less Software Complications

      Disadvantages of UART
      - Synchronizing Baud Rate
      - Only two devices can be connected
      - No Acknowledgement
        
   ## I2C (Inter-Integrated Circuit)

   1. It is a Synchronous Comunication Protocol, invented by Philips.
   2. I2C uses only two wires for communication - one for data (SDA) and one for the clock (SCL).
   3. I2C network uses master-slave architecture, there is one master device and one or more slave devices.
   4. Both the data (SDA) and clock (SCL) lines are bidirectional, allowing data to flow in both directions between the master and slave devices
   5. Each slave device on the bus has a unique 7-bit or 10-bit address, allowing the master to select a specific device for communication.
   6. The master device generates the clock signal (SCL), ensuring synchronization of data transmission between devices.
   7. Data is transferred in frames, with each frame consisting of 8 bits (1 byte). It may include a 9th bit for acknowledgment or other purposes.
   8. After each byte of data is sent, the receiving device acknowledges its successful reception by pulling the SDA line low (ACK) or leaving it high (NACK) to signal an error or end of communication.
   9. I2C supports multiple clock speeds, such as standard mode (100 kbps), fast mode (400 kbps), and high-speed mode (up to 3.4 Mbps)
   10. I2C is suitable for short-distance communication within a single board or between closely located devices due to its limited range.
   11. I2C is relatively simple compared to other communication protocols like SPI or UART.
   Bus Arbitration:
   It is the process of determining which device on the I2C bus gets to transmit data or initiate a communication transaction when multiple devices are connected to the same bus. I2C is a multi-master communication protocol, which means that multiple devices can be connected to the same bus, and they can all act as both masters and slaves. As a result, there needs to be a way to resolve conflicts when multiple devices try to communicate simultaneously.
   Clock Stretching:
   It a feature that allows one of the devices on the bus, typically the slave device, to temporarily hold the SCL (Serial Clock) line low to slow down the master device's clock when it needs more time to process data. This helps in preventing data overrun and ensuring reliable communication between devices with potentially different processing speeds or response times.
   
   Advantages of I2C
   - Two wires only
   - Multimater Compatibility
   - Better Error Handling
   - Different mode flexibility for Slave

   Disadvantages of I2C
   - Less Flexibility for Slave address
   - Complexity of Firmware
   - Increased Data Overhead
   - Hardware Limitations
   - Bus Topology
   ## SPI (Serial Perpheral Interface)

   1. It is a Synchronous Comunication Protocol.
   2. SPI supports multiple slave devices on the same bus.
   3. Each slave device has a unique chip select (CS) or slave select (SS) line that the master uses to select the specific slave with which it wants to communicate.
   4. SPI allows for full-duplex communication, which means that data can be transmitted in both directions simultaneously.This is achieved by having separate data lines for sending data from the master to the slave (MOSI - Master Out Slave In) and from the slave to the master (MISO - Master In Slave Out).
   5.  SPI transfers data serially, one bit at a time. The data bits are sent sequentially over the MOSI and MISO lines. Data is usually sent in 8-bit or 16-bit chunks, but the word size can be configured based on the devices involved.
   6. SPI supports two clock configuration modes: CPOL (Clock Polarity) and CPHA (Clock Phase).
   7. SPI usually consists of at least four pins: MOSI, MISO, SCLK (Serial Clock), and SS/CS (Slave Select/Chip Select).
   8. Unlike I2C, SPI does not involve addressing in the data packets. The master selects a specific slave by asserting the appropriate CS/SS line.
   9. SPI is suitable for short-distance communication, typically within a single PCB (Printed Circuit Board) or between closely located devices.
   10. SPI has minimal protocol overhead since it does not include addressing or acknowledgment signals.

   Advantages of SPI
   - Low Power Consumption
   - SPI is faster than I2C
   - Easy to Interface
   - Different Modes of Transmission

   Disadvantages of SPI
   - Atleast 4 connections are required
   - Does not support Multimaster
   - More GPIOs for more Slaves
     
   ## CAN (Control Area Network)

   1. It is an Asynchronous Communication Protocol, invented by Robert Bosch.
   2. CAN typically uses a two-wire bus system: one wire for transmitting data (CAN-High or CAN-H) and one wire for receiving data (CAN-Low or CAN-L).
   3. It helps to reduce electromagnetic interference (EMI) and ensures reliable data transfer.
   4. CAN supports a multi-master architecture, meaning that multiple ECUs can simultaneously transmit and receive data on the same bus without a centralized master controller.
   5. CAN offers deterministic communication, meaning that messages have a predictable and guaranteed transmission time.
   6. CAN uses a message-based communication model. Data is organized into frames, with each frame containing an identifier (ID) that defines the message's priority and content.
   7. CAN uses a non-destructive bitwise arbitration mechanism to determine which node gets to transmit data when multiple nodes attempt to send messages simultaneously.
   8. CAN incorporates built-in error detection and handling mechanisms. Nodes monitor the bus for errors such as bit errors, frame errors, and other fault conditions. When errors occur, nodes can retransmit       data or take appropriate actions.
   9. CAN allows for message prioritization using the CAN identifier (ID). Lower ID values represent higher-priority messages, which ensures critical data is transmitted before less critical data.
   10. CAN is extensible and scalable, making it suitable for a wide range of applications. CAN networks can range from a few nodes to hundreds or even thousands of nodes interconnected through bridges or          gateways.
   11. Can network can continue to operate even if one or more nodes fail.
   12. CAN is widely used in the automotive industry for various applications, including engine control, vehicle diagnostics, and infotainment systems.
   13. CAN is standardized under ISO 11898, which defines the physical and data-link layer specifications.
   14. CAN is known for its high reliability and robustness, making it suitable for demanding environments where noise and harsh conditions are common.

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
   12. When the simulation was turned on we can adjust the temperature above the TMP36 and we can adjust the smoke above the gas sensor
   13. The Temp Reading and Smoke Reading will be displayed in the Serial Monitor and if the Gas reading goes above 100 the piezo buzzer will turn on. 

   ## 4. Password Protected Security System.
 
   1. It is a Password protected System which need password to enter.
   2. Components Required: Arduino Uno(AU), Keypad 4X4, Red LED, Green LED, Piezo Buzzer, 2 1k ohm resistor, Connecting Wires.
   3. Connect GND of AU to cathode of Red LED, cathode of Green LED, negativ of Piezo Buzzer.
   4. The 1k resistors are connected between GNd of Au and both of Green LED and Red LED.
   5. The Digital pins D2,D3,D4,D5,D6,D7,D8,D9 are connected to Column 4,3,2,1 pins and Row 4,3,2,1 pins
   6. The Digital pin D10 is connected to anode of Red LED.
   7. The Digital pin D11 is connected to anode of Green LED.
   8. The Digital pin D12 is connected to positive of Piezo Buzzer.
   9. Necessary Code for the project was written in the Code tab of AU.
   10. When the simulation was turned on in Serial monitor a message is displayed to enter the password.
   11. If we enter the correct password the Green LED will light up.
   12. If we enter the wrong password the Red LED will light up and the Buzzer will turn on. 

## Arduino Challenges
   
   ## Traffic Light System
   1. It is a traffic light system in which each time we press the button the LEDs will change.
   2. Components required: Arduino Uno(AU), Red LED, Yellow LED, Green LED, 3 250 ohm resistor, Push Button, 1ok ohm resistor, Connecting Wires.
   3. Connect GND of AU to cathode of Red, Green, Yellow LEDs and terminal 2a of push button.
   4. Connect Digital pin D2 of AU to the terminal 1b of push button.
   5. Connect the 10k ohm resistor between Digital pin of AU and terminal 1b of push button.
   6. Connect the Digital pins D3,D4,D5 of AU and anode of Red, Green, Yellow LEDs.
   7. Connect the 250 ohm resistor between Digital pins of AU and anode of Red, Green, Yellow LEDs.
   8. Necessary Code for the project was written in the Code tab of AU.
   9. When the simulation was turned on we can use the push button to turn on the led and change the colour from red to green.

   ## Servomotor
   1. It is circuit with Potentiometer and Servomotor servo motor will rotate according to the potentiometer value.
   2. Components required: Arduino Uno(AU), Potentiometer, Servomotor, Connecting wires.
   3. Connect GND of AU to the terminal 1 of Potentiometer and Ground of Servomotor.
   4. Connect Analog pin A0 to the Wiper pin of Potentiometer.
   5. Connect terminal 2 of Potentiometer to the power of Servomotor.
   6. Connect the Digital pin D9 to the Signal of Servomotor.
   7. Necessary Code for the project was written in the Code tab of AU.
   8. When the simulation was turned on by adjusting the value in Potentiometer we can make the Servomotor rotate accordingly

   ## Quiz
   1. It  is cicuit involving LCD display where we conduct the quiz.
   2. Components required: Arduino Uno(AU), LCD 16X2 I2C, 4 Push buttons, 4 1ok ohm resistors.
   3. Connect 5V of AU to VCC of LCD and terminal 1b of 4 push buttons.
   4. Connect GND of AU to the GND of LCD and terminal 2a of 4 push buttons.
   5. Connect SDA of AU to SDA of LCD.
   6. Connect SCL of AU to SCL of LCD.
   7. Connect Digital pins D2,D3,D4,D5 to terminal 2a of respective 4 push buttons.
   8. Connect 10k ohm resistors between Digital pins and terminal 2a of 4 push buttons.
   9. Necessary Code for the project was written in the Code tab of AU.
   10. When the simulation was turned on the quiz will be displayed on the LCD screen and we can choose the answer using the 4 push buttons.
       
    

