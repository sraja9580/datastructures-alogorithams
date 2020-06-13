# Recursion
## 3 properties of recursion
  	1. an operation performed multiple times with different input
	2. every step we trying to make problem smaller
	3. mandatory base condition to exit the recursion,without this we might end up in infinite loop
  
## Why Recursion?
   	if we can break our problem into similar sub problem we can use recursion
	 make our code easy to read and write
	 Dealing with tree and grapes are much simpler	
   
##Structure of recursive method

  	recursive case -> when the function recur
	base case -> when the function stop
	
	simpleRecursion(param){
		if(base condition satisfied)
			return result
		else
			simpleRecursion(modified param)
	}
  
##How Recursion Works internally?

##When to use recursion when to avoid?
  1. when we can break down a problem into subproblem of similar nature
	2. it always comes with little time and memory overhead, if it not issue you can proceed with recursion
	example: let's say we are working on a airbag launch system there time is really important ,so we have to avoid recursion
  
##Practical uses of recursion
  Stack
  Tree
  Quick sort
  Merge sort 
  divide and conquer
  dynamic programing



