>>> camels = 42 >>> ’

’

I have spotted %d camels.

’

I have spotted 42 camels.

’

% camels

If there is more than one format sequence in the string, the second argument has to be a tuple. Each format sequence is matched with an element of the tuple, in order.

The following example uses %s ber (don’t ask why), and

’

’ %d ’ to format a string:

’

to format an integer,

’

%g

’

to format a ﬂoating-point num-

’

>>> ’

In %d years I have spotted %g %s. In 3 years I have spotted 0.1 camels.

’ ’

% (3, 0.1,

’

camels

’

)

The number of elements in the tuple has to match the number of format sequences in the string. Also, the types of the elements have to match the format sequences:

’

’

%d %d %d

>>> TypeError: not enough arguments for format string >>> TypeError: illegal argument type for built-in operation

% (1, 2)

’

’

’

’

%d

%

dollars

14.4. Filenames and paths

In the ﬁrst example, there aren’t enough elements; in the second, the element is the wrong type.