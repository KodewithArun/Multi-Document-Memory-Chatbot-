1 But if you get a question like this in an interview, I think a better answer is, “The fastest way to sort a million integers is to use whatever sort function is provided by the language I’m using. Its performance is good enough for the vast majority of applications, but if it turned out that my application was too slow, I would use a proﬁler to see where the time was being spent. If it looked like a faster sort algorithm would have a signiﬁcant effect on performance, then I would look around for a good implementation of radix sort.”

202

Appendix B. Analysis of Algorithms

run slower in this case. A common way to avoid this problem is to analyze the worst case scenario. It is sometimes useful to analyze average case performance, but that’s usually harder, and it might not be obvious what set of cases to average over.