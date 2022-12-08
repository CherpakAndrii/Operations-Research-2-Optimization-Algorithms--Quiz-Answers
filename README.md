# Operations-Research-2-Optimization-Algorithms--Quiz-Answers
## Coursera quiz answers

* [Quiz for Week 1 (100%)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-1)
* [Quiz for Week 2 (100%)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-2)
* [Quiz for Week 3 (not ready)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-3)
* [Quiz for Week 4 (not ready)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-4)
* [Quiz for Week 5 (not ready)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-5)
* [Quiz for Week 6 (not ready)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-6)

# Week 1

### Question 1: Among the following terms, which is not going to be introduced in this course?
* Advanced solvers.
* Exact algorithms.
* ***Data mining.***
* Heuristic algorithms.
* None of the above.

### Question 2: Among the following terms, which is not a characteristic of heuristic algorithms?
* Completing execution in a reasonably short time.
* ***Finding an optimal solution every time.***
* Finding a feasible solution when the problem is too complicated.
* All of the above.
* None of the above.

### Question 3: Please solve the following linear system by Gaussian elimination: 
```
u + 2v + 3w = 19
4u + 3v + 2w = 41
2u − 6v + w = −2
```
#### What are the values of u, v, and w?

* u = 7, v = 3, w = 1.
* u = 4, v = 2, w = 1.
* u = 7, v = 2, w = 2.
* ***u = 7, v = 3, w = 2.***
* The system is singular.

### Question 4: Regarding the following three vectors, which statement is not true?
```
x=[2, 4, −2]
y=[1, 3, −2]
z=[1, −1, 2]
```
* If we put all vectors into the columns of a matrix, the number of pivots is 2.
* The three vectors are linearly dependent.
* There are exactly 2 linear independent vectors.
* We may linearly combine  xx and yy to generate zz.
* ***If we put all vectors into the columns of a matrix, the matrix is nonsingular.***

### Question 5: Which of the following statements is not true?
* The time complexity of Gaussian elimination is O(n3) for an nxn linear system.
* ***A linear system must be singular when a zero appears in a pivot position during the Gaussian elimination process.***
* If a matrix A is invertible, then A^(-1) must be unique.
* A square matrix is nonsingular if and only if it is invertible.
* If we have m n-dimensional vectors, they must be linearly dependent if m > n.

# Week 2

### Question 1: Consider the following LP:
```
max 5*x1 + 3*x2
x1 + x2 <= 16
x1 + 4*x2 <= 20
x2 <= 8
x1 >= 0, x2 >= 0
```
#### If we find its standard form, what will be the first functional constraint look like?
* x1 + x2 + x3 <= 16
* ***x1 + x2 + x3 = 16***
* x1 + x2 - x3 >= 16
* x1 + x2 - x3 = 16

### Question 2: Following from the previous problem, we may list all the basic solutions of the standard form. For this example, there should be A basic variables and B nonbasic variables in each basic solution. There are C basic solutions and D basic feasible solutions.
* A=3, B=2, C=10, and D=4.
* A = 2A=2, B = 3B=3, C = 10C=10, and D = 4D=4.
* A = 2A=2, B = 3B=3, C = 9C=9, and D = 4D=4.
* A = 3A=3, B = 2B=2, C = 4C=4, and D = 9D=9.
* ***None of the above.***

### Question 3: Following from the previous problem. Use the simplex method to solve the linear program. After a few iterations, we obtain an optimal tableau:
0 | 2 | A | 0 | 0 | 80
--|---|---|---|---|---
1 | 1 | 1 | 0 | 0 | 16
0 | B | -1| 1 | 0 | 4
0 | 1 | 0 | 0 | 1 | C
#### where A, B, and C are missing. Please write down these missing values in the order of A, B, and C by separating two consecutive values with a comma. Do not have any symbol other than numeric values, negation, and comma in your answer.

***Answer:***
```
5,3,8
```

### Question 4: Following from the previous problem, what is an optimal solution to the original LP?

* (x1,x2)=(8,8).
* ***(x1, x2) = (16, 0).***
* The original LP is infeasible.
* The original LP is unbounded.
* None of the above.

### Question 5: Consider the following LP:
```
max x1 + 2*x2
x1 + x2 <= 16
x1 + 4*x2 <= 20
x2 <= 8
x1 >= 0, x2 >= 0
```
#### Use the simplex method with the two-phase implementation to solve the LP. Write down your conclusion. If you find an optimal solution, write it down in the order of x1 and x2 by separating two consecutive values with a comma. Do not have any symbol other than numeric values, negation, and comma in your answer. For example, if you believe an optimal solution is (0, 0), write down "0,0". If you conclude that the problem is infeasible or unbounded, write down a single character "I" or "U", respectively.

***Answer:***
```
8,8
```
