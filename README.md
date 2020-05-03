# GeneralSequenceExpression
Calculation of the general expression of a_n element from a sequence

## Mathematical approach - Fibonacci
Fibonacci is a sequence of integers numbers that: 

* a_n = a_(n-1) + a_(n-2) 
* a_0 = 0
* a_1 = 1 

How to calculate an expression to a_n ?

### Solution

a_n = a_(n-1) + a_(n-2) ---> x^2 - x - 1 = 0

The roots are:

* x1 = 0.5 + sqrt(5)/2
* x2 = 0.5 - sqrt(5)/2

Then, a_n = A.(x1)^n + B.(x2)^n, where A and B are constant. 
a_0 = A + B = 0
a_1 = A.x1 + B.x2 = 1

Solving the system of equations we get:
* A = 0.4472136
* B = -0.4472136

Finally, the general expression to a_n for fibonacci sequence is:

a_n = (0.4472136).(0.5 + sqrt(5)/2)^n + (-0.4472136).(0.5 - sqrt(5)/2)^n

If n=3, then a_n = 3, which satisfy the sequence recurrence. 
