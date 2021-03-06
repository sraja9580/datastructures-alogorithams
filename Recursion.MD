# Recursion
## 3 properties of recursion
  	1. an operation performed multiple times with different input
	2. every step we trying to make problem smaller
	3. mandatory base condition to exit the recursion,without this we might end up in infinite loop
  
## Why Recursion?
   	if we can break our problem into similar sub problem we can use recursion
	make our code easy to read and write
	Dealing with tree and grapes are much simpler	
   
## Structure of recursive method

  	recursive case -> when the function recur
	base case -> when the function stop
	
	simpleRecursion(param){
		if(base condition satisfied)
			return result
		else
			simpleRecursion(modified param)
	}
  
## How Recursion Works internally?
** Normal Method
![normal-method](/images/02_how-system-executes-normal-method.PNG)

** Recursive Method
![recursive-method](/images/03_how-system-executes-recursive-method.PNG)
	
## When to use recursion when to avoid?
  1. when we can break down a problem into subproblem of similar nature
  2. it always comes with little time and memory overhead, if it not issue you can proceed with recursion
	example: let's say we are working on a airbag launch system there time is really important ,so we have to avoid recursion
  
## Practical uses of recursion
  Stack
  Tree
  Quick sort
  Merge sort 
  divide and conquer
  dynamic programing
  
 ## Recursive vs Iteration
 ![recVsItr](/images/04_recursive-vs-iteration.PNG) 
 
 ## Example Code Snipt
 ### Fibonacci
	The Fibonacci Sequence is the series of numbers:
	0(f1), 1(f2), 1(f3), 2(f4), 3, 5, 8, 13, 21, 34, ...
	The next number is found by adding up the two numbers before it:
	the 2 is found by adding the two numbers before it (1+1),
	the 3 is found by adding the two numbers before it (1+2),
	
	/* n==0 and n<3 are base conditions 
	 * n>2 is recursive condition
	 */
	static int fibonacciRecursive(int n){	
		if(n==0) {
			return 0;
		}else if(n<3) {
			return n-1;
		}else {
			return fibonacciRecursive(n-1)+fibonacciRecursive(n-2);
		}		
	}
	 


