If you get stuck, you can download http://thinkpython.com/code/GoodKangaroo.py, which explains the problem and demonstrates a solution. Exercise 17.8. Visual is a Python module that provides 3-D graphics. It is not always included in a Python installation, so you might have to install it from your software repository or, if it’s not there, from http://vpython.org.

The following example creates a 3-D space that is 256 units wide, long and high, and sets the “center” to be the point (128,128,128). Then it draws a blue sphere.

from visual import *

scene.range = (256, 256, 256) scene.center = (128, 128, 128)

color = (0.1, 0.1, 0.9) sphere(pos=scene.center, radius=128, color=color)

# mostly blue

color is an RGB tuple; that is, the elements are Red-Green-Blue levels between 0.0 and 1.0 (see http://en.wikipedia.org/wiki/RGB_color_model).