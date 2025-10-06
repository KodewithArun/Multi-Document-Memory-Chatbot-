On the other hand, inheritance can make programs difﬁcult to read. When a method is invoked, it is sometimes not clear where to ﬁnd its deﬁnition. The relevant code may be scattered among several modules. Also, many of the things that can be done using inheritance can be done as well or better without it.

18.8 Class diagrams

So far we have seen stack diagrams, which show the state of a program, and object dia- grams, which show the attributes of an object and their values. These diagrams represent a snapshot in the execution of a program, so they change as the program runs.

They are also highly detailed; for some purposes, too detailed. A class diagram is a more abstract representation of the structure of a program. Instead of showing individual ob- jects, it shows classes and the relationships between them.

173

174

Chapter 18. Inheritance

HandDeck*Card

Figure 18.2: Class diagram.

There are several kinds of relationship between classes: