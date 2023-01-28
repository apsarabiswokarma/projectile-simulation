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

```python

BLACK = (18, 18, 18)
WHITE = (217, 217, 217)
RED = (252, 91, 122)
GREEN = (29, 161, 16)
BLUE = (78, 193, 246)
ORANGE = (252, 76, 2)
YELLOW = (254, 221, 0)
PURPLE = (155, 38, 182)
AQUA = (0, 249, 182)

COLORS = [RED, GREEN, BLUE, ORANGE, YELLOW, PURPLE]
```
This code defines several variables that hold RGB color values. These values are used to create different colors in an image or display.

BLACK, WHITE, RED, GREEN, BLUE, ORANGE, YELLOW, PURPLE, and AQUA are all variables that hold a tuple of 3 integers. 
These integers represent the red, green, and blue components of the color respectively, and range from 0-255.
For example, the value of the variable RED is (252, 91, 122) which represents a reddish color.

The variable COLORS is also a list, but it contains the variables RED, GREEN, BLUE, ORANGE, YELLOW, and PURPLE. 
These are the color constants that are being used in the code

```python
pygame.init()
SCREEN = WIDTH, HEIGHT = 288, 512

info = pygame.display.Info()
width = info.current_w
height = info.current_h

if width >= height:
    win = pygame.display.set_mode(SCREEN, pygame.NOFRAME)
else:
    win = pygame.display.set_mode(
        SCREEN, pygame.NOFRAME | pygame.SCALED | pygame.FULLSCREEN)

clock = pygame.time.Clock()
FPS = 60
```
This code initializes the Pygame library and creates a window with the dimensions 288x512.
It then uses the pygame.display.Info() function to get the current width and height of the screen. 
If the width is greater than or equal to the height, the window is created without a frame using the pygame.NOFRAME flag.
Otherwise, the window is created with the pygame.NOFRAME, pygame.SCALED, and pygame.
FULLSCREEN flags, which removes the frame, scales the window to fit the screen, and sets the window to fullscreen mode.
The code also creates a clock object with a target framerate of 60 FPS.


