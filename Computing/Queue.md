---
date: 2022-10-24
type: 🧠
tags:
  - MAC/3/ED
---

**Topics:** [[Data Structure]]

---

A _queue_ is [[Linear Data Structure|linear data structure]] in which we operate through its two ends. We insert elements through one end and delete them through the other.

The first element in a queue is the first one that's going out. This is why queues are also known as _FIFO_-type structures (first in, first out).

Like [[List|lists]] and [[Stack|stacks]], queues can be contiguous or linked. Queues have two special fields: a _head_ field and a _tail_ field:

| Head | …   | Tail |
| ---- | --- | ---- |

Stacks have the following operations:

1. Iteration through the stack
2. Element insertion (_push_)
3. Element deletion (_pop_)
4. Element search

# Biqueue

_Biqueues_ are a special type of queues from which we can insert/delete elements through *both *the head _or_ the tail.

There are two types of biqueues:

1. **Restricted entry biqueue:** this biqueue allows deletions to be carried out from any of its two ends, but insertions can only be carried out from the tail
2. **Restricted exit biqueue:** this biqueue allows insertions from any of its two ends, but deletions can only be carried out from the tail
# Priority Queue

A _priority queue_ is a special type of queue in which every element has an integer attached to it to indicate its processing priority.

The way in which a given element is inserted or deleted is:

1. The element with the highest priority is the first one processed
2. Two elements with the same priority are processed according to the order in which they were inserted to the queue
3. The lower the _priority integer_, the higher the proirity.
