print

’

Blastoff!

’

else:

print n countdown(n-1)

If n is 0 or negative, it outputs the word, “Blastoff!” Otherwise, it outputs n and then calls a function named countdown—itself—passing n-1 as an argument.

What happens if we call this function like this? >>> countdown(3)

The execution of countdown begins with n=3, and since n is greater than 0, it outputs the value 3, and then calls itself...

The execution of countdown begins with n=2, and since n is greater than 0, it outputs the value 2, and then calls itself...

The execution of countdown begins with n=1, and since n is greater than 0, it outputs the value 1, and then calls itself...

The execution of countdown begins with n=0, and since n is not greater than 0, it outputs the word, “Blastoff!” and then returns.

5.9. Stack diagrams for recursive functions

The countdown that got n=1 returns.

The countdown that got n=2 returns.

The countdown that got n=3 returns.