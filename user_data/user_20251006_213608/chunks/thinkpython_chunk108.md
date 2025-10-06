Now you can access pi directly, without dot notation. >>> print pi 3.14159265359

Or you can use the star operator to import everything from the module: >>> from math import * >>> cos(pi) -1.0

The advantage of importing everything from the math module is that your code can be more concise. The disadvantage is that there might be conﬂicts between names deﬁned in different modules, or between a name from a module and one of your variables.

3.14 Debugging

If you are using a text editor to write your scripts, you might run into problems with spaces and tabs. The best way to avoid these problems is to use spaces exclusively (no tabs). Most text editors that know about Python do this by default, but some don’t.

Tabs and spaces are usually invisible, which makes them hard to debug, so try to ﬁnd an editor that manages indentation for you.