# Binary Tree
## Tree Properties
	* Used to represent data in hierarchical form
	* Every Node(ideally) has 2 components (Data & Reference)
	* It has a root node and 2 disjoint binary tree called Left subtree and Right subtree

## Tree Terminologies
* [Root](#)<br> 
	Node with no parents<br> 
* [Edge](#)<br> 
	Link from parent to child <br> 
* [Leaf](#)<br> 
	Node with no children <br>
* [Sibling](#)<br> 	
	Children of same parent<br> 
* [Ancestor](#)<br> 
	 means parent,grant-parent,great grant-parent, and so on for the given node<br> 	
	![root_edge_leaf_sibilings_ancester](/images/logical-ds/binary-tree/1_tree-teriminologies_root_edge_leaf_sibilings_ancester.PNG) <br>
* [Depth of Node](#)<br> 
	Length of path from root node(ie no of edges)<br>
* [Hight of Node](#)<br> 
	 Length of path from node to the deepest node<br>
* [Hight of Tree](#)<br> 
	Same as hight of root node <br> 
* [Depth of Tree](#)<br> 
	 Same as Depth of root node which will be always 0<br> 
	![height_depth](/images/logical-ds/binary-tree/1_tree-teriminologies_height_depth.PNG) <br>
* [Predecessor](#)<br> 
	Predecessor of the node is the immediate previous node in inorder traversal of a binary tree.<br> 
	![predecessor](/images/logical-ds/binary-tree/1_10_tree-teriminologies_predecessor.PNG) <br>
* [Successor](#)<br> 
	Successor of the node is the immediate next node in inorder traversal of a binary tree.<br> 
	![successor](/images/logical-ds/binary-tree/1_11_tree-teriminologies_successor.PNG) <br>

## What is Binary Tree
* Tree in which each node can have up to two children(0 or 1 or 2),but not more than two.
* BST,Heap Tree,AVL are type of binary tree <br>
![binary-tree](/images/logical-ds/binary-tree/binary-tree.PNG) <br>

## Why is Binary Tree
* Prerequisite for more advanced trees(BST,AVL,Red-Black)
* Is used in solving problems like
	* Huffman coding
	* Heap(Priority queue)
	* Expression parsing
## Types of Binary Tree
![binary-tree_types](/images/logical-ds/binary-tree/binary-tree_types.PNG) <br>

## Operations on Binary Tree
* [Creation of Tree](#)
* [Insertion of Node]
* [Deletion of Node]
* [Traverse all nodes](#)
        * [Depth First](#)
		* [Preorder Traversal](#preorder-traversal)
		* [Inorder Traversal](#inorder-traversal)
		* [Postorder Traversal](#postorder-traversal)
	* [Breadh First](#)
		* [Level Order Traversal](#level-order-traversal)
* [Search]
* [Deletion of Tree](#)

## Preorder Traversal
![preorder-traversal](/images/logical-ds/binary-tree/2_1_1_binary-tree_preorder-traversal.PNG) <br>
![preorder-traversal](/images/logical-ds/binary-tree/2_1_2_binary-tree_preorder-traversal-algo.PNG) <br>
## Inorder Traversal
![inorder-traversal](/images/logical-ds/binary-tree/2_2_1_binary-tree_inorder-traversal.PNG) <br>
![inorder-traversal](/images/logical-ds/binary-tree/2_2_2_binary-tree_inorder-traversal-algo.PNG) <br>
## Postorder Traversal
![postorder-traversal](/images/logical-ds/binary-tree/2_3_1_binary-tree_postorder-traversal.PNG) <br>
![postorder-traversal](/images/logical-ds/binary-tree/2_3_2_binary-tree_postorder-traversal_algo.PNG) <br>
## Level Order Traversal
![levelorder-traversal](/images/logical-ds/binary-tree/2_4_1_binary-tree_levelorder-traversal.PNG) <br>
![levelorder-traversal](/images/logical-ds/binary-tree/2_4_2_binary-tree_levelorder-traversal_1.PNG) <br>
![levelorder-traversal](/images/logical-ds/binary-tree/2_4_3_binary-tree_levelorder-traversal_algo.PNG) <br>

		
	
	
