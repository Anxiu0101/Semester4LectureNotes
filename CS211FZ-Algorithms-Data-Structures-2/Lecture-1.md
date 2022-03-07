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