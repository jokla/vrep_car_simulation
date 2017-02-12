# vrep_car_simulation

The aim of this project is to simulate and control one ore more car in V-REP using ROS. 

The Open Source Self Driving Car (OSSDC) Initiative is fully organized and managed on GitHub at:
(https://github.com/OSSDC/)[https://github.com/OSSDC/]

I invite everyone to join the discussion and contribute, follow the instructions here:
http://ossdc.org/join

The mission of this initiative and open organization is to bring the best research in self driving car space and create a full stack of open source software and hardware components to allow anyone to build and test from toy to full size self driving cars.



V-Rep is a General purpose 3D robot simulator with integrated development environment developed by <a href="http://www.coppeliarobotics.com/" target="_parent">Coppelia Robotics</a>. Sensors, mechanisms, robots and whole systems can be modeled and simulated in various ways.
 
There are several ROS interfaces available for V-REP: see [here](http://www.coppeliarobotics.com/helpFiles/en/rosInterfaces.htm). You could use the [RosInterface](http://www.coppeliarobotics.com/helpFiles/en/rosInterf.htm), but in this case, you should program in LUA to apply the command coming from ROS (you can do it directly in V-REP using the [embedded script](http://www.coppeliarobotics.com/helpFiles/en/scripts.htm) that you can associate with any object in the scene). 


In this case I used the [VREP ROS Bridge](https://github.com/lagadic/vrep_ros_bridge/tree/master), basically because the functionalities I needed where already implemented (we need to publish images coming from a vision sensor and apply a twist velocity to an object with respect to its own frame).

In order to test the scene you will need to follow [this tutorial](https://github.com/lagadic/vrep_ros_bridge/tree/master).

After you can run V-REP and open the scene. When you play start, the plugin will publish images coming from the vision sensor.
