self.prefix = shift(self.prefix, word)

Transforming a program like this—changing the design without changing the function—is another example of refactoring (see Section 4.7).

This example suggests a development plan for designing objects and methods:

1. Start by writing functions that read and write global variables (when necessary).

2. Once you get the program working, look for associations between global variables and the functions that use them.

3. Encapsulate related variables as attributes of an object.

4. Transform the associated functions into methods of the new class.

Exercise 18.5. Download my code from Section 13.8 (http://thinkpython.com/code/ markov.py), and follow the steps described above to encapsulate the global variables as attributes of a new class called Markov. Solution: http://thinkpython.com/code/Markov.py (note the capital M).

18.11 Glossary

encode: To represent one set of values using another set of values by constructing a map-

ping between them.