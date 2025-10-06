from TurtleWorld import *

The details of the installation process and setting Python’s search path depend on your system, so rather than include those details here, I will try to maintain current information for several systems at http://thinkpython.com/swampy

Create a ﬁle named mypolygon.py and type in the following code:

from swampy.TurtleWorld import *

world = TurtleWorld() bob = Turtle() print bob

wait_for_user()

32

Chapter 4. Case study: interface design

The ﬁrst line imports everything from the TurtleWorld module in the swampy package.

The next lines create a TurtleWorld assigned to world and a Turtle assigned to bob. Printing bob yields something like:

<TurtleWorld.Turtle instance at 0xb7bfbf4c>

This means that bob refers to an instance of a Turtle as deﬁned in module TurtleWorld. In this context, “instance” means a member of a set; this Turtle is one of the set of possible Turtles.