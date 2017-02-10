# vrep_car_simulation


V-Rep is a General purpose 3D robot simulator with integrated development environment developed by <a href="http://www.coppeliarobotics.com/" target="_parent">Coppelia Robotics</a>. Sensors, mechanisms, robots and whole systems can be modeled and simulated in various ways.
 
There are several ROS interfaces available for V-REP: see [here](http://www.coppeliarobotics.com/helpFiles/en/rosInterfaces.htm). You could use the [RosInterface](http://www.coppeliarobotics.com/helpFiles/en/rosInterf.htm), but in this case, you should program in LUA, to apply the command coming from ROS (you can do it directly in V-REP using the [embedded script](http://www.coppeliarobotics.com/helpFiles/en/scripts.htm) that you can associate with any object). 


In this case I used the VREP ROS Bridge, basically because the functionalities I needed in this case where already implemented (publish images from a vision sensor of ROS and setting a twist velocity to an object wrt its own frame).

In order to test the scene you will need to follow [this tutorial](https://github.com/lagadic/vrep_ros_bridge/tree/master).

After you can run V-REP and open the scene. When you play start, the plugin will publish images coming from the vision sensor.
