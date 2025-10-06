’

’

m a lumberjack, and I

m okay."

To end the function, you have to enter an empty line (this is not necessary in a script).

Deﬁning a function creates a variable with the same name. >>> print print_lyrics <function print_lyrics at 0xb7e99e9c> >>> type(print_lyrics) function <type

’

’

>

The value of print_lyrics is a function object, which has type

’

function

’

.

The syntax for calling the new function is the same as for built-in functions: >>> print_lyrics() I I sleep all night and I work all day.

’

’

m a lumberjack, and I

m okay.

Once you have deﬁned a function, you can use it inside another function. For example, to repeat the previous refrain, we could write a function called repeat_lyrics: def repeat_lyrics():

print_lyrics() print_lyrics()

And then call repeat_lyrics: >>> repeat_lyrics() I I sleep all night and I work all day. I I sleep all night and I work all day.

’

’

m a lumberjack, and I

m okay.

’

’

m a lumberjack, and I

m okay.