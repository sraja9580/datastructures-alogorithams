# Queue
  First In First Out (FIFO)
## Operations
* CreateQueue()
* enQueue() 
* deQueue()
* peekInQueue()
* isEmpty()
* isFull()
* deleteQueue()
## Queue implementations
  * Array Implementation
    * Linear Queue
    * Circular Queue
  * Linked List implementation
  
## Queue -Linear Array
### CreateQueue
**_Algorithm_**
```
CreateQueue(queueSize)
  create blank array of queueSize -- O(1)
  beginingOfQueue=-1 --------------- O(1)
  topOfqueue=-1 -------------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(n)** <br> <br>
### EnQueue
  _addling value to queue_<br>
**_Algorithm_**
```
EnQueue(value)
  if queue==full (ie topOfqueue == arr.size-1) -- O(1)
    return errorMessage ------------------------- O(1)
  else   ---------------------------------------- O(1)
    arr[topOfqueue+1]=value --------------------- O(1)
    topOfqueue=topOfqueue+1 --------------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### DeQueue
  _returning and removing last element_<br>
**_Algorithm_**
```
DeQueue()
  if queue==empty (ie beginingOfQueue ==-1) -- O(1)
    return errorMessage ---------------------- O(1)
  else   
    tempVal=arr[beginingOfQueue] ------------- O(1)
    beginingOfQueue=beginingOfQueue+1 -------- O(1)
    
    //Last value dequeued,then we can reset
    if(beginingOfQueue>topOfqueue) ----------- O(1)
      beginingOfQueue=-1 --------------------- O(1)
      topOfqueue=-1 -------------------------- O(1)  
      
     return tempVal ------------------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### peekInQueue
  _return first value,it is like peak in stack_<br>
**_Algorithm_**
```
peekInQueue()
  if queue==empty (ie beginingOfQueue ==-1) -- O(1)
    return errorMessage ---------------------- O(1)
  else   
    return arr[beginingOfQueue] -------------- O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### isEmpty 
**_Algorithm_**
```
isEmpty()
  if beginingOfQueue ==-1  -- O(1)
    return true ------------- O(1)
  else   
    return false ------------ O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### isFull 
**_Algorithm_**
```
isFull()
 if topOfqueue == arr.size-1  -- O(1)
    return true ---------------- O(1)
  else   
    return false --------------- O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### deleteQueue 
**_Algorithm_**
```
deleteQueue()
 arr=null
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
## Queue -Circular array
### EnQueue
  _addling value to queue_<br>
**_Algorithm_**
```
EnQueue(value)
  if queue==full (ie topOfqueue == arr.size-1) -- O(1)
    return errorMessage ------------------------- O(1)
  else   ---------------------------------------- O(1)
    arr[topOfqueue+1]=value --------------------- O(1)
    topOfqueue=topOfqueue+1 --------------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### DeQueue
  _returning and removing last element_<br>
**_Algorithm_**
```
DeQueue()
  if queue==empty (ie beginingOfQueue ==-1) -- O(1)
    return errorMessage ---------------------- O(1)
  else   
    tempVal=arr[beginingOfQueue] ------------- O(1)
    beginingOfQueue=beginingOfQueue+1 -------- O(1)
    
    //Last value dequeued,then we can reset
    if(beginingOfQueue>topOfqueue) ----------- O(1)
      beginingOfQueue=-1 --------------------- O(1)
      topOfqueue=-1 -------------------------- O(1)  
      
     return tempVal ------------------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>

### isEmpty 
**_Algorithm_**
```
isEmpty()
  if endPos ==-1  -- O(1)
    return true ------------- O(1)
  else   
    return false ------------ O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### isFull 
**_Algorithm_**
```
isFull()
 if endPos+1 == startPos-------- O(1)
    return true ---------------- O(1)
  else   
    return false --------------- O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>


