#SPLAY TREE
## JAVA CODE


Splay Tree is a self-adjusting BST (Binary Search Tree), it follows the 
same principles. They are also balanced trees and use rotations to get 
balanced. Unlike AVL trees they are not completely balanced which is 
good feature of these trees as it is easier to search for recent items 
in this tree.  This data structure is widely in building caches where 
you need to access the recently used items.

**Worst Case: O (logn).**

#Problems with Binary Search Tree 
1. Not a balance tree 
2. Worst Case is O (n) (when data entered is already sorted) 
3. A lot of time to access recent inserted / searched element 

#Solution: AVL Tree 
1. A balance binary tree 
2. Worst case is O (log n)
3. Multiple Rotations (Left, Right, Left Right and Right Left rotation)

#Problems with AVL Tree 
1. Extra storage for height field in each node. 
2. Calculation of Balance Factor can be sometime difficult 
3. Ugly deletion of AVL Tree (around 12 different cases) 
4. A lot of time to access recent inserted / searched element. 

#Solution: Splay Trees
1. Deletion was made simple 
2. Recently inserted / searched element always be on root of the tree

#Searching in Splay Trees: 
Searching in Splay trees is quite similar to the BST tree except for one 
thing. If the search is successful, then the node that is found is 
splayed and becomes the new root. Else the last node accessed prior to 
reaching the NULL is splayed and becomes the new root.

#Insertion in Splay Trees:
Every insertion splays the tree based on the new value and then assigns 
that new value to the root.  Every tree node will have a left child node 
and right child node which maybe empty depending on the current tree 
order. Inserted elements will be inserted here and then splayed.

#Deletion in Splay Trees:
Deleting a node in splay tree will splay the tree such that the maximum 
key that is less than the removed key will now be the root. If a key 
chosen for removal does not exist, the tree will splay around the 
closest value to that key.

