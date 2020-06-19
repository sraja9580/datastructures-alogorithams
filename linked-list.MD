# Linked List
A inked list is a linear data structure where each element is a separate object.Each element(node) of list comprises of tow items - the data and reference to the next node.The most powerful feature of Linked List is that it is of variable size.<br> <br>
We can compare linked list to a train,each node to a compartment, even if we remove comportment(node) train(linked list)  will still work.
Train always starts with engine and ends with guard room,same ways Liked list always starts with head and ends with tail.<br> <br>
![DS](/images/linked-list/1_linked-list.PNG) <br> <br>
**Node** Contains Data and Reference to next Node  <br>
**Head** Reference to first Node in the list. <br>
**Tail** Reference to last node of the list. <br> <br>
## How Linked List Stored in RAM
![DS](/images/linked-list/1_1_linked-list_RAM.PNG) <br> <br>
## Types of Linked List
* [Single Linked List](#single-linked-list)
* [Circular Single Linked List](#circular-linked-list)
* [Double Linked List](#double-linked-list)
* [Circular Double Liked List](#circular-double-liked-list)<br><br>
**Single Linked List**<br>
  In a singly linked list each node in the list stores the data of the node and a reference to the next node in the list,it doesn't store any reference to previous node<br>
![DS](/images/linked-list/2_0_singly_linked-list.PNG) <br> <br>
**Circular Single Linked List**<br>
  only change is last node in the list holds reference to first node(instead of null)<br>
![DS](/images/linked-list/2_1_circuler_singly_linked-list.PNG) <br> <br>
**Double Linked List**<br>
  In a double linked list each node consists of two reference, reference to previous node and reference to next node.<br>
![DS](/images/linked-list/3_0_double_linked-list.PNG) <br> <br>
**Circular Double Liked List**<br>
  only change is last node in the list holds reference to first node(instead of null)<br>
![DS](/images/linked-list/3_1_circular_double_linked-list.PNG) <br> <br>

## Single Linked List
* [Single Linked List Time and Space Complexity Table](#single-linked-list-time-and-space-complexity-table)
* [Single Linked List Creation](#single-linked-list-creation)
* [Single Linked list Insert](#single-linked-list-insert)
* [Single Linked List Traverse](#single-linked-list-traverse)
* [Single Linked List Search](#single-linked-list-search)
* [Single Linked List Delete Node](#single-linked-list-delete-node)
* [Single Linked List Delete Entire List](#single-linked-list-delete-entire-list)
	
### Single Linked List Time and Space Complexity Table 
![DS](/images/linked-list/2_0_7_singly_linked-list_complexity_table.PNG) <br> <br>
### Single Linked List Creation 
![DS](/images/linked-list/2_0_1_singly_linked-list_creation_complexity.PNG) <br> <br>
### Single Linked List Insert 
![DS](/images/linked-list/2_0_2_singly_linked-list_node-insertion_complexity.PNG) <br> <br>
### Single Linked List Traverse 
![DS](/images/linked-list/2_0_3_singly_linked-list_traverse_complexity.PNG) <br> <br>
### Single Linked List Search 
![DS](/images/linked-list/2_0_4_singly_linked-list_search_complexity.PNG) <br> <br>
### Single Linked List Delete Node 
![DS](/images/linked-list/2_0_5_singly_linked-list_delete-node_complexity.PNG) <br> <br>
### Single Linked List Delete Entire List 
![DS](/images/linked-list/2_0_6_singly_linked-list_delete-entire_list_complexity.PNG) <br> <br>

## Circular single linked 
* [Circular single linked list time and space complexity table](#circular-single-linked-list-time-and-space-complexity-table)
* [Circular single linked list creation](#circular-single-linked-list-creation)
* [Circular single linked list insert](#circular-single-linked-list-insert)
* [Circular single linked list traverse](#circular-single-linked-list-traverse)
* [Circular single linked list search](#circular-single-linked-list-search)
* [Circular single linked list delete node](#circular-single-linked-list-delete-node)
* [Circular single linked list delete entire list](#circular-single-linked-list-delete-entire-list)
	
### Circular single linked list time and space complexity table 
---
![DS](/images/linked-list/2_1_7_circuler_singly_linked-list_complexity_table.PNG) <br> <br>
### Circular single linked list creation 
![DS](/images/linked-list/2_1_1_circuler_singly_linked-list_create.PNG) <br> <br>
### Circular single linked list insert 
**Insert in postion 0**<br>
![DS](/images/linked-list/2_0_2_1_singly_linked-list_node-insert-first_complexity.PNG) <br> <br>
**Insert in last position**<br>
![DS](/images/linked-list/2_0_2_2_singly_linked-list_node-insert-last_complexity.PNG) <br> <br>
```
insertInCLL(head,nodeValue,position)
	create new blank node(node)------------------------------------O(1)
	node.value=nodeValue-------------------------------------------O(1)
	
	if(position==0)------------------------------------------------O(1)
		node.next=head-----------------------------------------O(1)
		head=node----------------------------------------------O(1)
		//pointing last node to new first node
		tail.next=node-----------------------------------------O(1)
	else if(pointing==last)
		//pointing new last node to first node
		node.next=head-----------------------------------------O(1)
		//pointing previous last node to current last node
		tail.next=node-----------------------------------------O(1)
		tail=node----------------------------------------------O(1)
	else (any other position)--------------------------------------O(1)
		//getting previous node of the position
		loop to position-1-------------------------------------O(n)
		    tempNode=position-1-Node---------------------------O(1)
		node.next=tempNode.next--------------------------------O(1)
		tempNode.next=node-------------------------------------O(1)
```
**Time Complexity  -O(n)** <br>
**Space Complexity -O(1)** <br> <br>
### Circular single linked list traverse 
![DS](/images/linked-list/2_1_3_circuler_singly_linked-list_traverse.PNG) <br> <br>
### Circular single linked list search 
![DS](/images/linked-list/2_1_4_circuler_singly_linked-list_search.PNG) <br> <br>
### Circular single linked list delete node 
**delete first node**<br>
![DS](/images/linked-list/2_1_5_1_circuler_singly_linked-list_delete_first_node.PNG) <br> <br>
**delete last node**<br>
![DS](/images/linked-list/2_1_5_2_circuler_singly_linked-list_delete_last_node.PNG) <br> <br>
**delete any other node**<br>
![DS](/images/linked-list/2_1_5_3_circuler_singly_linked-list_delete_n-position_node.PNG) <br> <br>
![DS](/images/linked-list/2_1_5_circuler_singly_linked-list_delete_node.PNG) <br> <br>
### Circular single linked list delete entire list 
tail.next points to last nodes address cell<br>
so tail.next=NULL removes last elemnts link to first element <br>
![DS](/images/linked-list/2_1_6_circuler_singly_linked-list_delete-entire-list.PNG) <br> <br>

## Double Linked List
* [Double Linked List Time and Space Complexity Table](#double-linked-list-time-and-space-complexity-table)
* [Double Linked List Creation](#double-linked-list-creation)
* [Double Linked list Insert](#double-linked-list-insert)
* [Double Linked List Traverse](#double-linked-list-traverse)
* [Double Linked List Search](#double-linked-list-search)
* [Double Linked List Delete Node](#double-linked-list-delete-node)
* [Double Linked List Delete Entire List](#double-linked-list-delete-entire-list)
	
### Double Linked List Time and Space Complexity Table 
![DS](/images/linked-list/3_0_6_DLL_time-space-complexity_table.PNG) <br> <br>
### Double Linked List Creation 
![DS](/images/linked-list/3_0_1_double_linked-list_creation.PNG) <br> <br>
```
createDLL(nodeValue)
	create new blank node(node)----O(1)
	node.value=nodeValue-----------O(1)
	head=node----------------------O(1)
	tail=node----------------------O(1)
	node.next=null-----------------O(1)
	node.prev-null-----------------O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### Double Linked List Insert 
**Insert in postion 0**<br>
![DS](/images/linked-list/3_0_4_1_DLL_insert-node-first.PNG) <br> <br>
**Insert in last position**<br>
![DS](/images/linked-list/3_0_4_2_DLL_insert-node-last.PNG) <br> <br>
**Insert in any other position**<br>
![DS](/images/linked-list/3_0_4_3_DLL_insert-node-n-position.PNG) <br> <br>
```
insertNodeInDLL(head,nodeValue,position)
	create new blank node(node)---------------------O(1)
	node.value=nodeValue----------------------------O(1)
	if(position==0)---------------------------------O(1)
		node.next=head--------------------------O(1)
		node.prev=null--------------------------O(1)
		node.next.prev(head.prev)=node----------O(1)
		head=node-------------------------------O(1)
	else if(pointing==last)-------------------------O(1)
		node.next=null--------------------------O(1)
		node.prev=tail--------------------------O(1)
		node.prev.next(tail.next)=node----------O(1)
		tail=node-------------------------------O(1)
	else (any other position)-----------------------O(1)
		loop:tempNode=node(position-1)----------O(n)
		node.prev=tempNode----------------------O(1)
		node.next=tempNode.next-----------------O(1)
		tempNode.next=node----------------------O(1)
		node.next.prev=node---------------------O(1)
```
**Time Complexity  -O(n)  Space Complexity -O(1)** <br> <br>

### Double Linked List Traverse 
**Traverse Forward** <br>
![DS](/images/linked-list/3_0_2_1_DLL_traverse_forward.PNG) <br> <br>
**Traverse Backword** <br>
![DS](/images/linked-list/3_0_2_2_DLL_traverse_reverse.PNG) <br> <br>
### Double Linked List Search 
![DS](/images/linked-list/3_0_3_DLL_search.PNG) <br> <br>
### Double Linked List Delete Node 
**delete first node**<br>
![DS](/images/linked-list/3_0_7_1_DLL_delete-node-first.PNG) <br> <br>
**delete last node**<br>
![DS](/images/linked-list/3_0_7_2_DLL_delete-node-last.PNG) <br> <br>
**delete any other node**<br>
![DS](/images/linked-list/3_0_7_3_DLL_delete-node-n-position.PNG) <br>
```
deleteNodeInDLL(head,position)	
	if(position==0)-----------------------------O(1)
		//if size==1 head=tail=null		
		head=head.next--------------------------O(1)
		head.prev=null--------------------------O(1)		
	else if(pointing==last)---------------------O(1)
		//if size==1 head=tail=null		
		tail=tail.prev--------------------------O(1)
		tail.next=null--------------------------O(1)
	else (any other position)-------------------O(1)
		loop:tempNode=node(position-1)----------O(n)
		tempNode.next=tempNode.next.next--------O(1)
		tempNode.next.prev=tempNode-------------O(1)	
```
**Time Complexity  -O(n)  Space Complexity -O(1)** <br> <br>
### Double Linked List Delete Entire List 
![DS](/images/linked-list/3_0_5_DLL_delete-entire-list.PNG) <br> <br>
		
## Circular Double Linked List
* [Circular Double Linked List Time and Space Complexity Table](#circular-double-linked-list-time-and-space-complexity-table)
* [Circular Double Linked List Creation](#circular-double-linked-list-creation)
* [Circular Double Linked list Insert](#circular-double-linked-list-insert)
* [Circular Double Linked List Traverse](#circular-double-linked-list-traverse)
* [Circular Double Linked List Search](#circular-double-linked-list-search)
* [Circular Double Linked List Delete Node](#circular-double-linked-list-delete-node)
* [Circular Double Linked List Delete Entire List](#circular-double-linked-list-delete-entire-list)
	
### Circular Double Linked List Time and Space Complexity Table 
![DS](/images/linked-list/3_1_7_CDLL_time-space-complexity_table.PNG) <br> <br>
### Circular Double Linked List Creation 
![DS](/images/linked-list/3_1_1_CDLL_creation.PNG) <br>
```
createCDLL(nodeValue)
	create new blank node(node)----O(1)
	node.value=nodeValue-----------O(1)
	head=node----------------------O(1)
	tail=node----------------------O(1)
	node.next=node-----------------O(1)
	node.prev=node-----------------O(1)
```
**Time Complexity  -O(1)  Space Complexity -O(1)** <br> <br>
### Circular Double Linked List Insert 
**Insert in postion 0**<br>
![DS](/images/linked-list/3_0_4_1_DLL_insert-node-first.PNG) <br> <br>
**Insert in last position**<br>
![DS](/images/linked-list/3_0_4_2_DLL_insert-node-last.PNG) <br> <br>
**Insert in any other position**<br>
![DS](/images/linked-list/3_0_4_3_DLL_insert-node-n-position.PNG) <br> <br>
```
insertInCDLL(head,nodeValue,position)
	create new blank node(node)------------------------------------O(1)
	node.value=nodeValue-------------------------------------------O(1)
	
	if(position==0)------------------------------------------------O(1)
		node.next=head-----------------------------------------O(1)
		node.prev=tail-----------------------------------------O(1)
		tail.next=node-----------------------------------------O(1)
		head.prev=node-----------------------------------------O(1)
		head=node----------------------------------------------O(1)
	else if(pointing==last)
		node.next=head-----------------------------------------O(1)
		node.prev=tail-----------------------------------------O(1)
		tail.next=node-----------------------------------------O(1)
		head.prev=node-----------------------------------------O(1)
		tail=node----------------------------------------------O(1)
	else (any other position)--------------------------------------O(1)
		//getting previous node of the position
		loop to position-1-------------------------------------O(n)
		    tempNode=position-1-Node---------------------------O(1)
		node.next=tempNode.next--------------------------------O(1)
		node.prev=tempNode-------------------------------------O(1)
		tempNode.next=node-------------------------------------O(1)
		node.next.prev=node------------------------------------O(1)
```
**Time Complexity  -O(n)  Space Complexity -O(1)** <br> <br>

### Circular Double Linked List Traverse 
**Traverse Forward** <br>
![DS](/images/linked-list/3_1_3_1_CDLL_traverse_forward.PNG) <br> <br>
**Traverse Backword** <br>
![DS](/images/linked-list/3_1_3_2_CDLL_traverse_reverse.PNG) <br> <br>
### Circular Double Linked List Search 
![DS](/images/linked-list/3_1_3_4_CDLL_search.PNG) <br> <br>
### Circular Double Linked List Delete Node 
**delete first node**<br>
![DS](/images/linked-list/3_0_7_1_DLL_delete-node-first.PNG) <br> <br>
**delete last node**<br>
![DS](/images/linked-list/3_0_7_2_DLL_delete-node-last.PNG) <br> <br>
**delete any other node**<br>
![DS](/images/linked-list/3_0_7_3_DLL_delete-node-n-position.PNG) <br>
```
deleteNodeInDLL(head,position)	
	if(position==0)-----------------------------O(1)
		//if size==1 head=tail=null		
		head=head.next--------------------------O(1)
		head.prev=null--------------------------O(1)		
	else if(pointing==last)---------------------O(1)
		//if size==1 head=tail=null		
		tail=tail.prev--------------------------O(1)
		tail.next=null--------------------------O(1)
	else (any other position)-------------------O(1)
		loop:tempNode=node(position-1)----------O(n)
		tempNode.next=tempNode.next.next--------O(1)
		tempNode.next.prev=tempNode-------------O(1)	
```
**Time Complexity  -O(n)  Space Complexity -O(1)** <br> <br>
### Circular Double Linked List Delete Entire List 
![DS](/images/linked-list/3_1_6_1_CDLL_delete-entire-list.PNG) <br>
![DS](/images/linked-list/3_1_6_2_CDLL_delete-entire-list.PNG) <br>
