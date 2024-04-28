### topics_quiz

#### TODO
1. [`avoid_wall.cpp`](avoidwall.cpp). Specs:
   > ROS node:
   > 1. Create a Publisher that writes into the /cmd_vel topic in order to move the robot.
   > 2. Create a Subscriber that reads from the /kobuki/laser/scan topic. This is the topic where the laser publishes its data.
   > 3. Depending on the readings you receive from the laser's topic, you'll have to change the data you're sending to the /cmd_vel topic in order to avoid the wall. This means, use the values of the laser to decide.
   > 
   > Program logic:
   >
   > 1. If the laser reading in front of the robot is higher than 1 meter (there is no obstacle closer than 1 meter in front of the robot), the robot will move forward.
   > 2. If the laser reading in front of the robot is lower than 1 meter (there is an obstacle closer than 1 meter in front of the robot), the robot will turn left.
   > 3. If the laser reading at the right side of the robot is lower than 1 meter (there is an obstacle closer than 1 meter at the right side of the robot), the robot will turn left.
   > 4. If the laser reading at the left side of the robot is lower than 1 meter (there is an obstacle closer than 1 meter at the left side of the robot), the robot will turn right.
2. [`CMakeLists.txt`](CMakeLists.txt). To do:
   1. `add_executable`.
   2. `add_dependencies`.
   3. `target_link_libraries`.
   4. Anything specific for messages?
3. [`package.xml`](package.xml). To do:
   1. `<build_depend>`.
   2. `<build_export_depend>`.
   3. `<exec_depend>`.
   4. Anything else?
