# QOSF Screenig Cohort-7
## Name : S Sreyas

### Task to be evaluated - Task 1
Built the circuit for a 3-qubit quantum comparator in qiskit.

This can further be extrapolated to make a n-qubit quantum comparator circuit. The code can also be modified slightly to make it compatible with negative integers

Range of input values - [0, 3] included

### Thought about Task-2
given the 4 side lengths, we can find the smallest side length and subtract it from all the side lengths

Suppose a, b, c, d were the initial side lengths (ascending),

=> we have 0, b-a, c-a, d-a

We can form a rectangle only if 2 or 4 sides are equal-

we can make a function `f:{00, 01, 10, 11} -> {0, b-a, c-a, d-a}`

we can apply Deutsch-Joszaa algorithm on it.

If the algorithm returns only 0 (constant) or only 1 (balanced), then rectangle can be formed.
Otherwise, if the algorithm returns 0 for some measurements and 1 for some measurements,

=> function is neither constant nor balanced. Therefore no rectangle possible
