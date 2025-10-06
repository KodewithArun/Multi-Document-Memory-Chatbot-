def add_time(t1, t2):

if not valid_time(t1) or not valid_time(t2): ’

raise ValueError(

invalid Time object in add_time

’

)

seconds = time_to_int(t1) + time_to_int(t2) return int_to_time(seconds)

Or you could use an assert statement, which checks a given invariant and raises an ex- ception if it fails:

def add_time(t1, t2):

assert valid_time(t1) and valid_time(t2) seconds = time_to_int(t1) + time_to_int(t2) return int_to_time(seconds)

assert statements are useful because they distinguish code that deals with normal condi- tions from code that checks for errors.

16.6 Glossary

prototype and patch: A development plan that involves writing a rough draft of a pro-

gram, testing, and correcting errors as they are found.

planned development: A development plan that involves high-level insight into the prob-

lem and more planning than incremental development or prototype development.

155

156

Chapter 16. Classes and functions