Code examples from this chapter are available from http://thinkpython.com/code/ polygon.py.

4.1 TurtleWorld

To accompany this book, I have written a package called Swampy. You can download Swampy from http://thinkpython.com/swampy; follow the instructions there to install Swampy on your system.

A package is a collection of modules; one of the modules in Swampy is TurtleWorld, which provides a set of functions for drawing lines by steering turtles around the screen.

If Swampy is installed as a package on your system, you can import TurtleWorld like this:

from swampy.TurtleWorld import *

If you downloaded the Swampy modules but did not install them as a package, you can ei- ther work in the directory that contains the Swampy ﬁles, or add that directory to Python’s search path. Then you can import TurtleWorld like this:

from TurtleWorld import *