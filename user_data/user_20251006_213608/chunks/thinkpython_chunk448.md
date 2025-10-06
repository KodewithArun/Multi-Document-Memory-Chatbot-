en creates a new Entry: ’

entry = g.en(text=

Default text.

’

)

The text option allows you to put text into the entry when it is created. The get method returns the contents of the Entry (which may have been changed by the user):

>>> entry.get() ’ ’ Default text.

te creates a Text widget:

text = g.te(width=100, height=5)

width and height are the dimensions of the widget in characters and lines.

insert puts text into the Text widget:

text.insert(END,

’

A line of text.

’

)

19.6. Packing widgets

END is a special index that indicates the last character in the Text widget.

You can also specify a character using a dotted index, like 1.1, which has the line num- ber before the dot and the column number after. The following example adds the letters ’

’

after the ﬁrst character of the ﬁrst line. nother

nother

’

’