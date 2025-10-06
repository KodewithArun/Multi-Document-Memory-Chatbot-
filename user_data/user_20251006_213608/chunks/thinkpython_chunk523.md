C.3 Object diagrams

This example generates an object diagram showing the lists from Section 10.1. You can download it from http://thinkpython.com/code/lumpy_demo3.py. from swampy.Lumpy import Lumpy

lumpy = Lumpy() lumpy.make_reference()

cheeses = [

’

Cheddar

’

,

’

Edam

’

,

’

Gouda

’

]

213

214

Appendix C. Lumpy

1'p'

inverse

2't'

<module>

3'o'

1

dict

2

0'r'

list

'a'1

hist

'p'1

't'1

0'a'

dict

'r'2

list

'o'1

Figure C.4: Object diagram.

numbers = [17, 123] empty = []

lumpy.object_diagram()

Figure C.3 shows the result. Lists are represented by a box that shows the indices mapping to the elements. This representation is slightly misleading, since indices are not actually part of the list, but I think they make the diagram easier to read. The empty list is repre- sented by an empty box.

And here’s an example showing the dictionaries from Section 11.4. You can download it from http://thinkpython.com/code/lumpy_demo4.py. from swampy.Lumpy import Lumpy