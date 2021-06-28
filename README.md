# CPSC-335-Project-4
__Group Members: Maria Ortega and Neal Vaghasia__


__Introduction__

The project asked to develop and analyze a dynamic programming algorithm and compare its implementation to several alternatives. There are two components:

   1. Pseudocode and a written mathematical analysis
   2. Implementation of your pseudocode and several alternatives in C++


__i. Mathematical Analysis__

Complete Exercise 11-3 (a) from Algorithm Design in Three Acts.


![image](https://user-images.githubusercontent.com/79822470/123563801-8e12c780-d76b-11eb-8f5b-bd69922544ce.png)

    def dynamic(n):

	  A = Array(max(n+1, 3), None)
  
      A[0] = 0 
	
      A[1] = 0
      
      A[2] = 1
	
      for i in range(3, n+1):
	
        A[i] = A[i-3] + A[i-2] + A[i-1]
	
      return A[n]


Time complexity _O(n)_. 


__ii. Implementation in C++__

This project required us to implement four programs in C++17. Each of these programs implemented a solution to the triconacci number problem using one of the following:
  1. Naive Pattern
  2. A recursive solution directly implementing the recurrence relation defining the nth tribonacci   
     number.
  3. A recursive solution using memoization.
  4. The Dynamic Programming Pattern, using the algorithm you developed in Part (1).

Each program creates a table of the 25 tribonacci numbers. 
