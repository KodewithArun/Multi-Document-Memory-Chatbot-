This ﬁle is in plain text, so you can open it with a text editor, but you can also read it from Python. The built-in function open takes the name of the ﬁle as a parameter and returns a ﬁle object you can use to read the ﬁle. ’ >>> fin = open( >>> print fin , mode <open file fin is a common name for a ﬁle object used for input. Mode open for reading (as opposed to

’

)

words.txt

’

’

’

’

at 0xb7f4b380>

words.txt

r

’

’

r

indicates that this ﬁle is

’

’

w

for writing).

The ﬁle object provides several methods for reading, including readline, which reads characters from the ﬁle until it gets to a newline and returns the result as a string: >>> fin.readline() ’

’

aa\r\n The ﬁrst word in this particular list is “aa,” which is a kind of lava. The sequence \r\n represents two whitespace characters, a carriage return and a newline, that separate this word from the next.