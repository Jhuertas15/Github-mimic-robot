Our robot is based on several real-life and fictional car models, and the model that you can see in the second version of the v-photos folder was decided from them.
The mechanism is based on electric cars like the Tesla which uses electric motors to get instant acceleration, the cars has no gears so it means it has no torque but the speed of the robot is decided specifically to be fast but at the same time precise.
The design we tried for our robot was the Octane from a the popular game Rocket League, but in the building process, the size of the car was too big for the format and we had to scrap the idea. The design now is not based on anything but its made to be functional for the competition.

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
The LEGO Spike Prime robot's programming is designed to integrate readings from the distance and color sensors, enabling it to make autonomous decisions about its movement. Here is how a program for this robot is structured.

1. Initialization
At the start of the program, the robot performs an initial calibration of its sensors to ensure accurate readings. This includes setting the initial position of the motors and configuring the parameters of the distance and color sensors.

2. Sensor Reading
The robot enters a continuous loop where it reads the values from the three distance sensors and the color sensor. These values are stored in variables that are updated in each iteration of the loop.

3. Obstacle Detection
Using the values from the distance sensors, the robot determines if there are any nearby obstacles in its path or on its sides. For example:
The side distance sensors are used to detect if the spaces to the sides are clear for a safe turn.
The front sensor is used to detect how far the wall is from the robot and when is the right time to turn.

5. Color Interpretation
The color sensor allows the robot to interpret signals in its environment. For example, if the robot detects a red or green object in the front, it might interpret this as a signal to turn right or left.

6. Decision Making
Based on the readings from the distance and color sensors, the robot decides on the action to take. A simple algorithm might be:

If the front distance sensor detects a nearby obstacle, check the side sensors.
If the right side is clear, turn right.
If the left side is clear, turn left.
If a specific color is detected in the front, execute the associated action (e.g., turn or stop).

6. Movement
The decisions made are translated into commands for the motors. If the robot decides to move forward, the propulsion motor is activated to move the robot forward. If it needs to turn, the steering motor adjusts the robot's orientation in the desired direction.

Fails and how we fixed them

The robot used to turn way more than it should and then we found out that it was because of the failed calibration, to fix it, instead of using programed calibration, we resorted to using a manual calibration method which was to turn the motor by ourselves.
In the same topic of turning, if the ronot turned at the right angle, it would turn way to late, we figured that it was the front sensors fault so we completely scrapped the front sensor and it is now used for detecting the colored blocks.
The robot also did not drive straight, it went from side to side, to fix it, we reduced the radius of the side sensors from 45 cm to 35 cm, after that, the robot drived straight instead of wobbling from side to side.
