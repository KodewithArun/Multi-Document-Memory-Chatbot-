canvas.rectangle([[0, 0], [200, 100]], , outline= fill=

’

’

blue

’

orange

’

, width=10)

This way of specifying corners is called a bounding box because the two points bound the rectangle.

oval takes a bounding box and draws an oval within the speciﬁed rectangle:

canvas.oval([[0, 0], [200, 100]], outline=

’

orange

’

, width=10)

line takes a sequence of coordinates and draws a line that connects the points. This exam- ple draws two legs of a triangle:

canvas.line([[0, 100], [100, 200], [200, 100]], width=10)

polygon takes the same arguments, but it draws the last leg of the polygon (if necessary) and ﬁlls it in:

canvas.polygon([[0, 100], [100, 200], [200, 100]], ’

’

’

’

red

fill=

, outline=

orange

, width=10)

19.5 More widgets

Tkinter provides two widgets that let users type text: an Entry, which is a single line, and a Text widget, which has multiple lines.

en creates a new Entry: ’

entry = g.en(text=

Default text.

’

)