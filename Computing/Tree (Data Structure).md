---
date: 2022-10-26
type: 🧠
tags:
  - MAC/3/ED
---

**Topics:** [[Data Structure]]

---

A _tree_ is a [[Non-linear Data Structure|non-linear]] and dynamic data structure. It's dynamic since its structure can change during the execution of a program, and it's non-linear since each of its elements can be followed by more than one element.

> [!info]- Other definitions
> A tree can also be called a _hierarchical data_ structure that contains a collection of elements called _nodes_, one of them known as _root_. Between all of these elements, _parent-child_ relations are established.
>
> At the same time, trees are homogeneous structures defined by the concatenation of one node element along with a finite number of disjoint trees called _sub-trees_.

As with [[List|lists]], [[Stack|stacks]] and [[Queue|queues]], trees can be contiguous (which use arrays) or linked (which use pointers). Despite that, trees are commonly linked since they are a dynamic data structure.

A [[Binary Tree|binary tree]] is a special type of tree that is used to save up memory and space, since trees that contain nodes each with a different number of offspring can waste a lot of memory and space.

# Graphical representation

Graphically, trees can be seen as a [[Graph|graph]] with the following features:

1. Every non-empty tree has one and only one _root node_
2. Loops can't exist
3. The number if lines is always $n-1$, where $n$ is the number of elements in the tree
4. A node $X$ is a _direct child_ of a node $Y$ if $X$ is being pointed to by $Y$
5. A node $X$ is a _direct parent_ of a node $Y$ if $X$ points to $Y$
6. Every node that has no children is called a _terminal_ or _leaf_
7. Every node that isn't the root node nor a terminal node is known as an _interior node_
8. The _degree_ of a node is the number of direct offspring of a node. The degree of the tree is the maximum degree among all the node degrees
9. The _level_ is the amount of links that have to be traversed to reach a certain node plus one. By definition, the root node has a level of 1
10. The _height_ of a tree is the maximum number of levels among all the levels within the tree
