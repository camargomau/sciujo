---
date: 2022-10-10
type: 🧠
tags:
  - MAC/3/ED
---

**Topics:** [[Data Structure]] - [[List]]

---

A _doubly linked list_ is a type of [[List|list]]. It's very similar to a [[Simple Linked List|simple linked list]], the only difference being the fact that each node is composed of three (instead of two) fields:

- Previous link: contains the pointer to the previous element
- Information: contains the element of the list in the node
- Next link: contains the pointer to the next element

Visually, one of these nodes can be seen as follows:

| Previous | Information | Next |
| -------- | ----------- | ---- |

In its `Previous` field, the first node has a pointer that points to nothing. In its `Next` field, the last node has a pointer that points to nothing.

Just like in a simple linked list, it's necessary to have a pointer variable that points to the first element of the list.
