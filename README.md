# BTree-Header-File

B Tree is a specialized m-way tree that can be widely used for disk access. A B-Tree of order m can have at most m-1 keys and m children. One of the main reason of using B tree is its capability to store large number of keys in a single node and large key values by keeping the height of the tree relatively small.

A B tree of order m contains all the properties of an M way tree. In addition, it contains the following properties.

* Every node in a B-Tree contains at most m children.
* Every node in a B-Tree except the root node and the leaf node contain at least m/2 children.
* The root nodes must have at least 2 nodes.
* All leaf nodes must be at the same level.

B-Tree is a self-balancing search tree. In most of the other self-balancing search trees (like AVL and Red-Black Trees), it is assumed that everything is in main memory. To understand the use of B-Trees, we must think of the huge amount of data that cannot fit in main memory. When the number of keys is high, the data is read from disk in the form of blocks. Disk access time is very high compared to the main memory access time. The main idea of using B-Trees is to reduce the number of disk accesses. Most of the tree operations (search, insert, delete, max, min, ..etc ) require O(h) disk accesses where h is the height of the tree. B-tree is a fat tree. The height of B-Trees is kept low by putting maximum possible keys in a B-Tree node. Generally, the B-Tree node size is kept equal to the disk block size. Since the height of the B-tree is low so total disk accesses for most of the operations are reduced significantly compared to balanced Binary Search Trees like AVL Tree, Red-Black Tree, ..etc.

References :
* B Tree : https://www.geeksforgeeks.org/introduction-of-b-tree-2/
* Insertion in B Tree : https://www.geeksforgeeks.org/insert-operation-in-b-tree/
* Deletion in B Tree : https://www.geeksforgeeks.org/delete-operation-in-b-tree/
