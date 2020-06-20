# Stack
Stack follows **Last In First Out**
Browser back button has same principle of stack
As Stack is logical data structure it can be implemented using array or linked list(physical DS)
## Array Vs List implementation
|DS         |Pros               |Cons |
|---        |------             |-----|
|Array      | Easy to implement |fixed size (or) even in the case of dynamic array time complexity to increase the size is more|
|Linked List| Variable Size     |ListiImplementation stack is complex than array impementation of stack     |
## Operations
* CreateStack()
* push()
* pop()
* peak()
* isEmpty()
* isFull()
* DeleteStack()
## Stack Implemenentation using array
### CreateStack
**Algorithm**
```
CreateStack(size)
  create blank array of size -- O(1)
  //topOfStack=-1 is current pos=-1 which means no element is pushed(**stack is empty**)
  topOfStack=-1              -- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### Push
**Algorithm**
```
push(value)
  if stack is full (ie topOfStack == array.size)-- O(1)
    return error message-------------------------- O(1)
  else
    arry[topOfStack]= value ---------------------- O(1)
    topOfStack=topOfStack+1  --------------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### Push
**Algorithm**
```
pop()
  if stack empty (ie topOfStack == -1) -- O(1)
    return error message ---------------- O(1)
  else
    return arry[topOfStack] ------------- O(1)
    topOfStack=topOfStack-1 ------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### Peak
  _In pop top element is removed after returning the value, but in peak top element is not removed,it will just return top element_
**Algorithm**
```
peak()
  if stack empty (ie topOfStack == -1) -- O(1)
    return error message ---------------- O(1)
  else
    return arry[topOfStack] ------------- O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>


