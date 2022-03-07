## Objectives
- to know the concepts, terminologies(术语) and mathematical properties of trees
- to be able to describe the differences between various types of trees and their implementations
- to be able to analyze the performance(性能) of operations on trees
- to know how trees are used in real-world applications

## Properties of Trees

A tree or free tree is a connected, acyclic, undirected graph. 树或自由树是一个连通的、无环路的无向图。

- 𝑮 中的任何两个顶点都通过唯一的简单路径连接。
- 𝑮 是连接的，但是如果从 E（树中的一组边）中删除任何边，则结果图是不连接的。
- 𝑮 是连通的，并且|𝑬| = |𝑽| - 𝟏。
- 𝑮 是无环的，并且|𝑬| = |𝑽| - 𝟏。
- 𝑮 是非循环的，但如果将任何边添加到 E，则生成的图包含一个循环。

## Terminologies

- 根节点 root node
- 叶节点 leaf node / 外节点 External node
- 内节点 internal node
- 深度 Depth 描述的是节点的深度，查询时需要的次数
- 高度 Height 描述的是整个树的高度，即最多的查询次数
- Degree 用于描述某个节点拥有的子节点的数量，叶节点的 degree 为 0
- Ancestor (祖先) 查询某个节点时经过的所有节点都是这个节点的 Ancestor
- Descendant 与 Ancestor 对应，节点 x 为节点 y 的 Ancestor，则节点 y 为节点 x 的 Descendant，描述的是从某个节点可以抵达的所有节点
- 我们称所有的节点都为其自身的 Ancestor 和 Descendant，所以不为其自身的 Ancestor 和 Descendant 我们称为 proper Ancestor 以及 proper Descendant，即真祖先节点与真后代节点。
- The root is the only node without a parent. 根节点没有父节点
- 父子节点就是在同一条 edge 上的祖先节点与后代节点
- 如果节点具有相同的父节点，则它们是同辈节点 (siblings)。
- 以节点为根的子树 (subtree) 是由该节点的后代引出的以该节点为根的树。

## Other Type Trees

### Binary Tree 二分树

二叉树是在有限节点集上定义的结构，这些节点要么不包含节点，要么由三个不相交的节点集组成：根节点、称为左子树的二叉树和称为右子树的二叉树。因为二分树的子树可能不包含节点，我们称为 Empty Tree or Null Tree `NIL`，并且 child is absent or missing，即子节点缺失。而没有空节点的二分树称为 Full Binary Tree

> some full binary trees are complete 2-ary trees，所谓的 k-ary tree 就是所有叶子都具有相同的深度，并且所有内部节点的度数为𝒌 的树结构。
> k-ary tree 的节点数量为 1 + 𝑘 + 𝑘! + …+ 𝑘", n 为树的高度(Height)

个人理解来说，二分树就是每个节点只会存在两个子节点的树结构。这样的约束给予了二分树一些特殊的性质。

### Binary Search Tree 二分查找树 BST

二分查找树，就是在二分树的基础上再约定了，每个节点的子节点中，左子节点大于右子节点。

## Operation

### BST Operations - Tree Traversal BST树遍历

- Depth-first Search (DFS) 深度优先查找
	- In-order 
		- Prints the root of a subtree between printing the values in its left subtree and printing those in its right subtree.
	- Pre-order 
		- Prints the roots before the values in either subtree.
	- Post-order 
		- Prints the root after the values in its subtrees.
- Breadth-first Search (BFS) 广度优先算法
	- Prints all the keys in order on the current level before moving to the next depth (aka, level-order search)

