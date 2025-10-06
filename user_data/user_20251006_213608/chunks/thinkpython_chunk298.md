117

118

Chapter 12. Tuples

01’Cleese’’John’tuple

Figure 12.1: State diagram.

(’Cleese’, ’John’)’08700 100 222’’08700 100 222’’08700 100 222’’08700 100 222’’08700 100 222’(’Chapman’, ’Graham’)(’Idle’, ’Eric’)(’Jones’, ’Terry’)(’Gilliam’, ’Terry’)(’Palin’, ’Michael’)’08700 100 222’dict

Figure 12.2: State diagram.

for last, first in directory:

print first, last, directory[last,first]

This loop traverses the keys in directory, which are tuples. It assigns the elements of each tuple to last and first, then prints the name and corresponding telephone number.

There are two ways to represent tuples in a state diagram. The more detailed version shows the indices and elements just as they appear in a list. For example, the tuple (

’

’

’

’

Cleese

,

John

) would appear as in Figure 12.1.

But in a larger diagram you might want to leave out the details. For example, a diagram of the telephone directory might appear as in Figure 12.2.