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
  
**Queue: Array-Vs-Linked List Implementation**
![DS](/images/logical-ds/queue/Queue_array-vs-linkedlist.PNG) <br> <br>
## Queue -Linear Array
### Time and Space complexity table
![time-complexity-table](/images/logical-ds/queue/1_4_array_linear_queue_time-and-space_complexity.PNG) <br>
### CreateQueue
![create](/images/logical-ds/queue/1_1_array_linear_cereate-queue.PNG) <br>
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
![enqueue](/images/logical-ds/queue/1_2_array_linear_enque.PNG) <br>
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
![dequeue](/images/logical-ds/queue/1_3_array_linear_deque.PNG) <br>
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
### Time and Space complexity table
![DS](/images/logical-ds/queue/2_3_array_circular_queue_time-and-space_complexity.PNG) <br> <br>
### EnQueue
  _addling value to queue_<br>
 ![DS](/images/logical-ds/queue/2_1_array-circular_enque.PNG) <br>
**_Algorithm_**
```
EnQueue(value)
  if queue==full(call isFull method) ---- O(1)
    return errorMessage ----------------- O(1)
  else   -------------------------------- O(1)
    
    if queue=empty(call isEmpty mehtod) - O(1)
      start=0 ---------------------- ---- O(1)
      end=0 ----------------------------- O(1)
    else if end=arr.lenth-1 ------------- O(1)
      end=0 ----------------------------- O(1)
    else -------------------------------- O(1)
      end=end+1 ------------------------- O(1)
	
	//Assigning value
  arr[end]=value ------------------------ O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### DeQueue
  _returning and removing last element_<br>
 ![DS](/images/logical-ds/queue/2_2_array-circular_deque.PNG) <br>
**_Algorithm_**
```
DeQueue()
  if queue==empty(call isEmpty method) -- O(1)
    return errorMessage ----------------- O(1)
  else   -------------------------------- O(1)
	tempVal=arr[start] -------------- O(1)	
	//queue has just 1 value
	if start==end ------------------- O(1)	
		start=end=-1 ------------ O(1)	
	//dequeue last index value
	else if start=arr.lenth-1 ------- O(1)
		start=0 ----------------- O(1)
	else ---------------------------- O(1)
		start=start+1 ----------- O(1)	
	//Assigning value
    	return tempVal------------------- O(1)	
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>

### isEmpty 
**_Algorithm_**
```
isEmpty()
  if start ==-1  ------------ O(1)
    return true ------------- O(1)
  else   
    return false ------------ O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### isFull 
![DS](/images/logical-ds/queue/2_3_array-circular_isFull.PNG) <br> 
**_Algorithm_**
```
isFull()
 isFull = false ------------------------ O(1)
 if endPos+1 == startPos --------------- O(1)
    isFull = true ---------------------- O(1)
 else if (start=0 and end=arr.size-1) -- O(1)
    isFull = true ---------------------- O(1) 
 return isFull ------------------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
## Queue -Linear (Linked List)
### Time and Space complexity table
![time-complexity-table](/images/logical-ds/queue/3_linked-list_linear_queue_time-and-space_complexity.PNG) <br>
### CreateQueue
![create](/images/logical-ds/queue/1_1_array_linear_cereate-queue.PNG) <br>
**_Algorithm_**
```
CreateQueue()
  create blank linked list - O(1)
  head= null --------------- O(1)
  tail= null --------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### EnQueue
  _addling value to queue_<br>
![enqueue](/images/logical-ds/queue/1_2_array_linear_enque.PNG) <br>
**_Algorithm_**
```
EnQueue(value)
  create new node (newNode) -------------- O(1)
  newNode.value = value ------------------ O(1)
  newNode.next = null -------------------- O(1)
  if queue==empty (call isEmpty method) -- O(1)
    head = tail =newNode ----------------- O(1)
  else   --------------------------------- O(1)
    tail.next = newNode ------------------ O(1)
    tail=newNode ------------------------- O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### DeQueue
  _returning and removing last element_<br>
![dequeue](/images/logical-ds/queue/1_3_array_linear_deque.PNG) <br>
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
    return head.value -- O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### isEmpty 
**_Algorithm_**
```
isEmpty()
  if head ==null  -- O(1)
    return true  --- O(1)
  else   
    return false --- O(1)    
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### isFull 

**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### deleteQueue 
**_Algorithm_**
```
deleteQueue()
 head=tail=null
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>

