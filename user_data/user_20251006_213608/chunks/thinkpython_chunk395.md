self.hour = hour

stores the value of the parameter hour as an attribute of self.

The parameters are optional, so if you call Time with no arguments, you get the default values. >>> time = Time() >>> time.print_time() 00:00:00 If you provide one argument, it overrides hour: >>> time = Time (9) >>> time.print_time() 09:00:00 If you provide two arguments, they override hour and minute. >>> time = Time(9, 45) >>> time.print_time() 09:45:00

And if you provide three arguments, they override all three default values. Exercise 17.2. Write an init method for the Point class that takes x and y as optional parameters and assigns them to the corresponding attributes.

17.6. The __str__ method

17.6 The __str__ method

__str__ is a special method, like __init__, that is supposed to return a string representa- tion of an object.

For example, here is a str method for Time objects:

# inside class Time:

def __str__(self):

’

return

%.2d:%.2d:%.2d

’

% (self.hour, self.minute, self.second)