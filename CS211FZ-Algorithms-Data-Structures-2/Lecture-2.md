
## Importance of BST(Binary Search Tree)

- Most of the primitive operations on search trees run in $O(h)$ time on a tree of height $h$
- The average height of a node in a binary search tree on $N$ node is $O(\lg{N})$  
- Given $N$ elements to be inserted in a binary search tree, the height of the tree depends on the order of the elements inserted
	- E.g., given the set of nodes with their key values from 1 – 7, 
		- if the insertion order is {1, 2, 3, 4, 5, 6, 7}, the depth of the tree will be 6  
		- If the insertion order is { 4, 2, 5, 1, 3, 6, 7}, the depth of the tree will be 2  
- Deletion of nodes may result in an unbalanced tree

## AVL

### Feature of AVL

- An AVL (Adelson-Velsky and Landis) tree is a self-balancing binary search tree
- For every node in the tree, the height of the left and right subtree can differ by at most one



### Summary

- 在AVL树中，对于树中的每个节点，左右子树的高度最多相差一个，即高度平衡。
- 待删除的节点可以标记为已删除，因此不需要重新平衡(rebalancing)
- 搜索、插入和删除在平均情况和最坏情况下都需要 $O(\log_{2}{N})$ 时间
- 在某些情况下，AVL 树可能会偏重，导致性能相对较差

## Red-Black Tree

- 红黑树是AVL树的替代品，因此红黑树也是一种自平衡二叉搜索树
- 红黑树上的操作在最坏情况下需要$O(\lg{N})$时间，并且高度为红黑树最多为$2\lg{(N+1)}$ 
- 红黑树中的每个节点都需要一个额外的位来存储节点的颜色，可以是红色或黑色
- 红黑树确保没有路径从根到叶的长度是其他长度的两倍以上，因此树是近似平衡的





- A red-black tree is self-balancing binary search tree  
	红黑树是自平衡二叉搜索树
- One extra bit is needed for each node to store the colour of the node  
	每个节点需要一个额外的位来存储节点的颜色
- A node can only be coloured either red or black  
	节点只能着色为红色或黑色
- Red-black trees have relatively low overhead for insertion  
	红黑树的插入开销相对较低
- In practice, rotations occur relatively infrequently compared to AVL trees  
	在实践中，与 AVL 树相比，旋转发生的频率相对较低
- Using red-black trees can avoid side-overweighted subtrees  
	使用红黑树可以避免边权重过大的子树
