lumpy = Lumpy() lumpy.make_reference()

’

’

hist = histogram( inverse = invert_dict(hist)

parrot

)

lumpy.object_diagram()

Figure C.4 shows the result. hist is a dictionary that maps from characters (single-letter strings) to integers; inverse maps from integers to lists of strings.

This example generates an object diagram for Point and Rectangle objects, as in Sec- tion 15.6. You can download it from http://thinkpython.com/code/lumpy_demo5.py.

import copy from swampy.Lumpy import Lumpy

C.4. Function and class objects

<module>

corner

Rectangle

width100.0

box2

box

Rectangle

corner

height200.0

height200.0

x0.0

width100.0

Point

y0.0

Figure C.5: Object diagram.

__name__'Rectangle'

Rectangle

__name__'Point'

Point

type

instantiate

__name__'instantiate'

Point

function

constructor

<module>

type

instantiate

obj

Figure C.6: Object diagram.

lumpy = Lumpy() lumpy.make_reference()