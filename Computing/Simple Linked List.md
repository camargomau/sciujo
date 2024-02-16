---
type: 🧠
date: 2022-10-10
tags:
  - MAC/S3/ED
---

**Topics:** [[List]] - [[Data Structure]]

---

A _simple linked list_ is a type of [[List|list]]. It consists of a collection of elements called _nodes_. The orden between them is established through pointers. Each node is composed of two fields:

- Information: contains the element of the list in the node
- Link: contains the pointer to the next element

Visually, a node can be seen as follows:

| Information | Link |
| ----------- | ---- |

Notice that, since it's necessary to know the location of the first element of the list, it's also necessary to have a pointer variable that points to the first element.

The last node has a pointer that points to nothing.
