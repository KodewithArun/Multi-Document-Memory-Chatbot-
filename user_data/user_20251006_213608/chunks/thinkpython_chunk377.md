16.3. Modiﬁers

if sum.second >= 60: sum.second -= 60 sum.minute += 1

if sum.minute >= 60: sum.minute -= 60 sum.hour += 1

return sum

Although this function is correct, it is starting to get big. We will see a shorter alternative later.

16.3 Modiﬁers

Sometimes it is useful for a function to modify the objects it gets as parameters. In that case, the changes are visible to the caller. Functions that work this way are called modiﬁers.

increment, which adds a given number of seconds to a Time object, can be written naturally as a modiﬁer. Here is a rough draft: def increment(time, seconds): time.second += seconds

if time.second >= 60: time.second -= 60 time.minute += 1

if time.minute >= 60: time.minute -= 60 time.hour += 1

The ﬁrst line performs the basic operation; the remainder deals with the special cases we saw before.

Is this function correct? What happens if the parameter seconds is much greater than sixty?