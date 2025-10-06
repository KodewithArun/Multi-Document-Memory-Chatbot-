The ﬁrst button uses self.canvas.dump as a callback; the second uses self.quit. These are bound methods, which means they are associated with a particular object. When they are invoked, they are invoked on the object.

The next widget in the column is a row Frame that contains a Button and an Entry:

self.row([0,1], pady=30) self.bu(text= self.en_file = self.en(text= self.endrow()

’

’

Run file

, command=self.run_file) snowflake.py

’

’

, width=5)

The ﬁrst argument to row is a list of weights that determines how extra space is allocated between widgets. The list [0,1] means that all extra space is allocated to the second wid- get, which is the Entry. If you run this code and resize the window, you will see that the Entry grows and the Button doesn’t.

The option pady “pads” this row in the y direction, adding 30 pixels of space above and below.

19.7. Menus and Callables