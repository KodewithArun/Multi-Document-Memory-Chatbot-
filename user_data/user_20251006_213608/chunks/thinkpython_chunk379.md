In general, I recommend that you write pure functions whenever it is reasonable and resort to modiﬁers only if there is a compelling advantage. This approach might be called a functional programming style. Exercise 16.4. Write a “pure” version of increment that creates and returns a new Time object rather than modifying the parameter.

153

154

Chapter 16. Classes and functions

16.4 Prototyping versus planning

The development plan I am demonstrating is called “prototype and patch.” For each func- tion, I wrote a prototype that performed the basic calculation and then tested it, patching errors along the way.

This approach can be effective, especially if you don’t yet have a deep understanding of the problem. But incremental corrections can generate code that is unnecessarily complicated—since it deals with many special cases—and unreliable—since it is hard to know if you have found all the errors.