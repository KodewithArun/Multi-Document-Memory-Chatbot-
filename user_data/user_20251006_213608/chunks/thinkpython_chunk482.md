the spelling! You can use dir to list the attributes that do exist.

If an AttributeError indicates that an object has NoneType, that means that it is None. One common cause is forgetting to return a value from a function; if you get to the end of a function without hitting a return statement, it returns None. Another com- mon cause is using the result from a list method, like sort, that returns None.

IndexError: The index you are using to access a list, string, or tuple is greater than its length minus one. Immediately before the site of the error, add a print statement to display the value of the index and the length of the array. Is the array the right size? Is the index the right value?

The Python debugger (pdb) is useful for tracking down Exceptions because it allows you to examine the state of the program immediately before the error. You can read about pdb at http://docs.python.org/2/library/pdb.html.

A.2.4

I added so many print statements I get inundated with output.