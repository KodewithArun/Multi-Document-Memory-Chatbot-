Most of the time, an inﬁnite recursion will cause the program to run for a while and then produce a “RuntimeError: Maximum recursion depth exceeded” error. If that happens, go to the “Inﬁnite Recursion” section below. If you are not getting this error but you suspect there is a problem with a recursive method or function, you can still use the techniques in the “Inﬁnite Recursion” sec- tion.

If neither of those steps works, start testing other loops and other recursive functions and methods.

If that doesn’t work, then it is possible that you don’t understand the ﬂow of execu- tion in your program. Go to the “Flow of Execution” section below.

195

196

Appendix A. Debugging

Inﬁnite Loop

If you think you have an inﬁnite loop and you think you know what loop is causing the problem, add a print statement at the end of the loop that prints the values of the variables in the condition and the value of the condition.

For example: