7. Modify steer so the Turtles play tag. You can add methods to Tagger and you can override steer and __init__, but you may not modify or override step, wobble or move. Also, steer is allowed to change the heading of the Turtle but not the position. Adjust the rules and your steer method for good quality play; for example, it should be possible for the slow Turtle to tag the faster Turtles eventually.

Solution: http://thinkpython.com/code/Tagger.py.

Chapter 19

Case study: Tkinter

19.1 GUI

Most of the programs we have seen so far are text-based, but many programs use graphical user interfaces, also known as GUIs.

Python provides several choices for writing GUI-based programs, including wxPython, Tkinter, and Qt. Each has pros and cons, which is why Python has not converged on a standard.

The one I will present in this chapter is Tkinter because I think it is the easiest to get started with. Most of the concepts in this chapter apply to the other GUI modules, too.