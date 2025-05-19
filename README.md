# Autonomous-maze-solving-for-micromouse
Right-Hand Rule and Left-Hand Rule: The code starts by using the right-hand rule, which means that the robot follows the right wall of the maze. If the robot encounters a situation where the right-hand rule cannot be applied, it switches to the left-hand rule, which means following the left wall.

Stacks: The code uses two stacks (righthandstack and lefthandstack) to keep track of the movements made while following the right-hand rule and the left-hand rule, respectively. The movements are encoded as integers (e.g., 4 for a right turn, 5 for a left turn, 1 for moving forward).

Backtracking: If the robot reaches a point where both the right-hand rule and the left-hand rule fail to find a path, it enters the deneme state. In this state, the robot compares the lengths of the righthandstack and lefthandstack to determine which stack has the shorter path. The robot then follows the shorter path, backtracking to a point where it can try a different direction.

Final Path: After the backtracking process, the robot enters the son state, where it follows the optimal path stored in the BABANSTACK. The robot pops movements from this stack and executes them until it reaches the center of the maze.

The code uses ultrasonic sensors (trigPin and echoPin) to detect walls and obstacles in the maze. Based on the sensor readings, the robot decides whether to move forward, turn right, or turn left, following the right-hand rule or the left-hand rule.

The algorithm is implemented using several boolean flags (sagadonus, soladonus, righthandrule, lefthandrule, deneme, son, turnbacktime) and conditional statements to handle various maze situations.

Materials Required:
1. Arduino Uno
2. ArduMoto
3. Ultrasonic Sensors
4. Lithium battery
5. Stepper Motor

