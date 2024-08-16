---
type: 🧠
date: 2022-10-26
tags:
  - MAC/3/ED
---

**Topics:** [[Tree (Data Structure)]] - [[Data Structure]]

---

A _binary tree_ is a [[Tree (Data Structure)|tree]] in which every node can have 0, 1 or 2 children nodes. It's used to save up memory and space, since other kind of trees can waste a lot of memory and space.

Formally, it's defined as a homogeneous structure that's the concatenation of a root node with two disjoint binary trees (called left sub-tree and right sub-tree).

# Converting a Non-Binary Tree to a Binary Tree

To convert a tree that's non-binary to one that's binary, we can use the following process:

1. Link horizontally the offspring of each node (i.e. link the siblings)
2. Link vertically the parent node with the leftmost child, then delete the link between that parent and the rest of its offspring
3. Rotate the corresponding diagram by 45°

The links to the left of a node represent parent-child relationships, while the links to the right represent sibling relationships.

# Memory representation

A binary tree can be represented in memory as a register that contains three fields:

1. The link to a children node (left link)
2. Information in the node
3. The link to a sibling node (right link)

| Left link | Info | Right link |
| --------- | ---- | ---------- |
