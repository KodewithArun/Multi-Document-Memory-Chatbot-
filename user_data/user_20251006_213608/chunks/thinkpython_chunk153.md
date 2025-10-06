conditional statement.

recursion: The process of calling the function that is currently executing.

base case: A conditional branch in a recursive function that does not make a recursive call.

inﬁnite recursion: A recursion that doesn’t have a base case, or never reaches it. Eventu-

ally, an inﬁnite recursion causes a runtime error.

5.14 Exercises

Exercise 5.3. Fermat’s Last Theorem says that there are no positive integers a, b, and c such that

an + bn = cn

for any values of n greater than 2.

1. Write a function named check_fermat that takes four parameters—a, b, c and n—and that checks to see if Fermat’s theorem holds. If n is greater than 2 and it turns out to be true that

an + bn = cn

the program should print, “Holy smokes, Fermat was wrong!” Otherwise the program should print, “No, that doesn’t work.”