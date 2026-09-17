# README.md

## Data Structures Notebook

This notebook provides implementations of fundamental data structures, specifically a Singly Linked List and a Doubly Linked List, in Python.

### Contents

1.  **Linked List**: A basic implementation of a singly linked list with common operations like append, prepend, insert, delete, find, and reverse.
2.  **Doubly Linked List**: An implementation of a doubly linked list, supporting operations such as append, prepend, and delete.

### Usage

#### Singly Linked List

```python
ll = LinkedList()
ll.insert_values(['banana', 'mango', 'grapes', 'orange'])
print(f"Linked List: {ll}")

ll.insert_after_value('mango', 'apple')
print(f"Linked List: {ll}")

ll.remove_by_value('orange')
print(f"Linked List: {ll}")
```

#### Doubly Linked List

```python
dll = DLinkedList()

dll.append("A")
dll.append("B")
dll.prepend("C")
print(f"Doubly Linked List: {dll}")
print(f"Backward Doubly LinkedList: ", end="")
dll.print_backward()
```
