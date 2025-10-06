Parentheses have the highest precedence and can be used to force an expression to evaluate in the order you want. Since expressions in parentheses are evaluated ﬁrst, 2 * (3-1) is 4, and (1+1)**(5-2) is 8. You can also use parentheses to make an expression easier to read, as in (minute * 100) / 60, even if it doesn’t change the result.

Exponentiation has the next highest precedence, so 2**1+1 is 3, not 4, and 3*1**3 is 3, not 27.

Multiplication and Division have the same precedence, which is higher than Addition and Subtraction, which also have the same precedence. So 2*3-1 is 5, not 4, and 6+4/2 is 8, not 5.

Operators with the same precedence are evaluated from left to right (except exponen- tiation). So in the expression degrees / 2 * pi, the division happens ﬁrst and the result is multiplied by pi. To divide by 2π, you can use parentheses or write degrees / 2 / pi.