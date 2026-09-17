# 🔗 Python Data Structures: Linked Lists

A clean, pure Python implementation of **Singly Linked Lists** and **Doubly Linked Lists**. This repository demonstrates fundamental data structure operations including insertion, deletion, bidirectional traversal, in-place reversal, and string representations.

---

## 📌 Features

### 1. Singly Linked List (`LinkedList`)
- **Insertion Operations**: Prepend ($O(1)$), Append ($O(n)$), Insert at Index ($O(n)$), Insert After Value, and Batch Insert (`insert_values`).
- **Deletion Operations**: Remove by Value, Remove at Index, and Delete Head.
- **Utility Methods**: Linear Search (`find`), In-place Reversal (`reverse`), Python list conversion (`to_list`), and `__len__` support.
- **Pythonic Iteration**: Implements `__iter__` to allow native `for item in linked_list` loops.

### 2. Doubly Linked List (`DLinkedList`)
- **Two-Way Pointers**: Nodes maintain references to both `next` and `prev` elements.
- **Efficient Tail Access**: Keeps track of both `head` and `tail` pointers for $O(1)$ appending.
- **Bidirectional Traversal**: Supports forward iteration and backward printing (`print_backward`).

---

## 📁 Repository Structure

```text
.
├── linked_list.py      # Contains LinkedList & DLinkedList class implementations
└── README.md           # Project documentation
```

---

## ⏱️ Time Complexity Summary

| Operation | Singly Linked List | Doubly Linked List |
| :--- | :--- | :--- |
| **Prepend** | $O(1)$ | $O(1)$ |
| **Append** | $O(n)$ *(without tail pointer)* | $O(1)$ *(with tail pointer)* |
| **Delete by Value** | $O(n)$ | $O(n)$ |
| **Find/Search** | $O(n)$ | $O(n)$ |
| **Reverse** | $O(n)$ | $O(n)$ |

---

## 💻 Running in Google Colab

To run this directly in Google Colab or locally:

```bash
git clone https://github.com/ouqbah/Data-Structures.git
```
