>>> temp = a >>> a = b >>> b = temp

This solution is cumbersome; tuple assignment is more elegant:

>>> a, b = b, a

The left side is a tuple of variables; the right side is a tuple of expressions. Each value is assigned to its respective variable. All the expressions on the right side are evaluated before any of the assignments.

The number of variables on the left and the number of values on the right have to be the same:

>>> a, b = 1, 2, 3 ValueError: too many values to unpack

More generally, the right side can be any kind of sequence (string, list or tuple). For exam- ple, to split an email address into a user name and a domain, you could write:

’

>>> addr = >>> uname, domain = addr.split(

monty@python.org

’

’

@

’

)

The return value from split is a list with two elements; the ﬁrst element is assigned to uname, the second to domain.

>>> print uname monty >>> print domain python.org

12.3. Tuples as return values

12.3 Tuples as return values