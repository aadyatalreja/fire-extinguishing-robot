# Flame Detection and Robotic Motion Control System
This repository contains the source code for a flame detection and robotic motion control system built using Arduino. The system integrates DC motors, a servo motor, flame sensors, and a temperature sensor to detect flames and respond appropriately with motorized actions and a relay-controlled actuator.

## Features
<b> Flame Detection: </b> Utilizes three flame sensors and a temperature sensor to detect fire or high temperatures. <br>
<b> Smooth Motor Control:</b>  Provides acceleration and deceleration for DC motors for smooth movement. <br>
<b> Servo Swivel Action:</b> Swivels a servo motor to simulate a spraying mechanism or other actuating response. <br>
<b> Relay Control:</b>  Activates a relay for further operations, such as triggering an extinguisher. <br>
<b> Forward Movement:</b> Moves the robot forward until a flame is detected. <br>
<b> Interactive Debugging:</b>  Prints system status and sensor readings to the serial monitor. <br>

## Components
1. Microcontroller: Arduino board (compatible with the AFMotor library). <br>
2. Motor Driver: Adafruit Motor Shield. <br>
3. DC Motors: Four motors for robot movement. <br>
4. Servo Motor: Controlled swivel action for spraying.<br>
5. Flame Sensors: Three sensors for flame detection.<br>
6. Temperature Sensor: For additional flame detection criteria.<br>
7. Relay Module: To control external devices, such as extinguishers.<br>

## How It Works
<b> Step 1: Initialization </b>
- Sets up pins, motor speeds, and servo positions.
- Configures flame sensors with internal pull-up resistors.
  
<b> Step 2: Loop </b>
- Continuously monitors flame sensors and the temperature sensor.
- Moves forward if no flame is detected.
- Stops, activates the relay, and performs a servo swivel action when a flame is detected.
  
<b> Step 3: Motor Acceleration/Deceleration </b>
- Gradually changes motor speeds to ensure smooth transitions.
  
<b> Step 4: Servo Swivel Action </b>
- Moves the servo in a predefined pattern (0° to 180° and back).
