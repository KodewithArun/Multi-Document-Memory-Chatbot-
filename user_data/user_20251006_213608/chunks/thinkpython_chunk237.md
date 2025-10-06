’

’

>>> cheeses = [ >>> Edam True >>> False

Cheddar

,

’

’

in cheeses

’

’

Brie

in cheeses

Edam

’

,

’

Gouda

’

]

10.3. Traversing a list

10.3 Traversing a list

The most common way to traverse the elements of a list is with a for loop. The syntax is the same as for strings:

for cheese in cheeses:

print cheese

This works well if you only need to read the elements of the list. But if you want to write or update the elements, you need the indices. A common way to do that is to combine the functions range and len:

for i in range(len(numbers)):

numbers[i] = numbers[i] * 2

This loop traverses the list and updates each element. len returns the number of elements in the list. range returns a list of indices from 0 to n − 1, where n is the length of the list. Each time through the loop i gets the index of the next element. The assignment statement in the body uses i to read the old value of the element and to assign the new value.