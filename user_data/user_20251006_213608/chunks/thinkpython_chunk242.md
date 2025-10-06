Sometimes you want to traverse one list while building another. For example, the following function takes a list of strings and returns a new list that contains capitalized strings:

def capitalize_all(t):

res = [] for s in t:

res.append(s.capitalize())

return res

res is initialized with an empty list; each time through the loop, we append the next ele- ment. So res is another kind of accumulator.

An operation like capitalize_all is sometimes called a map because it “maps” a function (in this case the method capitalize) onto each of the elements in a sequence. Exercise 10.2. Use capitalize_all to write a function named capitalize_nested that takes a nested list of strings and returns a new nested list with all strings capitalized.

Another common operation is to select some of the elements from a list and return a sublist. For example, the following function takes a list of strings and returns a list that contains only the uppercase strings:

def only_upper(t):