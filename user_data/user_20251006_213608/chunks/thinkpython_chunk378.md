Is this function correct? What happens if the parameter seconds is much greater than sixty?

In that case, it is not enough to carry once; we have to keep doing it until time.second is less than sixty. One solution is to replace the if statements with while statements. That would make the function correct, but not very efﬁcient. Exercise 16.3. Write a correct version of increment that doesn’t contain any loops.

Anything that can be done with modiﬁers can also be done with pure functions. In fact, some programming languages only allow pure functions. There is some evidence that programs that use pure functions are faster to develop and less error-prone than programs that use modiﬁers. But modiﬁers are convenient at times, and functional programs tend to be less efﬁcient.