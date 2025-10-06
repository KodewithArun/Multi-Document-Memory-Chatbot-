There are several books and web pages about Tkinter. One of the best online resources is An Introduction to Tkinter by Fredrik Lundh.

I have written a module called Gui.py that comes with Swampy. It provides a simpliﬁed interface to the functions and classes in Tkinter. The examples in this chapter are based on this module.

Here is a simple example that creates and displays a Gui:

To create a GUI, you have to import Gui from Swampy:

from swampy.Gui import *

Or, depending on how you installed Swampy, like this:

from Gui import *

Then instantiate a Gui object:

g = Gui() ’ g.title( Gui g.mainloop()

’

)

When you run this code, a window should appear with an empty gray square and the title Gui. mainloop runs the event loop, which waits for the user to do something and

180

Chapter 19. Case study: Tkinter

responds accordingly. It is an inﬁnite loop; it runs until the user closes the window, or presses Control-C, or does something that causes the program to quit.