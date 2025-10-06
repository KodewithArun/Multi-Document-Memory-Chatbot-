Here is code that creates a color selection Menubutton (you can download it from http: //thinkpython.com/code/menubutton_demo.py):

g = Gui() g.la( , red colors = [ mb = g.mb(text=colors[0])

’

’

Select a color:

) green

’

’

’

,

’

’

blue

’

]

185

186

Chapter 19. Case study: Tkinter

mb creates the Menubutton. Initially, the text on the button is the name of the default color. The following loop creates one menu item for each color:

for color in colors:

g.mi(mb, text=color, command=Callable(set_color, color))

The ﬁrst argument of mi is the Menubutton these items are associated with.

The command option is a Callable object, which is something new. So far we have seen functions and bound methods used as callbacks, which works ﬁne if you don’t have to pass any arguments to the function. Otherwise you have to construct a Callable object that contains a function, like set_color, and its arguments, like color.