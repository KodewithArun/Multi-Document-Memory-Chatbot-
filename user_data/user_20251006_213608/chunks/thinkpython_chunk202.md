The following example shows how to use concatenation (string addition) and a for loop to generate an abecedarian series (that is, in alphabetical order). In Robert McCloskey’s book Make Way for Ducklings, the names of the ducklings are Jack, Kack, Lack, Mack, Nack, Ouack, Pack, and Quack. This loop outputs these names in order:

8.4. String slices

fruitbannaa’0123456index’

Figure 8.1: Slice indices.

prefixes = ’ suffix =

’

JKLMNOPQ

’

ack

’

for letter in prefixes:

print letter + suffix

The output is: Jack Kack Lack Mack Nack Oack Pack Qack

Of course, that’s not quite right because “Ouack” and “Quack” are misspelled. Exercise 8.2. Modify the program to ﬁx this error.

8.4 String slices