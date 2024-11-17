# Odd-Even-Linked-List
This Java solution reorders a singly linked list by placing nodes at odd indices first, followed by nodes at even indices. The purpose of the oddEvenList method is to group all nodes located at odd indices followed by all nodes at even indices, preserving the relative order within each group.

Code Explanation
Edge Case Handling: If the list is empty or has only one node, it returns the list as-is.
Pointer Initialization:
odd points to the head of the list (first odd node).
even points to the second node in the list (first even node).
evenHead stores the head of the even-indexed nodes to link with the end of the odd-indexed nodes later.
Traversal and Rearrangement:
Using a while loop, the code alternates nodes by linking the next odd node, then the next even node, advancing each pointer accordingly.
Final Connection: Once the end of the list is reached, the last odd node is linked to the head of the even nodes to complete the reordering.
Complexity
Time Complexity: 
𝑂(𝑛)
O(n) — Each node is visited once.
Space Complexity: 
𝑂(1)
O(1) — No additional space is used apart from a few pointers.
Example
For an input list 1 -> 2 -> 3 -> 4 -> 5, the output will be reordered as 1 -> 3 -> 5 -> 2 -> 4.

This function is particularly useful for operations where you need to maintain grouped positions in a linked list based on their index parity.
