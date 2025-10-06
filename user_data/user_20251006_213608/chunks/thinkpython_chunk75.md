Variable names can be arbitrarily long. They can contain both letters and numbers, but they have to begin with a letter. It is legal to use uppercase letters, but it is a good idea to begin variable names with a lowercase letter (you’ll see why later).

2.4. Operators and operands

The underscore character, _, can appear in a name. It is often used in names with multiple words, such as my_name or airspeed_of_unladen_swallow.

If you give a variable an illegal name, you get a syntax error:

’

’

big parade

>>> 76trombones = SyntaxError: invalid syntax >>> more@ = 1000000 SyntaxError: invalid syntax >>> class = SyntaxError: invalid syntax

’

Advanced Theoretical Zymurgy

’

76trombones is illegal because it does not begin with a letter. more@ is illegal because it contains an illegal character, @. But what’s wrong with class?