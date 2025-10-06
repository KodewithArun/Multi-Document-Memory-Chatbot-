’

’

Hello, World!

.

’

’

These values belong to different types: 2 is an integer, and is a string, so-called because it contains a “string” of letters. You (and the interpreter) can identify strings because they are enclosed in quotation marks.

Hello, World!

If you are not sure what type a value has, the interpreter can tell you.

’

>>> type( <type > >>> type(17) ’ > <type

Hello, World! ’

’

str

’

int

’

)

Not surprisingly, strings belong to the type str and integers belong to the type int. Less obviously, numbers with a decimal point belong to a type called float, because these num- bers are represented in a format called ﬂoating-point.

>>> type(3.2) ’ ’ <type

float

>

What about values like marks like strings.

’

17

’

and

’

3.2

’

? They look like numbers, but they are in quotation

’

>>> type( <type >>> type( <type

’

str ’

’

str

’

17 ’ > 3.2 ’ >

)

’

)

They’re strings.