8.4 String slices

A segment of a string is called a slice. Selecting a slice is similar to selecting a character: >>> s = >>> print s[0:5] Monty >>> print s[6:12] Python The operator [n:m] returns the part of the string from the “n-eth” character to the “m-eth” character, including the ﬁrst but excluding the last. This behavior is counterintuitive, but it might help to imagine the indices pointing between the characters, as in Figure 8.1.

’

’

Monty Python

If you omit the ﬁrst index (before the colon), the slice starts at the beginning of the string. If you omit the second index, the slice goes to the end of the string: >>> fruit = >>> fruit[:3] ’

’

’

banana

’

ban

>>> fruit[3:] ’

’

ana

If the ﬁrst index is greater than or equal to the second the result is an empty string, repre- sented by two quotation marks: ’ >>> fruit = >>> fruit[3:3] ’’

’

banana

73

74

Chapter 8. Strings