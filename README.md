Our robot is based on several real-life and fictional car models, and the model that you can see in the second version of the v-photos folder was decided from them.

Now we are going to talk about our robot.

Robot Components
1. Brain
The brain of the robot is the central processing unit (CPU) that acts as the main controller. In the LEGO Spike Prime system, this brain is known as the Hub.

The Hub features an integrated screen to display information and feedback, multiple input/output ports to connect sensors and motors, and Bluetooth and USB connectivity for program loading and communication with other devices, it is also integrated with a gyroscope to keep the robot calibrated at all times.

2. Distance Sensors
This robot is equipped with three distance sensors. These sensors use ultrasonic technology to measure the distance between the robot and objects in the track. Distance sensors are critical for autonomous navigation as they allow the robot to detect obstacles and calculate distances to avoid collisions.

Front Distance Sensor: This sensor is mounted on the front of the robot and is primarily used to detect obstacles directly in the robot's path.

Side Distance Sensors: Mounted on both sides of the robot, these sensors enable the detection of side obstacles and keep the robot aligned to the track, they also assist in making decisions regarding lateral movements or turns.

3. Color Sensor
The robot's color sensor is a versatile tool that can detect different colors. This sensor is placed on the front of the robot, and it   is used to detect the color of the various obstacles in the track.

The color sensor can identify various colors and also measure the intensity of reflected light. This allows the robot to interpret different color signals as action commands, which is essential for navigation.

4. Motors
The robot uses two motors for its movement, one dedicated to providing propulsion and another for steering.

Propulsion Motor: This motor is responsible for moving the robot forward and backward. Its speed and power can be controlled to adjust the robot's travel speed as needed.

Steering Motor: This motor controls the robot's turning. By adjusting its position, the robot can change direction, allowing it to move left or right. The combination of propulsion and steering motors gives the robot the ability to perform complex and precise maneuvers.

Programming and Functionality
The LEGO Spike Prime robot's programming is designed to integrate readings from the distance and color sensors, enabling it to make autonomous decisions about its movement. Here is how a program for this robot might be structured.

1. Initialization
At the start of the program, the robot performs an initial calibration of its sensors to ensure accurate readings. This includes setting the initial position of the motors and configuring the parameters of the distance and color sensors.

2. Sensor Reading
The robot enters a continuous loop where it reads the values from the three distance sensors and the color sensor. These values are stored in variables that are updated in each iteration of the loop.

3. Obstacle Detection
Using the values from the distance sensors, the robot determines if there are any nearby obstacles in its path or on its sides. For example:
The side distance sensors are used to detect if the spaces to the sides are clear for a safe turn.

4. Color Interpretation
The color sensor allows the robot to interpret signals in its environment. For example, if the robot detects a red or green object in the front, it might interpret this as a signal to turn right or left.

5. Decision Making
Based on the readings from the distance and color sensors, the robot decides on the action to take. A simple algorithm might be:

If the front distance sensor detects a nearby obstacle, check the side sensors.
If the right side is clear, turn right.
If the left side is clear, turn left.
If a specific color is detected in the front, execute the associated action (e.g., turn or stop).
6. Movement
The decisions made are translated into commands for the motors. If the robot decides to move forward, the propulsion motor is activated to move the robot forward. If it needs to turn, the steering motor adjusts the robot's orientation in the desired direction.
