# Operations-Research-2-Optimization-Algorithms--Quiz-Answers
## Coursera quiz answers

* [Quiz for Week 1 (100%)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-1)
* [Quiz for Week 2 (100%)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-2)
* [Quiz for Week 3 (80%)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-3)
* [Quiz for Week 4 (80%)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-4)
* [Quiz for Week 5 (100%)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-5)
* [Quiz for Week 6 (100%)](https://github.com/CherpakAndrii/Operations-Research-2-Optimization-Algorithms--Quiz-Answers#week-6)

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

# Week 3

### Question 1: In this problem, we will use the branch-and-bound algorithm to solve the following IP:
```
max 3*x1 + 5*x2
x1 + x2 <= 16
x2 <= 7.5
x1 є Z+, x2 є Z+  
```
#### As always, our first step is to solve the linear relaxation of the given IP. Write down the unique optimal solution in the order of x1 and x2 by separating two consecutive values with a comma. Do not have any symbol other than numeric values, negation, decimal point, and comma in your answer. For example, if you believe an optimal solution is (0.2, −2.3), write down "0.2,-2.3".

***Answer:***
```
8.5, 7.5
```

### Question 2: Following from the previous problem, branch on x1 to obtain two subproblems. What are the two constraints you add to the first subproblem to generate the two new subproblems?
* x1=8 and x1=9.
* x1≤8 and x1≤9.
* ***x1≤8 and x1≥9.***
* x1≤8 and x2≤7.
* None of the above.

### Question 3: Following from the previous problem, find an optimal solution to the original IP. Write down the unique optimal solution in the order of x1 and x2 by separating two consecutive values with a comma. Do not have any symbol other than numeric values, negation, and comma in your answer. For example, if you believe an optimal solution is (2,−3), write down "2,-3".

***Answer:***
```
9,7
```

### Question 4: ***IDK the correct answer :(*** Please, make a comment if you know how to solve it.

### Question 5: Following from the previous problem, whenever we apply a heuristic algorithm on an instance and obtain a feasible solution, we want to evaluate its performance by calculating the optimality gap. For the instance above, as we do not have an optimal solution, we look for a lower bound on the makespan of an optimal solution. To do this, note that we may formulate an IP for the makespan minimization problem, we may then solve its linear relaxation to obtain a lower bound. For the makespan minimization problem, however, there is an easier way: All we need to do is to divide the total processing time by the number of machines (i.e., to calculate ***sum(p(j))/m*** , where J is the set of jobs). The ratio is then a lower bound we need. Let *z^(ALG)* be the makespan you find in the previous problem and z^(LB) be the lower bound you find using the above method, find the (relative) optimality gap (z^(ALG) - z^(LB))/z^(LB). Express the optimality gap in percentages and round it down to the closest integer. For example, if you believe that the optimality gap is 0.06780, which is 6.78%, you should write down 6 as your answer.
***Answer:***
```
2
```

# Week 4

### Question 1: Let f(x) = x1^2 + 2*x2^2. Find the gradient of f(x) at (x1, x2) = (2, 1). Write down a pair of parentheses to include two values separated by a comma. Do not have any symbol other than numeric values, negation, decimal point, comma, and parentheses in your answer. Do not have unnecessary zeros at the end of a number. For example, if you believe the gradient is (0.1, -2.3), write down "0.1,-2.3".

***Answer:***
```
4,4
```

### Question 2: Let's solve min(xєR^2) f(x) = x1^2 + 2*x2^2 by gradient descent. Let x^0 = (1, 0) be the initial solution. Run on iteration of gradient descent to find the next solution x^1. In each iteration, let the step size be that bringing you to the global minimum along the improving direction. Follow the output format requirement provided in Question 1.

***Answer:***
```
0,0
```

### Question 3: Let f(x) = x1^2 + 2*x2^3. Find the Hessian of f(x) at (x1, x2) = (0, 2). Then find its determinant. Write down a single number. Do not have any symbol other than numeric values, negation, and decimal point in your answer. Do not have unnecessary zeros at the end of a number. For example, if you believe the determinant is -9.01, write down "-9.01".

***Answer:***
```
48
```

### Question 4: ***IDK the correct answer :(*** Please, make a comment if you know how to solve it.

### Question 5: Which of the follow statements are correct? Check all correct answers.
* ***Gradient descent is an interior-point method, i.e., its search path is not restricted in the boundary of the feasible region of an optimization problem.***
* Gradient descent is always slower than the Newton's method in solving a nonlinear optimization problem. 
* ***Gradient descent is a first-order method, i.e., it does not require any information about the second-order derivative of the objective function.***
* ***The Newton's method always find an optimal solution when it is used to solve an unconstrained minimization problem whose objective function is quadratic with upward curvature.***
* All of the above.

# Week 5

### Question 1: According to the instructor, what are the major sources of costs in the facility location problem introduced in this week? Check all the correct answers. 

* ***Office rent.***
* ***Traveling cost.***
* ***Engineer hosting cost.***
* Engineer training cost.
* Facility construction cost.

### Question 2: Which of the following statements best describes the main decision to make in the facility location problem discussed in this week? 

* For each location, determine the facility scale and facility type. 
* ***For each location, determine the facility scale and number of engineers hosted here.***
* For each location, determine the number of engineers hosted here.
* For each location, determine whether to build a facility there. 
* None of the above.

### Question 3: What of the following is not one of the three models we need in an Operations Research study? 
* A conceptual model.
* A mathematical model. 
* ***A universal model.***
* A computer model. 
* All of the above.

### Question 4: Recall that in the facility location problem discussed in this week, there is a constraint saying that for each customer and each location, only a built facility may serve customers. Which of the following statement is correct?

* ***The new feasible region becomes smaller or the same. The new formulation is wrong.***
* The new feasible region remains the same. The new formulation is correct.
* The new feasible region becomes larger or the same. The new formulation is wrong. 
* The new feasible region may become smaller or larger. The new formulation is wrong. 
* None of the above. 

### Question 5: Which of the following is the most appropriate category of the heuristic algorithm introduced in this week? 

* A brute-force algorithm.
* A divide-and-conquer algorithm.
* ***A greedy algorithm.***
* A dynamic programming algorithm. 
* A backtracking algorithm.

# Week 6

### Question 1: Fifteen jobs, each with its processing time, should be scheduled on three machines. If two jobs cannot be scheduled on the same machine, they are called conflicting jobs. Table 1 lists the job IDs, processing times, and sets of conflicting jobs. For example, we cannot schedule any pair of jobs out of jobs 2, 5, 8 on the same machine. Note that a job may have no conflicting jobs. We want to schedule the jobs to minimize makespan. For example, we may schedule jobs 1, 4, 7, 8, and 13 to machine 1, jobs 2, 6, 10, 11, and 14 to machine 2, and jobs 3, 5, 9, 12, and 15 to machine 3. The total processing times on the three machines are 52, 39, and 37, respectively. The makespan is thus 52. While this is a feasible schedule, this may or may not be an optimal schedule. When we try to improve the schedule, be careful about conflicting jobs. For example, we cannot exchange jobs 8 and 11 (even though this reduces the makespan) because that will result in machine 2 processing conflicting jobs 2 and 8, which is infeasible. Formulate a linear integer program that generates a feasible schedule to minimize makespan. Then write a computer program (e.g., using Python to invoke Gurobi Optimizer) to solve this instance and obtain an optimal schedule. Write down the minimized makespan (i.e. the objective value of an optimal solution). Do not have any symbol other than numeric values in your answer.

***Answer:***
```
43
```

### Question 2: A city is divided into nn districts. The time (in minutes) it takes an ambulance to travel from District i to District j is denoted as d(ij). The population of District i (in thousands) is p(i). An example is shown in Table 2 and Table 3. The distances between districts are shown in Table 2, and the population information is shown in Table 3. In this instance, we have n = 8 districts. We may see that, e.g., it takes 5 minutes to travel from District 2 to District 3, and there are 40,000 citizens. The city has m ambulances and wants to locate them to m of the districts. For each district, the population-weighted firefighting time is defined as the product of the district population times the amount of time it takes for the closest ambulance to travel to it. The decision maker aims to locate the m ambulances to minimize the maximum population-weighted firefighting time among all districts.
As an example, suppose that m = 2, n = 8, d(ij) and p(ip) are provided in Table 2, and the two ambulances are located in District 1 and 8. We then know that for Districts 1, 2, and 3 the closest ambulance is in District 1 and for the remaining five districts the closet ambulance is in District 8. The firefighting time for the eight districts are thus 0, 3, 4, 4, 4, 2, 2, and 0 minutes, respectively. The population-weighted firefighting times may then be calculated as 0, 90, 140, 80, 60, 100, 90, and 0. The maximum among the eight districts is therefore 140. For this problem, formulate an integer program that can minimize the maximum population-weighted firefighting time among all districts. Then write a program to invoke a solver (e.g., write a Python program to invoke Gurobi Optimizer) to solve the above instance and find an optimal solution for each problem. Write down the minimized maximum population-weighted firefighting times among all districts of the two districts that ambulances should be located in (i.e., the objective value of an optimal solution). Do not have any symbol other than numeric values in your answer.

***Answer:***
```
135
```

### Question 3: Continue from the previous question. For any value of m, consider the following heuristic algorithm which runs m iterations. In each iteration, we locate an ambulance in a district that currently does not have an ambulance, and may minimize the maximum population-weighted firefighting times among all districts. If there are multiple districts satisfying these two conditions, pick the one with the smallest district ID among them. We then proceed to the next iteration to look for the next district to locate an ambulance. Consider a tiny example with n = 4, m = 2, and d(ij) and p(j) are provided in Table 4 and Table 5. To locate the first ambulance, we examine the maximum population-weighted firefighting times of locating an ambulance in Districts 1, 2, 3, and 4 as 140, 175, 160, and 240, respectively. We will choose District 1. To locate the second ambulance, we take the ambulance in District 1 as given and examine the maximum population-weighted firefighting times of locating an ambulance in Districts 2, 3, and 4 as 140, 90, and 90, respectively. We will choose District 3. The final objective value of locating two ambulances in Districts 1 and 3 is 90 (which is 30*3 for District 2). Coming back to the instance provided in Table 2 and Table 3 with n = 8. Now let m = 3. Use the heuristic algorithm introduced above to generate a feasible solution. Then use the program you wrote for Question 2 to generate an optimal solution. Write down the absolute optimality gap between the two solutions (i.e., the difference between the two objective values). Do not have any symbol other than numeric values in your answer.

***Answer:***
```
0
```
