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
### Stack Implemenentation using array Time and Space complexity table
![big-O-table](/images/logical-ds/stack/8_1_4_stack_array_time-space-complexity-table.PNG) <br>
### CreateStack
![stack create](/images/logical-ds/stack/8_1_1_create_stack_array.PNG) <br>
**_Algorithm_**
```
CreateStack(size)
  create blank array of size -- O(1)
  //topOfStack=-1 is current pos=-1 which means no element is pushed(**stack is empty**)
  topOfStack=-1              -- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### Push
![push](/images/logical-ds/stack/8_1_2_stack_array_pushPNG) <br>
**_Algorithm_**
```
push(value)
  if stack is full (ie topOfStack == array.size)-- O(1)
    return error message-------------------------- O(1)
  else
    arry[topOfStack]= value ---------------------- O(1)
    topOfStack=topOfStack+1  --------------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### Pop
![top](/images/logical-ds/stack/8_1_3_stack_array_pop.PNG) <br>
**_Algorithm_**
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
**_Algorithm_**
```
peak()
  if stack empty (ie topOfStack == -1) -- O(1)
    return error message ---------------- O(1)
  else
    return arry[topOfStack] ------------- O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### isEmpty
**_Algorithm_**
```
isEmpty()
  if stack empty (ie topOfStack == -1) -- O(1)
    return true--------- ---------------- O(1)
  else
    return false----------- ------------- O(1)   
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### isFull
**_Algorithm_**
```
isFull()
  if stack full (ie topOfStack == array.size) -- O(1)
    return true -------------------------------- O(1)
  else
    return false ------------------------------- O(1)     
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### DeleteStack
**_Algorithm_**
```
DeleteStack()
 array = null ------ O(1) 
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>

## Stack Implemenentation using Linked List
### CreateStack
**_Algorithm_**
```
//As we are using linked list size is dynamic
CreateStack()
  create blank linked list(ie just head) -- O(1)  
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### Push
**_Algorithm_**
```
push(value)
    create new node = newNode -- O(1)
    newNode.value=value -------- O(1)
    newNode.next=head ---------- O(1)
    head=newNode --------------- O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### Pop
**_Algorithm_**
```
pop()
   if stack empty (ie head == null) -- O(1)
      return error message ----------- O(1)
   else
       tempNode = head --------- O(1)
       head=head.next ---------- O(1)   
       return tempNode.value --- O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### Peak
  _In pop top element is removed after returning the value, but in peak top element is not removed,it will just return top element_
**_Algorithm_**
```
peak()
  if stack empty (ie head == null) -- O(1)
    return error message ------------ O(1)
  else
    return head.value --------------- O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### isEmpty
**_Algorithm_**
```
isEmpty()
  if stack empty (head==null) -- O(1)
    return true--------- ---------------- O(1)
  else
    return false----------- ------------- O(1)   
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### ~~isFull~~
_In the linked list implementation **stack size dont have limitation**,we can create as many nodes as possible if ram has memory.**Linked list implementation of stack dont have isFull mehtod as the size is dynamic_ 

### DeleteStack
**_Algorithm_**
```
DeleteStack()
 head = null ------ O(1) 
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>


