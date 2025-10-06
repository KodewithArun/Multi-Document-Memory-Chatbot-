’

,

’

E

’

Anne ’

), (

, ’

n

’ ’

Elk ’ ,

’

l

) ’

), (

’

n

’

,

’

k

’

)]

You can use tuple assignment in a for loop to traverse a list of tuples: ’

’

’

’

’

’

a

t = [( , 0), ( for letter, number in t: print number, letter

b

, 1), (

c

, 2)]

Each time through the loop, Python selects the next tuple in the list and assigns the ele- ments to letter and number. The output of this loop is:

0 a 1 b 2 c

If you combine zip, for and tuple assignment, you get a useful idiom for traversing two (or more) sequences at the same time. For example, has_match takes two sequences, t1 and t2, and returns True if there is an index i such that t1[i] == t2[i]:

def has_match(t1, t2):

for x, y in zip(t1, t2):

if x == y:

return True

return False

If you need to traverse the elements of a sequence and their indices, you can use the built-in function enumerate:

for index, element in enumerate(

’

abc

’

):

print index, element

12.6. Dictionaries and tuples