>>> word.find( 4

’

na

’

, 3)

And as a third argument the index where it should stop:

’

’

>>> name = >>> name.find( -1

bob ’

’

b

, 1, 2)

This search fails because b does not appear in the index range from 1 to 2 (not including 2). Exercise 8.7. There is a string method called count that is similar to the function in the previous exercise. Read the documentation of this method and write an invocation that counts the number of as in Exercise 8.8. Read the documentation of the string methods at http://docs.python.org/2/ library/stdtypes.html#string-methods. You might want to experiment with some of them to make sure you understand how they work. strip and replace are particularly useful.

’

’

banana

.

in The documentation uses find(sub[, start[, end]]), the brackets indicate optional arguments. So sub is required, but start is optional, and if you include start, then end is optional.

a

syntax that might

be

confusing.

For

example,

8.9 The in operator