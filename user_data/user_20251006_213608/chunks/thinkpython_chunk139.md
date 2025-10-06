There is no limit on the number of statements that can appear in the body, but there has to be at least one. Occasionally, it is useful to have a body with no statements (usually as a place keeper for code you haven’t written yet). In that case, you can use the pass statement, which does nothing. if x < 0:

pass

# need to handle negative values!

5.5. Alternative execution

5.5 Alternative execution

A second form of the if statement is alternative execution, in which there are two possi- bilities and the condition determines which one gets executed. The syntax looks like this:

if x%2 == 0: print

’

x is even

’

else:

print

’

x is odd

’