19.7. Menus and Callables

endrow ends this row of widgets, so subsequent widgets are packed in the column Frame. Gui.py keeps a stack of Frames:

When you use row, col or gr to create a Frame, it goes on top of the stack and becomes the current Frame.

When you use endrow, endcol or endgr to close a Frame, it gets popped off the stack and the previous Frame on the stack becomes the current Frame.

The method run_file reads the contents of the Entry, uses it as a ﬁlename, reads the con- tents and passes it to run_code. self.inter is an Interpreter object that knows how to take a string and execute it as Python code.

def run_file(self):

filename = self.en_file.get() fp = open(filename) source = fp.read() self.inter.run_code(source, filename)

The last two widgets are a Text widget and a Button:

self.te_code = self.te(width=25, height=10) ) self.te_code.insert(END, self.te_code.insert(END,

’ ’

’

world.clear()\n bob = Turtle(world)\n

’

)

self.bu(text=

’

Run code

’