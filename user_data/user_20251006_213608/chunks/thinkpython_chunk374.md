"""Represents the time of day.

attributes: hour, minute, second """

We can create a new Time object and assign attributes for hours, minutes, and seconds: time = Time() time.hour = 11 time.minute = 59 time.second = 30 The state diagram for the Time object looks like Figure 16.1. Exercise 16.1. Write a function called print_time that takes a Time object and prints it in the form hour:minute:second. Hint: the format sequence prints an integer using at least two digits, including a leading zero if necessary. Exercise 16.2. Write a boolean function called is_after that takes two Time objects, t1 and t2, and returns True if t1 follows t2 chronologically and False otherwise. Challenge: don’t use an if statement.

’

’

%.2d

16.2 Pure functions