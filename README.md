HEAD MOVEMENT BASED CURSOR CONTROL 
WITH HUMAN COMPUTER INTERACTION
It focuses on the design and implementation of a 
head mouse, an innovative assistive technology aimed at enhancing accessibility and 
independence for such individuals. The system utilizes a microcontroller combined with a 
gyroscope to create a cost-effective solution. Its core functionality involves translating head 
movements into cursor movements, enabling users to control devices without conventional 
input methods. The system also integrates connectivity features, providing flexibility for use 
in various environments. Furthermore, it incorporates a lithium battery charging mechanism 
(03962A) to ensure sustained and reliable power, enhancing its portability

Features of the Code:
MPU6050 Sensor:
Reads gyroscope data (gx, gy) for head movement detection.
Maps head tilts to horizontal (X) and vertical (Y) cursor movements.

Mouse Emulation:
Utilizes the Arduino HID library to simulate mouse actions.
Sends cursor movements to a connected device.

Sensitivity Adjustment:
The sensitivity variable allows fine-tuning of the cursor's responsiveness.

Debugging:
Prints the cursor movement values to the Serial Monitor for testing and calibration.

Hardware Connections:

MPU6050 to Arduino Pro Micro:
VCC → 5V
GND → GND
SDA → Pin A4
SCL → Pin A5

Power Supply:
Connect the lithium battery charger module's output to the Arduino Pro Micro's VIN and GND.

Required Libraries:
Install the MPU6050 library for sensor communication.
Install the HID-Project library for mouse emulation.

Calibration:
Adjust the sensitivity variable in the code to suit the user's head movements.
Ensure that the MPU6050 is placed securely for accurate readings.

Notes:
Ensure your Arduino IDE is set to the correct board and port.
The Arduino Pro Micro supports USB HID, allowing it to emulate mouse movements.                                                                    
