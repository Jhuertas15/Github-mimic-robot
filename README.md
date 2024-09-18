Our robot is based on several real-life and fictional car models, and the model that you can see in the second version of the v-photos folder was decided from them. The mechanism is inspired by electric cars like the Tesla, which utilize electric motors for instant acceleration. These vehicles operate without traditional gears, providing a unique torque profile; however, the speed of the robot is specifically designed to be fast while maintaining precision. Initially, we attempted to base our robot on the Octane from the popular game Rocket League, but during the building process, the size of the car was too large for our format, leading us to scrap that design. The current design is not based on anything specific but is engineered to be functional for the competition.

 Now we are going to talk about our robot.

 Robot Components

Brain  
The brain of the robot is the central processing unit (CPU), which acts as the main controller. In the LEGO Spike Prime system, this brain is known as the Hub. The Hub features an integrated screen to display information and feedback, multiple input/output ports to connect sensors and motors, and Bluetooth and USB connectivity for program loading and communication with other devices. It is also equipped with a gyroscope to ensure the robot remains calibrated at all times, which is crucial for maintaining accurate movement and positioning.

Distance Sensors  
This robot is equipped with three distance sensors that utilize ultrasonic technology to measure the distance between the robot and objects on the track. Distance sensors are critical for autonomous navigation, allowing the robot to detect obstacles and calculate distances to avoid collisions.
- Front Distance Sensor: Mounted on the front, this sensor primarily detects obstacles directly in the robot's path, providing crucial data for forward navigation.
- Side Distance Sensors: Installed on both sides of the robot, these sensors help detect lateral obstacles and maintain alignment on the track. They are vital for making decisions regarding lateral movements or turns, ensuring the robot can navigate tight spaces effectively.

Color Sensor  
The robot's color sensor is a versatile tool capable of detecting various colors. Positioned on the front of the robot, it identifies the colors of different obstacles on the track. This sensor can discern multiple colors and measure the intensity of reflected light, enabling the robot to interpret color signals as action commands essential for navigation and decision-making.

Motors  
The robot utilizes two motors for movement—one dedicated to propulsion and another for steering.
- Propulsion Motor: Responsible for moving the robot forward and backward, this motor's speed and power can be controlled, allowing for adjustments in travel speed as needed. The propulsion system is designed for rapid acceleration, mimicking the performance characteristics of electric vehicles.
- Steering Motor: This motor controls the robot's turning capabilities. By adjusting its position, the robot can change direction, allowing it to move left or right. The combination of propulsion and steering motors provides the robot with the ability to perform complex and precise maneuvers, crucial for navigating obstacles effectively.

 Energy Management

Energy management is a fundamental aspect of the robot's design. The robot is powered by a rechargeable battery, which supplies energy to the Hub and the motors. This choice allows for efficient operation and portability, essential for competition settings. 

- Battery Life Monitoring: The Hub is programmed to monitor battery levels continuously. If the energy level drops below a certain threshold, the robot can execute a predefined action, such as returning to a designated charging station or pausing its operations to conserve energy.
- Energy Efficiency: The programming includes energy-efficient algorithms that optimize motor usage. For example, the robot reduces motor power during idle periods and employs regenerative braking techniques when slowing down, which helps extend battery life.

 Programming and Functionality

The LEGO Spike Prime robot's programming is designed to integrate readings from the distance and color sensors, enabling it to make autonomous decisions about its movement. Here is how a program for this robot is structured.

Initialization  
At the start of the program, the robot performs an initial calibration of its sensors to ensure accurate readings. This includes setting the initial position of the motors and configuring the parameters of the distance and color sensors.

Sensor Reading  
The robot enters a continuous loop where it reads the values from the three distance sensors and the color sensor. These values are stored in variables that are updated in each iteration of the loop, allowing for real-time decision-making.

Obstacle Detection  
Using the values from the distance sensors, the robot determines if there are any nearby obstacles in its path or on its sides. For example:
- The side distance sensors are used to detect if the spaces to the sides are clear for a safe turn.
- The front sensor measures the distance to the nearest wall or obstacle, providing critical data for timing the robot's turns.

Color Interpretation  
The color sensor allows the robot to interpret signals in its environment. For instance, if the robot detects a red or green object in front, it might interpret this as a signal to turn right or left, respectively. The robot can also be programmed to respond to specific color patterns, enhancing its ability to navigate complex environments.

Decision Making  
Based on the readings from the distance and color sensors, the robot decides on the action to take. A simple algorithm might be:
- If the front distance sensor detects a nearby obstacle, check the side sensors.
- If the right side is clear, turn right; if the left side is clear, turn left.
- If a specific color is detected in the front, execute the associated action (e.g., turn or stop).

Movement  
The decisions made are translated into commands for the motors. If the robot decides to move forward, the propulsion motor is activated to move the robot forward. If it needs to turn, the steering motor adjusts the robot's orientation in the desired direction. The robot can also execute complex movements, such as sharp turns or gradual curves, depending on the situation.

 Strategy for Overcoming Obstacles

The strategy of the robot for overcoming obstacles is based on a combination of sensors, programming logic, and motor control. Here are the key steps in this strategy:

1. Obstacle Detection: The three distance sensors (front and sides) are essential for detecting obstacles in the path. The front sensor measures the distance to the nearest object, while the side sensors help evaluate available space for lateral movement.

2. Data Analysis: The data collected by the sensors is processed in real-time. If the front sensor detects an obstacle at a critical distance, the robot initiates its evasion protocol.

3. Decision Making: Using a simple algorithm, the robot evaluates the situation:
   - If the front sensor detects an obstacle, it checks the side sensors.
   - If the right side is clear, the robot turns right; if the left side is clear, it turns left.
   - If both sides are blocked, the robot may opt to back up or stop.

4. Movement Execution: Once a decision is made, the robot sends commands to the motors:
   - The propulsion motor is activated to move the robot backward or forward.
   - The steering motor is adjusted to change the robot's orientation based on the decision.

5. Continuous Adaptation: The robot enters a continuous cycle of sensor reading and decision-making, allowing it to adapt to changes in the environment in real-time. This is crucial for effective navigation in a dynamic and obstacle-filled environment.

6. Use of the Color Sensor: In addition to distance sensors, the robot uses the color sensor to interpret signals in the environment. For example, if it detects a specific color block, it can execute a programmed action, such as stopping or changing direction.

 Failures and Solutions

The robot initially had issues with turning more than it should, which was traced back to failed calibration. To fix this, we switched from programmed calibration to a manual method, where we turned the motor ourselves. Another issue was that if the robot turned at the correct angle, it would do so too late; we identified this as a fault with the front sensor, which we subsequently replaced with a sensor dedicated to detecting colored blocks. Additionally, the robot did not drive straight and wobbled from side to side. We resolved this by reducing the radius of the side sensors from 45 cm to 35 cm, after which the robot drove straight instead of swaying.

 Conclusion

In summary, our robot integrates advanced sensor technology, efficient energy management, and intelligent programming to navigate its environment and overcome obstacles effectively. The combination of propulsion and steering motors allows for precise movement, while real-time data analysis ensures adaptive responses to dynamic challenges. This comprehensive design not only enhances the robot's performance in competitions but also provides a robust platform for further development and improvements.
