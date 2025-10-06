>>> x = 52 >>> fout.write(str(x))

An alternative is to use the format operator, %. When applied to integers, % is the modulus operator. But when the ﬁrst operand is a string, % is the format operator.

The ﬁrst operand is the format string, which contains one or more format sequences, which specify how the second operand is formatted. The result is a string.

’

For example, the format sequence ted as an integer (d stands for “decimal”):

%d

’

means that the second operand should be format-

>>> camels = 42 ’ >>> ’ 42

’

%d

% camels

’

The result is the string

’

42

’

, which is not to be confused with the integer value 42.

A format sequence can appear anywhere in the string, so you can embed a value in a sentence:

>>> camels = 42 >>> ’

’

I have spotted %d camels.

’

I have spotted 42 camels.

’

% camels