 projectile-simulation
 
 ----main.py-----
This script is a Pygame program that simulates projectile motion. It uses trigonometric functions to calculate the position, range, and time of flight of a projectile. The program also allows the user to interact with the simulation by adjusting the launch angle of the projectile using the mouse. 
The program uses several Pygame features such as the display, event, and font modules, as well as game loop structures to update and render the simulation on the screen.

------functions.py----
In this it takes in two points (p1, p2) and calculates the slope (gradient) of the line that connects them. 
If the x-coordinate of the two points are the same, the slope is set to 90 degrees (in radians).

The getAngleFromGradient() function takes in the gradient of a line and returns the angle (in radians) that the line makes with the x-axis.

The getAngle() function takes in a point (pos) and an origin point, and calculates the angle (in degrees) that the line from the origin to the point makes with the positive x-axis.

The getPosOnCircumeference() function takes in an angle (in degrees) and an origin point, and returns the coordinates of a point on the circle's circumference that is at the given angle from the origin. This is done by converting the angle to radians, and then using the sine and cosine functions to calculate the x and y coordinates of the point.
