row creates a row Frame and makes it the “current Frame.” Until this Frame is closed or another Frame is created, all subsequent widgets are packed in a row.

Here is the code that creates the Canvas and the column Frame that hold the other widgets:

183

184

Chapter 19. Case study: Tkinter

Figure 19.1: TurtleWorld after running the snowﬂake code.

self.canvas = self.ca(width=400, height=400, bg= self.col()

’

white

’

)

The ﬁrst widget in the column is a grid Frame, which contains four buttons arranged two- by-two:

self.gr(cols=2) self.bu(text= self.bu(text= self.bu(text= self.bu(text= self.endgr()

’ ’ ’ ’

’

Print canvas Quit Make Turtle ’ Clear

, command=self.canvas.dump)

’

, command=self.quit)

’

, command=self.make_turtle)

, command=self.clear)

gr creates the grid; the argument is the number of columns. Widgets in the grid are laid out left-to-right, top-to-bottom.