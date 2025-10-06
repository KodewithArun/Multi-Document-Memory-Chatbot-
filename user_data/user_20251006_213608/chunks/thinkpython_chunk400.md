If the second operand is a Point, the method should return a new Point whose x coordinate is the sum of the x coordinates of the operands, and likewise for the y coordinates.

If the second operand is a tuple, the method should add the ﬁrst element of the tuple to the x coordinate and the second element to the y coordinate, and return a new Point with the result.

17.9 Polymorphism

Type-based dispatch is useful when it is necessary, but (fortunately) it is not always neces- sary. Often you can avoid it by writing functions that work correctly for arguments with different types.

Many of the functions we wrote for strings will actually work for any kind of sequence. For example, in Section 11.1 we used histogram to count the number of times each letter appears in a word.

def histogram(s): d = dict() for c in s:

if c not in d:

d[c] = 1

else:

d[c] = d[c]+1

return d