’ ’

’

world.clear()\n bob = Turtle(world)\n

’

)

self.bu(text=

’

Run code

’

, command=self.run_text)

run_text is similar to run_file except that it takes the code from the Text widget instead of from a ﬁle:

def run_text(self):

source = self.te_code.get(1.0, END) self.inter.run_code(source,

’

<user-provided code>

’

)

Unfortunately, the details of widget layout are different in other languages, and in different Python modules. Tkinter alone provides three different mechanisms for arranging widgets. These mechanisms are called geometry managers. The one I demonstrated in this section is the “grid” geometry manager; the others are called “pack” and “place”.

Fortunately, most of the concepts in this section apply to other GUI modules and other languages.

19.7 Menus and Callables

A Menubutton is a widget that looks like a button, but when pressed it pops up a menu. After the user selects an item, the menu disappears.