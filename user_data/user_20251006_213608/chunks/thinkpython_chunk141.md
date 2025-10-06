’

a

if choice == draw_a()

:

’

’

elif choice ==

b

:

draw_b()

elif choice ==

’

c

’

:

draw_c()

Each condition is checked in order. If the ﬁrst is false, the next is checked, and so on. If one of them is true, the corresponding branch executes, and the statement ends. Even if more than one condition is true, only the ﬁrst true branch executes.

5.7 Nested conditionals

One conditional can also be nested within another. We could have written the trichotomy example like this:

if x == y:

print

’

x and y are equal

’

else:

if x < y:

43

44

Chapter 5. Conditionals and recursion

print

’

x is less than y

’

else:

print

’

x is greater than y

’

The outer conditional contains two branches. The ﬁrst branch contains a simple statement. The second branch contains another if statement, which has two branches of its own. Those two branches are both simple statements, although they could have been conditional statements as well.