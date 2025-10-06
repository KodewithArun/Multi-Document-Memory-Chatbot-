>>> db.close()

14.7 Pickling

A limitation of anydbm is that the keys and values have to be strings. If you try to use any other type, you get an error.

The pickle module can help. It translates almost any type of object into a string suitable for storage in a database, and then translates strings back into objects.

pickle.dumps takes an object as a parameter and returns a string representation (dumps is short for “dump string”):

137

138

Chapter 14. Files

>>> import pickle >>> t = [1, 2, 3] >>> pickle.dumps(t) ’

(lp0\nI1\naI2\naI3\na.

’

The format isn’t obvious to human readers; it is meant to be easy for pickle to interpret. pickle.loads (“load string”) reconstitutes the object: >>> t1 = [1, 2, 3] >>> s = pickle.dumps(t1) >>> t2 = pickle.loads(s) >>> print t2 [1, 2, 3]

Although the new object has the same value as the old, it is not (in general) the same object: >>> t1 == t2 True >>> t1 is t2 False