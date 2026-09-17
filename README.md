🔗 Python Data Structures: Linked ListsA clean, pure Python implementation of Singly Linked Lists and Doubly Linked Lists. This repository demonstrates fundamental data structure operations including insertion, deletion, bidirectional traversal, in-place reversal, and string representations.   📌 Features1. Singly Linked List (LinkedList)Insertion Operations: Prepend (O(1)), Append (O(n)), Insert at Index (O(n)), Insert After Value, and Batch Insert (insert_values).   Deletion Operations: Remove by Value, Remove at Index, and Delete Head.   Utility Methods: Linear Search (find), In-place Reversal (reverse), Python list conversion (to_list), and __len__ support.   Pythonic Iteration: Implements __iter__ to allow native for item in linked_list loops.   2. Doubly Linked List (DLinkedList)Two-Way Pointers: Nodes maintain references to both next and prev elements.   Efficient Tail Access: Keeps track of both head and tail pointers for O(1) appending.   Bidirectional Traversal: Supports forward iteration and backward printing (print_backward).   📁 Repository StructurePlaintext.
├── linked_list.py      # Contains LinkedList & DLinkedList class implementations
└── README.md           # Project documentation
🛠️ Usage ExamplesSingly Linked ListPythonfrom linked_list import LinkedList

# Initialize and populate list
ll = LinkedList()
ll.insert_values(['banana', 'mango', 'grapes', 'orange'])
print(f"Initial List: {ll}")
# Output: 'banana' -> 'mango' -> 'grapes' -> 'orange' -> None

# Insert after a specific value
ll.insert_after_value('mango', 'apple')
print(f"After Insertion: {ll}")
# Output: 'banana' -> 'mango' -> 'apple' -> 'grapes' -> 'orange' -> None

# Remove a specific value
ll.remove_by_value('orange')
print(f"After Deletion: {ll}")
# Output: 'banana' -> 'mango' -> 'apple' -> 'grapes' -> None

# Reverse the list in-place
ll.reverse()
print(f"Reversed: {ll}")
# Output: 'grapes' -> 'apple' -> 'mango' -> 'banana' -> None
Doubly Linked ListPythonfrom linked_list import DLinkedList

# Initialize Doubly Linked List
dll = DLinkedList()

# Add items to front and back
dll.append("A")
dll.append("B")
dll.prepend("C")

# Forward representation
print(f"Forward: {dll}")
# Output: C <-> A <-> B <-> None

# Backward traversal
print("Backward: ", end="")
dll.print_backward()
# Output: B <-> A <-> C <-> None
⏱️ Time Complexity SummaryOperationSingly Linked ListDoubly Linked ListPrepend$O(1)$$O(1)$Append$O(n)$ (without tail pointer)$O(1)$ (with tail pointer)   Delete by Value$O(n)$$O(n)$Find/Search$O(n)$$O(n)$Reverse$O(n)$$O(n)$💻 Running in Google ColabTo run this directly in Google Colab or locally:Bashgit clone https://github.com/ouqbah/AI_Engineer.git
cd AI_Engineer
python linked_list.py
