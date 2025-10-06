16.5 Debugging

A Time object is well-formed if the values of minute and second are between 0 and 60 (including 0 but not 60) and if hour is positive. hour and minute should be integral values, but we might allow second to have a fraction part.

Requirements like these are called invariants because they should always be true. To put it a different way, if they are not true, then something has gone wrong.

Writing code to check your invariants can help you detect errors and ﬁnd their causes. For example, you might have a function like valid_time that takes a Time object and returns False if it violates an invariant: def valid_time(time):

if time.hour < 0 or time.minute < 0 or time.second < 0:

return False

if time.minute >= 60 or time.second >= 60:

return False

return True

Then at the beginning of each function you could check the arguments to make sure they are valid:

def add_time(t1, t2):

if not valid_time(t1) or not valid_time(t2): ’

raise ValueError(