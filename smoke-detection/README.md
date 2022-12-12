## Gas leak and smoke detection system
Accidental gas leaks or fires pose very large threats to property, the environment and human life. Many industrial facilities as well as homes, comprise technological setups to detect gas leaks and fires, and transmit useful notifications like alarms, automatic SMS/calls, etc. This project aims to build a simple prototype gas leak/smoke detection system based on the Arduino MC. Gas, smoke, and temperature sensors are used to detect any accidental gas leaks or fire, and trigger necessary alarms e.g SMS calls, LED flashes, or buzzers.

## Project description
In this project, you will use a gas sensor to determine if there is a gas leak. The sensor will send a signal to the Arduino MC when it detects a high gas/smoke concentration. The Arduino will respond by turning on a buzzer alarm and flashing a red LED. When the gas concentration returns to normal, the green LED will turn on.

## Identification of components
### Arduino Uno (x1)

### MQ2 gas sensor (x1)
- The MQ2 gas sensor is an electronic sensor used for sensing the concentration of gases in the air such as propane, methane, hydrogen, smoke, alcohol, carbon monoxide etc. This sensor detects gas concentrations in the between 300ppm to 10000ppm. `ppm` is `parts-per-million` and is a unit of measure for gas concentration. 
- The gas sensor sends an analog or digital value to the Arduino which represents the gas concentration.
- The MQ2 gas sensor has 4 pins: 1- `VCC`: this pin powers the module, 2- `GND`: the ground pin, 3- `A0`: used to send an analog signal when gas is detected, and 4- `D0`: used to send a digital signal when gas is detected.


### Buzzer alarm
- The buzzer alarm will emit a buzzer sound when it receives a HIGH signal from the Arduino MC.

### Jumper wires
- Jumper wires: M-F (x6); M-M (x6)

### Red LED
- Will flash when gas concentration is high.

### Green LED
- Will flash when gas concentration is low.

### Resistor (220 ohm)
- Use the Arduino manual (page 32) to identify a `220 ohm` resistor. Resistors will be connected to all LEDs. This prevents the LEDs from being destroyed by high current.

## Circuit diagram


## Circuit construction (connections)

- VCC pin of gas sensor to +5V on Arduino.
- Ground pin of gas sensor to Arduino ground.
- A0 pin of gas sensor to analog pin A0 of Arduino. We will not use the D0 pin in this exercise.
- Red LED `+` pin to pin 13 of Arduino through 220 ohm resistor; `-` pin to ground.
- Green LED `+` pin to pin 12 of Arduino through 220 ohm resistor; `-` pin to ground.
- One buzzer pin to pin 7 of Arduino; the other pin on ground of Arduino.


## Arduino program
- Explain the Arduino program to the students.

-