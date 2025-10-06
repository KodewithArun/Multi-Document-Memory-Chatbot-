Of course, you should be building and testing components as you develop the program. If you encounter a problem, there should be only a small amount of new code that is not known to be correct.

A.3.2

I’ve got a big hairy expression and it doesn’t do what I expect.

Writing complex expressions is ﬁne as long as they are readable, but they can be hard to debug. It is often a good idea to break a complex expression into a series of assignments to temporary variables.

For example: self.hands[i].addCard(self.hands[self.findNeighbor(i)].popCard())

This can be rewritten as: neighbor = self.findNeighbor(i) pickedCard = self.hands[neighbor].popCard() self.hands[i].addCard(pickedCard)

The explicit version is easier to read because the variable names provide additional docu- mentation, and it is easier to debug because you can check the types of the intermediate variables and display their values.