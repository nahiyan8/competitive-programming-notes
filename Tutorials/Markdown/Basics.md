## Basics

### Prerequisites

These tutorials provide a high-level overview of the problem-solving techniques that you can use to get better at competitive programming. I believe that everyone can derive some benefit from these materials; however, you will get the most out of them if you have some prior experience in fundamental computer science topics. In particular, you should be familiar with big-O notation for time and space complexity (and be able to apply it), and you should know basic algorithms and data structures.

If you want to get up to speed on these topics, I recommend Stanford's algorithms courses on Coursera ([part 1](https://www.coursera.org/course/algo) and [part 2](https://www.coursera.org/course/algo2)). They strike a good balance between clarity/accessibility and conciseness.

I will also assume some basic knowledge of discrete math.

Of course, you should also know at least one programming language and its standard library. Code snippets in these tutorials will use Python, but C++ is another common choice. I personally tend to use Python for some problems and C++ for others; I know some people who use Java for everything. It's a matter of personal preference. Regardless, you should have some level basic literacy in Python if you want to understand the code snippets in these tutorials.

### Reading problem statements

Programming competitions usually have between 5 and 10 problems, of varying levels of difficulty. Each problem statement has several components:

* a description of the problem
* the numerical constraints of the problem
* a description of the input
* a description of the expected output
* sample input and output

Problem statements can be given in lengthy English prose, concise mathematical statements, or something in between. Sometimes the most difficult and time-consuming part of solving a problem is reading and understanding the description!

Problem statements should be read very carefully and any ambiguities should be resolved *before* coding begins. This careful reading saves time in the long run--there are times that I have spent more than an hour solving a problem only to find out that my approach does not work on the sample input because I misinterpreted the problem statement.

Once you have some experience solving certain types of problems, you'll be able to read and understand problems more quickly. In the early minutes of a programming competition, the scoreboard is volatile and many competitors try to be the first to solve the easy problems to get a boost. This is a losing strategy: make sure you understand the problems you are solving before you try to solve them. With practice, you'll get faster; in a well-written contest, the final standings will be reflective of the actual skill of the competitors, not their reading speed.

### Time complexity

After reading a problem statement, be sure to check the constraints so you know how fast your solution needs to be. If the input size is at most 10, a brute-force algorithm will work; if N can be 1,000,000, something more clever is necessary.

A good rule of thumb is to assume that a computer can execute 10^8 operations per second. Substitute the maximum input size of the problem into your big-O time bound, divide by the time limit in seconds, and if the result is less than 10^8, your algorithm will probably be fast enough. Now, we aren't taking into account constant factors, and sometimes those make a difference: for example, both quicksort and fast Fourier transform run in O(N log N) time, but in practice you're much less likely to run into time trouble with the former than with the latter on problems with similar maximum input sizes.

### Input and output

Different contests use different means of reading input and returning output. Most modern platforms use standard I/O, but there are notable exceptions (for example, USACO requires reading from and writing to files). Make sure you know how to handle I/O before the competition begins.

### Templates

You will often see competitive programmers use large templates in their solutions (and I'm talking about blocks of prewritten code, not C++ generic types). These often consist of macros for common tasks (`for` loops, `pair` and `make_pair`, etc.). I don't use them, and for now neither should you. Typing speed will not be the limiting factor in your learning competitive programming. Neither of us is good enough for macros or templates to make a difference.
