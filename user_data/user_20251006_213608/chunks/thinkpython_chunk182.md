One way to ﬁnd the GCD of two numbers is based on the observation that if r is the remainder when a is divided by b, then gcd(a,b) = gcd(b,r). As a base case, we can use gcd(a,0) = a.

61

62

Chapter 6. Fruitful functions

Write a function called gcd that takes parameters a and b and returns their greatest common divisor.

Credit: This exercise is based on an example from Abelson and Sussman’s Structure and Interpre- tation of Computer Programs.

Chapter 7

Iteration

7.1 Multiple assignment

As you may have discovered, it is legal to make more than one assignment to the same variable. A new assignment makes an existing variable refer to a new value (and stop referring to the old value).

bruce = 5 print bruce, bruce = 7 print bruce

The output of this program is 5 7, because the ﬁrst time bruce is printed, its value is 5, and the second time, its value is 7. The comma at the end of the ﬁrst print statement suppresses the newline, which is why both outputs appear on the same line.