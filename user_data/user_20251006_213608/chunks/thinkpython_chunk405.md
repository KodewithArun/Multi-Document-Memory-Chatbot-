17.12. Glossary

Keeping the interface separate from the implementation means that you have to hide the attributes. Code in other parts of the program (outside the class deﬁnition) should use methods to read and modify the state of the object. They should not access the attributes di- rectly. This principle is called information hiding; see http://en.wikipedia.org/wiki/ Information_hiding. Exercise 17.6. Download the code from this chapter (http://thinkpython.com/code/ Time2.py). Change the attributes of Time to be a single integer representing seconds since mid- night. Then modify the methods (and the function int_to_time) to work with the new implemen- tation. You should not have to modify the test code in main. When you are done, the output should be the same as before. Solution: http://thinkpython.com/code/Time2_soln.py

17.12 Glossary

object-oriented language: A language that provides features, such as user-deﬁned classes