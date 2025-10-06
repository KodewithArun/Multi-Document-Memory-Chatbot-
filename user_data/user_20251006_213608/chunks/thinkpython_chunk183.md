Figure 7.1 shows what multiple assignment looks like in a state diagram.

With multiple assignment it is especially important to distinguish between an assignment operation and a statement of equality. Because Python uses the equal sign (=) for assign- ment, it is tempting to interpret a statement like a = b as a statement of equality. It is not!

First, equality is a symmetric relation and assignment is not. For example, in mathematics, if a = 7 then 7 = a. But in Python, the statement a = 7 is legal and 7 = a is not.

Furthermore, in mathematics, a statement of equality is either true or false, for all time. If a = b now, then a will always equal b. In Python, an assignment statement can make two variables equal, but they don’t have to stay that way:

a = 5 b = a a = 3

# a and b are now equal # a and b are no longer equal

The third line changes the value of a but does not change the value of b, so they are no longer equal.