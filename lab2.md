(5 points) From the xacro file, find the lengths of each link of the robot arm and include a list of these lengths in your write-up. Given the link lengths, and possibly your knowledge of the robot arm geometry from the visualizer, compute a maximum possible overall length of the robot arm. Note that units are in meters. This does not need to be the actual overall length of the arm, but rather a somewhat close upper bound:

From the desciription of the robot arm and the way the the joins are stacked on top of each other, I estimate the max length to be the upper_arm_length + fore_arm_length + elbow_offset+ write_offsett = .13m+.425m+.1197m+.039225m = 0.7069m

This seem like the current distance because the wrist overlap doesnt increase the horizontal length of the arm.

(5 points) Can you get your robot end effector to the maximum range you estimated in Q1, along any of the x/y/z axes? Why or why not?


(25 points) Write code to estimate the boundaries of the 3D volume of points that are reachable by the robot arm. You probably want to sample from points on a large sphere around the robot, and attempt to get the robot to reach those points, such that the arm is fully "stretched". Your code should return your results: at least, print out all the reachable points, but I encourage you to find more sophisticated ways to plot or summarize your data. You might fit an oblate spheroid to the data, or display the convex hull, or generate linear constraints containing the data - this part is up to you! Include your code and results in your write-up (screenshots are OK).

(65 points) Define and visualize a plane in the 3D plot with the robot arm; the plane should not intersect the robot arm when all the joints are set to zero position. Write code to determine if any part of the robot arm is intersecting the plane for an arbitrary pose of the robot arm, and include at least three test cases for your method. You may assume the robot arm links have zero width; in other words, as long as all the joints are on the same side of the plane, you can assume the robot arm is not colliding with the plane.
