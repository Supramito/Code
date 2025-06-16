# Code
Detailed Explanation of Code Sections:
Imports and Initialization:

The vex library is imported to access the robot's hardware components and functionalities.
A brain object is created to interface with the robot's main controller, allowing for screen output and control.
Motor and Sensor Setup:

Two motors are initialized for the left and right wheels. The left motor spins in the default forward direction, while the right motor is set to spin in reverse to facilitate turning.
A distance sensor is initialized to detect obstacles in the robot's path, connected to a specific port.
Movement Functions:

moveForward(): This function spins both motors forward, allowing the robot to move straight.
stopRobot(): This function stops both motors, bringing the robot to a complete stop.
turnRight(): This function spins the left motor forward and the right motor in reverse, causing the robot to turn right.
turnLeft(): This function spins the left motor in reverse and the right motor forward, causing the robot to turn left.
Main Function:

The main() function initializes the robot's operation and contains an infinite loop that continuously checks for obstacles while moving forward.
The distance sensor checks for obstacles, and if one is detected within 300 mm, the robot stops, prints a message, turns right to avoid the obstacle, and waits before resuming forward movement.
Delays:

Small delays are added to prevent overwhelming the CPU and to control the timing of movements, ensuring smooth operation.
