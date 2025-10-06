18.10 Data encapsulation

Chapter 16 demonstrates a development plan we might call “object-oriented design.” We identiﬁed objects we needed—Time, Point and Rectangle—and deﬁned classes to repre- sent them. In each case there is an obvious correspondence between the object and some entity in the real world (or at least a mathematical world).

But sometimes it is less obvious what objects you need and how they should interact. In that case you need a different development plan. In the same way that we discovered function interfaces by encapsulation and generalization, we can discover class interfaces by data encapsulation.

Markov analysis, from Section 13.8, provides a good example. If you download my code from http://thinkpython.com/code/markov.py, you’ll see that it uses two global variables—suffix_map and prefix—that are read and written from several functions.

suffix_map = {} prefix = ()