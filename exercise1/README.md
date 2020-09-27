# Monday 28/09 Exercise

Please follow these steps:

1. Create a package, with dependencies: *geometry_msgs*, *nav_msgs*, *roscpp*.
2. Put the source code **exercise.cpp** in the src directory of the new package.
3. Create another package, with dependencies: *roscpp*, *std_msgs*, *message_generation*.
4. Put the source code **PositionServer.cpp** in the src directory of the new package.
5. Now, create a service message (using this second package) with an empty request, and two floats (x and y) as response.
6. Modify **PositionServer.cpp** so as to implement a Ros service which use the service message that you have defined to return two random floats, x and y, respectively between *x_min* and *x_max* and *y_min* and *y_max* (the function **RandomFloat** is already defined). Some code should be added when you see comments in the form:
```
/* Bla bla bla

*/
```
7. Now modify **exercise1.cpp** so as to reach the target with the robot. When the target is reached, the node should require the service to send a new target position.
8. If needed, modify the **CMakeLists.txt** and **package.xml** of the two packages.

Run and have fun!
