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
* [single linked list](#single-linked-ist)
* [circular linked list](#circular-linked-list)
* [double linked list](#double-linked-list)
* [circular double liked list](#circular-double-liked-list)<br>
**single linked list**<br>
  In a singly linked list each node in the list stores the data of the node and a reference to the next node in the list,it doesn't store any reference to previous node<br>
![DS](/images/linked-list/2_0_singly_linked-list.PNG) <br> <br>
**circular linked list**<br>
  only change is last node in the list holds reference to first node(instead of null)<br>
![DS](/images/linked-list/2_1_circuler_singly_linked-list.PNG) <br> <br>
**double linked list**<br>
  In a double linked list each node consists of two reference, reference to previous node and reference to next node.<br>
![DS](/images/linked-list/3_0_double_linked-list.PNG) <br> <br>
**circular double liked list**<br>
  only change is last node in the list holds reference to first node(instead of null)<br>
![DS](/images/linked-list/3_1_circular_double_linked-list.PNG) <br> <br>

## single linked 
* [single linked list time and space complexity table](#single-linked-list-time-and-space-complexity-table)
* [single linked list creation](#single-linked-list-creation)
* [single linked list insert](#single-linked-list-insert)
* [single linked list traverse](#single-linked-list-traverse)
* [single linked list search](#single-linked-list-search)
* [single linked list delete node](#single-linked-list-delete-node)
* [single linked list delete entire list](#single-linked-list-delete-entire-list)
	
### single linked list time and space complexity table 
![DS](/images/linked-list/2_0_7_singly_linked-list_complexity_table.PNG) <br> <br>
### single linked list creation 
![DS](/images/linked-list/2_0_1_singly_linked-list_creation_complexity.PNG) <br> <br>
### single linked list insert 
![DS](/images/linked-list/2_0_2_singly_linked-list_node-insertion_complexity.PNG) <br> <br>
### single linked list traverse 
![DS](/images/linked-list/2_0_3_singly_linked-list_traverse_complexity.PNG) <br> <br>
### single linked list search 
![DS](/images/linked-list/2_0_4_singly_linked-list_search_complexity.PNG) <br> <br>
### single linked list delete node 
![DS](/images/linked-list/2_0_5_singly_linked-list_delete-node_complexity.PNG) <br> <br>
### single linked list delete entire list 
![DS](/images/linked-list/2_0_6_singly_linked-list_delete-entire_list_complexity.PNG) <br> <br>
