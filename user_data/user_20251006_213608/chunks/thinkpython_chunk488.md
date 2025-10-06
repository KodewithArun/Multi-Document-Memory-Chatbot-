Another problem that can occur with big expressions is that the order of evaluation may not be what you expect. For example, if you are translating the expression x 2π into Python, you might write: y = x / 2 * math.pi

That is not correct because multiplication and division have the same precedence and are evaluated from left to right. So this expression computes xπ/2.

A good way to debug expressions is to add parentheses to make the order of evaluation explicit:

y = x / (2 * math.pi)

Whenever you are not sure of the order of evaluation, use parentheses. Not only will the program be correct (in the sense of doing what you intended), it will also be more readable for other people who haven’t memorized the rules of precedence.

A.3.3

I’ve got a function or method that doesn’t return what I expect.