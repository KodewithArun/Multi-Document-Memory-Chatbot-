Figure C.1 shows the result. The graphical style is different from what I showed earlier; for example, each reference is represented by a circle next to the variable name and a line to the value. And long strings are truncated. But the information conveyed by the diagram is the same.

The variable names are in a frame labeled <module>, which indicates that these are module- level variables, also known as global.

You can download this example from http://thinkpython.com/code/lumpy_demo1.py. Try adding some additional assignments and see what the diagram looks like.

C.2 Stack diagram

Here’s an example that uses Lumpy to generate a stack diagram. You can download it from http://thinkpython.com/code/lumpy_demo2.py.

C.3. Object diagrams

0'Cheddar'

2'Gouda'

list

1123

list

list

<module>

cheeses

1'Edam'

empty

017

numbers

Figure C.3: Object diagram.

from swampy.Lumpy import Lumpy

def countdown(n): if n <= 0:

’

’

print Blastoff! lumpy.object_diagram()

else: