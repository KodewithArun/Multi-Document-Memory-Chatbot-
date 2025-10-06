The return value (1) is multiplied by n, which is 2, and the result is returned.

The return value (2) is multiplied by n, which is 3, and the result, 6, becomes the return value of the function call that started the whole process.

Figure 6.1 shows what the stack diagram looks like for this sequence of function calls.

The return values are shown being passed back up the stack. In each frame, the return value is the value of result, which is the product of n and recurse.

In the last frame, the local variables recurse and result do not exist, because the branch that creates them does not execute.

6.6. Leap of faith

n3recurse2recurse1recurse1<module>factorialn2n1n0factorialfactorialfactorial11261result26resultresult

Figure 6.1: Stack diagram.

6.6 Leap of faith