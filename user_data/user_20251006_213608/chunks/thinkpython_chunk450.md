You can see my solution at http://thinkpython.com/code/circle_demo.py.

19.6 Packing widgets

So far we have been stacking widgets in a single column, but in most GUIs the layout is more complicated. For example, Figure 19.1 shows a simpliﬁed version of TurtleWorld (see Chapter 4).

This section presents the code that creates this GUI, broken into a series of steps. You can download the complete example from http://thinkpython.com/code/ SimpleTurtleWorld.py.

At the top level, this GUI contains two widgets—a Canvas and a Frame—arranged in a row. So the ﬁrst step is to create the row. class SimpleTurtleWorld(TurtleWorld):

"""This class is identical to TurtleWorld, but the code that lays out the GUI is simplified for explanatory purposes."""

def setup(self):

self.row() ...

setup is the function that creates and arranges the widgets. Arranging widgets in a GUI is called packing.