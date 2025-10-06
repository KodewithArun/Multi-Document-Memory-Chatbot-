The one-eth element of numbers, which used to be 123, is now 5.

You can think of a list as a relationship between indices and elements. This relationship is called a mapping; each index “maps to” one of the elements. Figure 10.1 shows the state diagram for cheeses, numbers and empty:

Lists are represented by boxes with the word “list” outside and the elements of the list inside. cheeses refers to a list with three elements indexed 0, 1 and 2. numbers contains two elements; the diagram shows that the value of the second element has been reassigned from 123 to 5. empty refers to a list with no elements.

List indices work the same way as string indices:

Any integer expression can be used as an index.

If you try to read or write an element that does not exist, you get an IndexError.

If an index has a negative value, it counts backward from the end of the list.

The in operator also works on lists. ’

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