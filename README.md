![rc_Car](https://github.com/at-cs-ubbcluj-ro/team-project-smart-remote-control-car/assets/91084651/d54ffddb-ef7d-462a-a67a-ae3d00ca4573)

TEAM PROJECT - Bluetooth Controled Car

This Arduino project involves building a remote control smart car that combines hardware and software to create an interactive device. The car is controlled remotely using a smartphone app connected via Bluetooth. It features an auto-driving mode and obstacle detection, with a sensor that makes the car turn left or right to avoid running into obstacles. 


Members:
- <b>Bodnariu Nicolae-Matei</b> - Grupa 231
     * Hardware & Arduino Code
- <b>Dămătar Eusebiu-Anton</b> - Grupa 232
     * Mobile App
- <b>Tomuța Răzvan Claudiu</b> - Grupa 237
     * Arduino Code and Team Organization

 
Components:
- Arduino UNO R3 Board
- L293D Motor Shield - https://www.sigmanortec.ro/Shield-Modul-L293D-p125162435
- Bluetooth HC-05 Module - https://cleste.ro/modul-bluetooth-hc-05.html
- 2x Motor with reductor + plastic wheel - https://www.sigmanortec.ro/Kit-Motor-reductor-Roata-plastic-cu-cauciuc-p134585625
- HC-SR04 Ultrasonic Sensor - https://cleste.ro/senzor-ultrasonic-hc-sr04.html
- Breadboard
- 2x 9V Batteries
- Wires


Pre-requisite:
- Arduino Uno R3 - https://docs.arduino.cc/hardware/uno-rev3/
- Arduino IDE - https://docs.arduino.cc/
- Arduino Adafruit Motor Shield Library - https://www.arduino.cc/reference/en/libraries/adafruit-motor-shield-library/


Running:

1. Remote Control Navigation
The Arduino car can be navigated in four directions—forward, backward, left, and right—using commands from an external application, using a smartphone app connected via Bluetooth. This allows for precise and user-directed control over the car's movements.

Functionality in Detail:

- Forward Movement: When the app sends a forward command, the Arduino activates both motors to rotate in the same direction, propelling the car forward.
- Backward Movement: For backward movement, the Arduino reverses the polarity of the motor signals, causing the wheels to rotate in the opposite direction.
- Left Turn: To turn left, the Arduino rotates the motor on the left side backward while the right motor runs forward, causing the car to pivot left.
- Right Turn: Similarly, to turn right, the Arduino rotates the motor on the right side backward while the left motor runs forward, causing the car to pivot right.

2. Obstacle Detection
The car has a HC-SR04 Ultrasonic Sensor used for obstacle detection.
- if the car runs forward in remote control mode and an obstacle is detected, the car stops
- if the car is in auto-driving mode, the behaviour is described in the next part

3. Auto-driving Mode
The Arduino car drives itself when the mode is activated from the app.
- The car runs forward until it finds an obstacle
- A direction between left and right is randomly chosen and the car turns
- Previous steps repeat until Auto-driving mode is stoped or baterry runs out :)))


Mobile Application Interface 

<p align="center">
<img src="https://github.com/at-cs-ubbcluj-ro/team-project-smart-remote-control-car/assets/91084651/fd48aa5d-8711-470b-b075-3290310d1b0b" width="300">
</p>

